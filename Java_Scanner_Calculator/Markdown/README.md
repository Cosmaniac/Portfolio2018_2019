import java.util.Scanner;

public class Main {

  public static void main(String[] args) {
    Scanner scan = new Scanner(System.in);
    float firstN;
    float secondN;
    char operator;
    float answer;
    boolean cont = true;
    char help;
```markdown
    while (cont) {
      System.out.println("Enter the first number you would like to calculate: ");
      firstN = scan.nextFloat();
      scan.nextLine();
      System.out.println("Enter the operator: ");
      operator = scan.next().charAt(0);
      System.out.println("Enter the second number you would like to calculate: ");
      secondN = scan.nextFloat();
      if (operator == '+') {
        answer = firstN + secondN;
        System.out.println("Your answer is: " + answer);
      } else if (operator == '-') {
        answer = firstN - secondN;
        System.out.println("Your answer is: " + answer);
      } else if (operator == '*') {
        answer = firstN * secondN;
        System.out.println("Your answer is: " + answer);
      } else if (operator == '/') {
        answer = firstN / secondN;
        System.out.println("Your answer is: " + answer);
      } else if (operator == '%') {
        answer = firstN % secondN;
        System.out.println("Your answer is: " + answer);
      } else {
        System.out.println("Sorry, not available.");
      }
      scan.nextLine();
      System.out.println("Continue? Y/N");
      help = scan.next().charAt(0);
      if (help == 'Y') {
        cont = true;
      } else if (help == 'N') {
        cont = false;
      } else if (help == 'y') {
        cont = true;
      } else if (help == 'n') {
        cont = false;
      } else {
        System.out.println("Not valid.");
        cont = false;
      }

    }
  }

}
```markdown
