# 30 Patterns Question

Print these patterns using loops:


<!-- que 1 --->

<details>
<summary>

```
1.  *****
    *****
    *****
    *****
    *****
```
</summary>

```java
    public static void main(String[]args) {
        pattern1(5);
    }
    static void pattern1(int n) {
        for (int row = 0; row < n; row++) {
            for (int col = 0; col < n; col++) {
                System.out.print("* ");
            }
            System.out.println(" ");
        }
    }
```

</details>


<!-- que 2 --->

<details>
<summary>

```
2.  *
    **
    ***
    ****
    *****
```
</summary>

```java
    public static void main(String[]args) {
        pattern2(5);
    }
    static void pattern2(int n) {
        for (int row = 1; row <= n; row++) {
            for (int col = 0; col < row; col++) {
                System.out.print("* ");
            }
            System.out.println(" ");
        }
    }
```

</details>



<!-- que 3 --->

<details>
<summary>

```
3.  *****
    ****
    ***
    **
    *
```
</summary>

```java
    public static void main(String[]args) {
        pattern3(5);
    }
    static void pattern3(int n) {
        for (int row = n; row > 0; row--) {
            for (int col = 0; col < row; col++) {
                System.out.print("* ");
            }
            System.out.println(" ");
        }
    }
```

</details>



<!-- que 4 --->

<details>
<summary>

```
4.  1
    1 2
    1 2 3
    1 2 3 4
    1 2 3 4 5
```
</summary>

```java
    public static void main(String[]args) {
        pattern4(5);
    }
    static void pattern4(int n) {
        for (int row = 1; row <= n; row++) {
            for (int col = 1; col <= row; col++) {
                System.out.print( col + " ");
            }
            System.out.println(" ");
        }
    }
```

</details>



<!-- que 5 --->

<details>
<summary>

```
5.  *
    **
    ***
    ****
    *****
    ****
    ***
    **
    *
```
</summary>

```java
    public static void main(String[]args) {
        pattern5(5);
    }
    static void pattern5(int n) {
        for (int row = 0; row < 2 * n; row++) {
            int totalColsInRow = row > n ? 2 * n - row : row;
            for (int col = 0; col < totalColsInRow; col++) {
                System.out.print("* ");
            }
            System.out.println(" ");
        }
    }
```

</details>



<!-- que 6 --->

<details>
<summary>

```
6.       *
        **
       ***
      ****
     *****
```
</summary>

```java
    public static void main(String[]args) {
        pattern6(5);
    }
    static void pattern6(int n) {
        for (int row = 1; row <= 5; row++) {
            int noOfSpaces = n - row;
            for (int space = 0; space < noOfSpaces; space++) {
                System.out.print(" ");
            }
            for (int col = 0; col < row; col++) {
                System.out.print("*");
            }
            System.out.println(" ");
        }
    }
```

</details>



<!-- que 7 --->

<details>
<summary>

```
7.   *****
      ****
       ***
        **
         *
```
</summary>

```java
    public static void main(String[]args) {
        pattern7(5);
    }
    static void pattern7(int n) {
        for (int row = n; row > 0; row--) {
            int noOfSpaces = n - row;
            for (int space = 0; space < noOfSpaces; space++) {
                System.out.print(" ");
            }
            for (int col = 0; col < row; col++) {
                System.out.print("*");
            }
            System.out.println(" ");
        }
    }
```

</details>



<!-- que 8 --->

<details>
<summary>

```
8.      *
       ***
      *****
     *******
    *********
```
</summary>

```java
    public static void main(String[]args) {
        pattern8(5);
    }
    static void pattern8(int n) {
        for (int row = 0; row < n; row++) {
            int noOfSpaces = n - row;
            for (int space = 0; space < noOfSpaces; space++) {
                System.out.print(" ");
            }
            for (int col = 0; col < 2 * row + 1; col++) {
                System.out.print("*");
            }
            System.out.println(" ");
        }
    }
```

</details>



<!-- que 9 --->

<details>
<summary>

```
9.  *********
     *******
      *****
       ***
        *
```
</summary>

```java
    public static void main(String[]args) {
        pattern9(5);
    }
    static void pattern9(int n) {
        for (int row = n; row > 0; row--) {
            int noOfSpaces = n - row;
            for (int space = 0; space < noOfSpaces; space++) {
                System.out.print(" ");
            }
            for (int col = 0; col < 2 * row - 1; col++) {
                System.out.print("*");
            }
            System.out.println(" ");
        }
    }
```

</details>



<!-- que 10 --->

<details>
<summary>

```
10.      *
        * *
       * * *
      * * * *
     * * * * *
```
</summary>

```java
    public static void main(String[]args) {
        pattern10(5);
    }
    static void pattern10(int n) {
         for (int row = 0; row <= n; row++) {
            int noOfSpaces = n - row;
            for (int space = 0; space < noOfSpaces; space++) {
                System.out.print(" ");
            }
            for (int col = 0; col < row ; col++) {
                System.out.print("* ");
            }
            System.out.println(" ");
          }
     }
```

</details>



<!-- que 11 --->

<details>
<summary>

```
11.  * * * * *
      * * * *
       * * *
        * *
         *
```
</summary>

```java
    public static void main(String[]args) {
        pattern11(5);
    }
    static void pattern11(int n) {
        for (int row = n; row > 0; row--) {
            int noOfSpaces = n - row;
            for (int space = 0; space < noOfSpaces; space++) {
                System.out.print(" ");
            }
            for (int col = 0; col < row ; col++) {
                System.out.print("* ");
            }
            System.out.println(" ");
        }
    }
```

</details>


<!-- que 12 --->

<details>
<summary>

```
12.  * * * * *
      * * * *
       * * *
        * *
         *
         *
        * *
       * * *
      * * * *
     * * * * *
```
</summary>

```java
    public static void main(String[]args) {
        pattern12(5);
    }
    static void pattern12(int n) {
        for (int row = n; row > 0; row--) {
            int noOfSpaces = n - row;
            for (int space = 0; space < noOfSpaces; space++) {
                System.out.print(" ");
            }
            for (int col = 0; col < row ; col++) {
                System.out.print("* ");
            }
            System.out.println(" ");
        }
        for (int row = 0; row <= n; row++) {
            int noOfSpaces = n - row;
            for (int space = 0; space < noOfSpaces; space++) {
                System.out.print(" ");
            }
            for (int col = 0; col < row ; col++) {
                System.out.print("* ");
            }
            System.out.println(" ");
        }
    }
```

</details>




<!-- que 13 --->

<details>
<summary>

```
13.      *
        * *
       *   *
      *     *
     *********
```
</summary>

```java
    static void pattern13(int n) {
        for (int row = 1; row <= n ; row++) {
            for (int space = row; space <= n ; space++) {
                System.out.print(" ");
            }
            for (int col = 1; col <= (2*row -1) ;col++) {
                if( col == 1 || row == n || col == (2 * row - 1)) {
                    System.out.print("*");
                }
                else {
                    System.out.print(" ");
                }
            }
            System.out.println("");
        }
    }
```

</details>



<!-- que 14 --->

<details>
<summary>

```
14.  *********
      *     *
       *   *
        * *
         *
```
</summary>

```java
   static void pattern14(int n) {
        for (int row = n; row  > 0; row--) {
            int noOfSpace = n - row ;
            for (int space = 0; space < noOfSpace; space++) {
                System.out.print(" ");
            }
            for (int col = 1; col <= 2*row-1; col++) {
                if(col == 1 || row == n || col == 2 * row -1  ){
                    System.out.print("*");
                }else {
                    System.out.print(" ");
                }
            }
            System.out.println(" ");
        }
    }
```

</details>



<!-- que 15 --->

<details>
<summary>

```
15.      *
        * *
       *   *
      *     *
     *       *
      *     *
       *   *
        * *
         *
```
</summary>

```java
    static void pattern15(int n) {
        for (int row = 1; row <= n; row++) {
            int noOfSpace = n - row;
            for (int space = 0; space < noOfSpace; space++) {
                System.out.print(" ");
            }
            for (int col = 1; col <= 2*row-1; col++) {
                if(col == 1 || col == 2* row -1){
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println(" ");
        }
        for (int row = n-1; row > 0; row--) {
            int noOfSpace =n - row;
            for (int space = 0; space < noOfSpace; space++) {
                System.out.print(" ");
            }
            for (int col = 1; col <= 2*row-1; col++) {
                if(col == 1 || col == 2* row -1){
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println(" ");
        }
```

</details>



<!-- que 16 --->

<details>
<summary>

```
16.           1
            1   1
          1   2   1
        1   3   3   1
      1   4   6   4   1

```
</summary>

```java
    public static void main(String[]args) {
        pattern16(5);
    }
    static void pattern16(int n) {
        for (int row = 1; row <= 5; row++) {
            int noOfSpace =  n -row;
            for (int space = 0; space <= noOfSpace; space++) {
                System.out.print(" ");
            }
            int c = 1;
            for (int col = 1; col <= row; col++) {
                System.out.print(c + " ");
                c = c* (row - col) / col;
            }
            System.out.println();
        }
    }
```

</details>











