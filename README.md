# Factorial Using Recursion

## Problem Statement

Given a non-negative integer `n`, find its factorial using recursion.

The factorial of a number `n` is the product of all positive integers less than or equal to `n`.

## Formula

:contentReference[oaicite:0]{index=0}

## Example

Input:
```text
5
```

Output:
```text
120
```

Explanation:

```text
5! = 5 × 4 × 3 × 2 × 1 = 120
```

## Approach

1. Define a recursive function `factorial(n)`.
2. If `n` is `0` or `1`, return `1` (base case).
3. Otherwise, return `n * factorial(n - 1)`.
4. Print the result.

## Java Solution

```java
import java.util.*;

class Main {

    static long factorial(int n) {
        if (n == 0 || n == 1) {
            return 1;
        }
        return n * factorial(n - 1);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        System.out.println(factorial(n));
    }
}
```

## Recursion Trace

```text
factorial(5)
= 5 × factorial(4)
= 5 × 4 × factorial(3)
= 5 × 4 × 3 × factorial(2)
= 5 × 4 × 3 × 2 × factorial(1)
= 5 × 4 × 3 × 2 × 1
= 120
```

## Complexity Analysis

- **Time Complexity:** O(n)
- **Space Complexity:** O(n)

## Tags

`Recursion` `Math` `Basic Programming`
