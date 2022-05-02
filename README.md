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