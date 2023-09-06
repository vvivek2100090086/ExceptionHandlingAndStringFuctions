      //Simple Exception Handling
      public class Main {
          public static void main(String[] args) {
              try {
                  int numerator = 10;
                  int denominator = 0;
                  int result = numerator / denominator; // This line may throw an ArithmeticException
                  System.out.println("Result: " + result);
              } catch (ArithmeticException e) {
                  System.err.println("An error occurred: " + e.getMessage());
                  e.printStackTrace();
              }
              System.out.println("Program continues after handling the exception.");
          }
      }
      
      //String Fuctions
      
      public class Main {
          public static void main(String[] args) {
              
        String str = "Hello, World!";

        // String length
        int length = str.length();
        System.out.println("Length of the string: " + length);

        // Concatenation
        String anotherStr = " Welcome!";
        String concatenatedStr = str + anotherStr;
        System.out.println("Concatenated string: " + concatenatedStr);

        // Substring
        String substring = str.substring(0, 5); // Extract "Hello"
        System.out.println("Substring: " + substring);

        // Character extraction
        char firstChar = str.charAt(0); // Get the first character 'H'
        System.out.println("First character: " + firstChar);

        // String comparison
        String str1 = "apple";
        String str2 = "banana";
        int comparison = str1.compareTo(str2);
        if (comparison < 0) {
            System.out.println(str1 + " comes before " + str2);
        } else if (comparison > 0) {
            System.out.println(str1 + " comes after " + str2);
        } else {
            System.out.println(str1 + " is equal to " + str2);
        }

        // Searching for a substring
        boolean contains = str.contains("World"); // Check if 'World' exists in the string
        System.out.println("Contains 'World': " + contains);

        // String replacement
        String replacedStr = str.replace("World", "Universe");
        System.out.println("Replaced string: " + replacedStr);

        // Splitting a string
        String sentence = "This is a simple sentence.";
        String[] words = sentence.split(" "); // Split by space
        System.out.println("Split sentence: ");
        for (String word : words) {
            System.out.println(word);
        }
    }
}
