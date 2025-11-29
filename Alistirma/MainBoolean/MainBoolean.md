Great question! 🎯  
Right now, your code is **procedural** — everything happens inside `main`. To make it **object-oriented (OOP)**, we should encapsulate logic into classes and methods, and separate responsibilities. Let me show you how to refactor your prime-checker program into a more OOP style.

---

## 🛠 Steps to Refactor into OOP
1. **Create a class** to represent the concept of a number and its prime-checking logic.  
2. **Encapsulate behavior** (prime checking) inside methods.  
3. **Use objects** instead of static code in `main`.  
4. **Keep `main` clean** — only handle input/output and delegate logic to objects.

---

## ✅ Example OOP Code

```java
import java.util.Scanner;

// Class that encapsulates prime-checking logic
class PrimeChecker {
    private int number;

    // Constructor
    public PrimeChecker(int number) {
        this.number = number;
    }

    // Method to check if the number is prime
    public boolean isPrime() {
        if (number <= 1) return false;
        for (int i = 2; i <= number / 2; i++) {
            if (number % i == 0) {
                return false;
            }
        }
        return true;
    }

    // Method to display result
    public void printResult() {
        System.out.println(isPrime() ? "prime" : "not prime");
    }
}

// Main class
public class MainBool {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int n = s.nextInt();

        // Create an object of PrimeChecker
        PrimeChecker checker = new PrimeChecker(n);

        // Use object methods
        checker.printResult();
    }
}
```

---

## 🔍 What Changed?
- **Encapsulation**: The prime-checking logic lives inside `PrimeChecker`.  
- **Abstraction**: `main` doesn’t care how `isPrime()` works, it just calls it.  
- **Objects**: We create a `PrimeChecker` object with the input number.  
- **Clean main**: Input/output only, no logic clutter.

---

👉 This is a simple example, but you could extend it:
- Add methods for checking other properties (e.g., even/odd, factorial).  
- Create a `NumberAnalyzer` class that uses multiple checkers.  
- Use inheritance if you want specialized number types.

Would you like me to show you a **more advanced OOP version** with multiple classes (like `NumberAnalyzer` and `PrimeChecker`), or keep it simple like this?
