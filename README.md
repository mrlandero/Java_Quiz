# Java_Quiz
We will create a quiz will that asks multiple-choice questions about common trivia. It tracks the user's answers and prints their final score.

## Step 1:

Import the Scanner utility:

```java
import java.util.Scanner;
```

## Step 2:

Create the Quiz class:

```java
public class Quiz {
    public static void main(String[] args) {

    }

}
```

## Step 3:

Inside the Quiz class, initialize a new **Scanner** instance: 

```java
Scanner scan = new Scanner(System.in);
```

## Step 4: 

Ask the 4 questions for the quiz. Do this after the new **Scanner** instance:

```java
        System.out.println("1. Which country held the 2016 Summer Olympics?");
        System.out.println("\ta) China\n\tb) Ireland\n\tc) Brazil\n\td) Italy\n");
        //store answer 1
        String answer1 = scan.nextLine();

        System.out.println("\n2. Which planet is the hottest?");
        System.out.println("\ta) Venus\n\tb) Saturn\n\tc) Mercury\n\td) Mars\n");
        //store answer 2
        String answer2 = scan.nextLine();

        System.out.println("\n3. What is the rarest blood type?");
        System.out.println("\ta) O\n\tb) A\n\tc) B\n\td) AB-Negative\n");
        //store answer 3
        String answer3 = scan.nextLine();

        System.out.println("\n4. Which one of these characters is friends with Harry Potter?");
        System.out.println("\ta) Ron Weasley\n\tb) Hermione Granger\n\tc) Draco Malfoy\n");
        //store answer 4
        String answer4 = scan.nextLine();
```

## Step 5:

Initialize a score variable to 0. Then add 5 points to the user's score for every question they answer correctly. We achieve this with some if-statements:

```java
        int score = 0;


        //Task 2: Check each answer - For each correct answer, add 5 points to the score. 
        if (answer1.equals("c")) {
            score += 5;
        }
        if (answer2.equals("a")) {
            score += 5;
        }
        if (answer3.equals("d")) {
            score += 5;
        }
        if (answer4.equals("a") || answer4.equals("b")) {
            score += 5;
        } 
```

## Step 6: 

Print the user's score. Write if-statements to display to the user how they performed on the quiz:

```java
        System.out.println("Your final score is: " + score + "/20");

        //Task 3: print a message depending on the score
        if (score > 15) {
            System.out.println("Wow! You know your stuff");
        } else if (score >= 5 && score <= 15) {
            System.out.println("Not bad!");
        } else {
            System.out.println("Better luck next time!");
        }
```

## Step 7:

Close the **Scanner** instance to avoid any data leaks:

```java
scan.close();
```

## Step 8: 

Test the application compiling and running the program and answer the questions. 