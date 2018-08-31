```markdown
//original made by Hayden Soelberg
import java.util.Scanner;

class Main {
  public static void main(String[] args) {
    Scanner scan = new Scanner(System.in);
    float dailyOunces;
    float longevity;
    float totalTankers;

    System.out.println("Please enter the average amount of cups consumed daily: ");
    dailyOunces = 8 * scan.nextFloat();

    System.out.println("Please enter the number of years/months/days you would like to calculate(years, enter, months, enter, etc.): ");
    int years = scan.nextInt();

    scan.nextLine();
    int months = scan.nextInt();

    scan.nextLine();
    int days = scan.nextInt();

    longevity = (days) + (months * 30.42f) + (years * 365);

    float ouncesTotal = longevity * dailyOunces;

    totalTankers = (0.0078125f * ouncesTotal) / (11000f);

    /*if (ouncesTotal % 1408000 > 0) {
      totalTankers += 1;
    } else {
    }*/
    System.out.println("You will need " + totalTankers + " to survive " + longevity + " days, or " + years + " years, " + months + " months, and " + days + " days.");

  }
}
```
