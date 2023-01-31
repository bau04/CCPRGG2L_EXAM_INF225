public class App {
    public static void main(String[] args) throws Exception {
        // Remove letters (30 pts)

        // Instructions (Important!)

        // Without using arrays or loops or regular expressions, apply recursion to remove specific letters in
        // your full name.

        // 1. If the last letter of your surname is a vowel, remove all vowels in
        // your full name.

        // 2. If the last letter of your surname is a consonant, remove all
        // consonants in your full name.

        // 3. Use only lowercase letters
        
        // 4. Each letter should be removed one by one.

        // Example:
        // Full name is "elizer ponio jr".
        // The output should be "lzr pn jr".

        // Put your complete name in the "fullName" variable.
        // Example:
        // String fullName = "elizer ponio jr";

        String fullName = "charles denzel bautista";

        removeLetter1(fullName);
    }


    static void removeLetter1(String str) {
        
        int NameLength = str.length();
        int spaceIndex = str.lastIndexOf(" ") + 1;

        String surname = str.substring(spaceIndex, NameLength);

        char LastLetter = surname.charAt(surname.length() - 2);

        String vowels1 = "aeiou";

        int vowelCheck = vowels1.indexOf(LastLetter) >= 0 ? 0 : 1;

        String result = removeLetter2(str, vowelCheck, "", 0);
        System.out.println(result);
    }
    
    private static String removeLetter2(String fullName, int vowelCheck, String result, int index) {

        if (index >= fullName.length())
        {
          return result;
        }
         
        char letter = fullName.charAt(index);

        String vowels2 = "aeiou";
        
        int isVowel = vowels2.indexOf(letter) >= 0 ? 0 : 1;
        
        return removeLetter2(fullName, vowelCheck, isVowel == vowelCheck ? result + letter : result, index + 1);
    }
}

