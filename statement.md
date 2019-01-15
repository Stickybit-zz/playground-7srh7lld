
# Java Interview Questions and Programming Examples

## Java Language Questions

![Java Books Library](https://iili.io/Hpk7I.jpg)

Questions relating to the Java language check the developer’s ability to use functionalities that are well-known. Using the correct APIs and data structures determine the developer's level of experience in the practice of the Java programming language. This skill is particularly important for a developer who has to be quickly operational in a Java working environment.

An example of very simple task consists in writing a method which takes a string `str` as parameter and returns `true` if it equals to `"Hello World"`, `false` otherwise.

```java runnable
public class Main {

    static boolean isHelloWord(String str) { 
        return str == "Hello World"; // scary code (@see https://www.codingame.com/playgrounds/1097/the-most-common-java-pitfalls)
        return str.equals("Hello World"); // correct, but what happens if str is null?
        return "Hello World".equals(str); // expected solution
    }
    
    public static void main(String[] args) {
        System.out.println(isHelloWord("Hello World"));
    }
}
```

## Java Problem Solving Questions

![Java Algorithms](https://www.geeksforgeeks.org/wp-content/uploads/Competitive-Programming-1.jpg)

This skill corresponds to the developer's ability to evaluate and resolve a problem by writing an efficient algorithm in Java. Any developers should be able to solve simple problems but advanced analytical skills and logical reasoning are essential when your are hiring Java R&D developers. Problem Solving exercises cover several topics like the graph theory, dynamic programming and the number theory.

An example of a simple problem is: 
> *From a given array of natural numbers, return the distance between the two closest numbers.*

```java runnable
import java.util.*;

public class Main {

    // Returns the distance between the two closest numbers.
    static int distClosestNumbers(int[] numbers) { 
        // try to implement it!
    }
    
    public static void main(String[] args) {
        int[] testArray = {3, 9, 50, 15, 99, 7, 98, 65};
        int result = distClosestNumbers(testArray);
        System.out.println(result); // Expected result is 1 (the 2 closest numbers are 98 and 99)
    }
}
```

A basic solution consists in: for each number, compare it to all the other numbers. This solution takes a long time to process large data sets, its time complexity is O(n²) then it will fail on some test cases. A more efficient solution consists in a two steps algorithm: 

 1. sort the array using a built-in function like `Arrays.sort()` which has a time complexity of O(n log n).
 2. iterate through the sorted array and compare each number to the previous one.

See? This is much better!

## Java Design Questions

![Application architecture and design](https://www.timeshighereducation.com/sites/default/files/styles/the_breaking_news_image_style/public/why-study-architecture_0.jpg)

Having a good understanding of the design patterns, OOP (object-oriented programming) and unit tests give an indication of the developer's ability to implement standard solutions to common problems. A developer with a good level of proficiency in this skill will contribute to increase the maintainability and the extensibility of applications. This skill is particularly important for senior Java developers who will have to work on the architecture of applications to design long-term solutions.

This is a simple question example:
> *Among these Java method declarations, which is usually the preferred one?*
```java
1) public HashMap getTable()
2) public Map getTable()
3) public Hashtable getTable()
```
A general rule of thumb is to prefer interface over implementation, it improves code maintenance, testability and code portability. `Map getTable()` is the expected answer.

## Java Readability Questions

![Code readability](https://cdn.tutsplus.com/net/uploads/legacy/516_code/preview.jpg)

This metric focus on the developer’s ability to follow the Java guidelines and best practices. A high score means that the code is easily understandable by other programmers, easier to maintain and to debug. For example, `private String Name;` will impact the readability score because it does not respect the Java naming convention: `Name` should be written `name`.

## Java Reliability Questions

![Fixing bugs in practice](https://i.imgur.com/HTisMpC.jpg)

Remember `str.equals("Hello World")` upper? What happens if `str` is `null`? 🧐 This kind of error is like a mine silently waiting in a program.

Reliability refers to the developer's ability to achieve solutions that address specific cases like corner and edge cases. The higher this skill, the higher the developer anticipates possible errors and minimizes those to build robust programs.

## About CodinGame Assessment

Coding tests are one of the most efficient ways to screen developers before hiring.

The CodinGame Java online tests assess candidates' skills. They are perfect for pre-employment screening for developers. Most of the coding interview tools focus only on the candidates' ability to write efficient algorithms but algorithms are a tiny part of software development, mastering them is one skill among several other important skills. [CodinGame Assessment](https://www.codingame.com/work/solutions/coding-skill-assessment/) provides tests covering a wide scope of technical characteristics to evaluate candidates' ability to write good Java programs.

They provide a proven model for identifying and hiring proficient developers. Candidates code their way through real, practical problems that they could encounter in a company (such as finding a bug in a defective piece of code or properly synchronizing a multi-threaded application), enabling recruiters to measure their coding skills objectively and efficiently.

Tech recruiters to HR managers can set up coding tests using platforms like CodinGame, choosing to test applicants in one specific programming language or over multiple technologies (Java, Angular, Python, etc.).

Candidates’ code is automatically analyzed and recruiters are provided with performance metrics. Once completed, a [test report](https://www.codingame.com/work/candidates-demo/74) is available to download and share to easily compare and shortlist candidates.

[![Foo](https://iili.io/HT9Wv.png)](https://www.codingame.com/work/solutions/coding-skill-assessment/)
