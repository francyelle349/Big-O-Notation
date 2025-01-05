# Big-O-Notation
Studies about Big O notation - Computer Science.

O(1) - 

In computer science, O(1), also called constant time complexity, refers to an algorithm or operation whose execution time does not depend on the size of the input. In other words, regardless of how large the dataset or input grows, the time taken to perform the operation remains the same.

Key Characteristics of 𝑂(1)

- Predictable Performance: The operation executes in a fixed amount of time.
- Independent of Input Size: Even if the input increases significantly, the time taken does not change.
- Examples in Data Structures:
Accessing an Array Element by Index: Since array indices provide direct access, it takes the same amount of time, regardless of the size of the array.
HashMap Access (Ideally): A properly implemented hash table retrieves values in 
O(1) on average.

### Real-World Analogy
Imagine a bookshelf where each book is labeled with a number. If you know the number, you can directly go to that book without searching through the entire shelf. The time it takes to retrieve a specific book remains constant, whether there are 10 or 1,000 books.

### Example

public class Example {
    public static void main(String[] args) {
        // Example array
        int[] numbers = {10, 20, 30, 40, 50};
        
        // Accessing an element by index (O(1))
        int index = 2; // access the 3rd element
        int value = numbers[index]; // Always constant time

   
        System.out.println("Value at index " + index + ": " + value);

        // Modifying an element by index 
        numbers[index] = 100; // Modifies the 3rd element
        System.out.println("Updated value at index " + index + ": " + numbers[index]);
    }
}

O(N) - 

Called linear time complexity, basically describes an algorithm or operation whose execution time grows linearly to the size of the Input N. 

Key Characteristics of 𝑂(N)

- Direct relationship with the input size: If the input size doubles, this means the execution time it will double too.
- Iterative processes: Operations that evolves traversing or processing every element of the list typically is O(N) complexity.
- Example in DS:
-     Linear Search
-     Summing Array Elements
-      Finding the Maximum Element in an Array
-      copying a List

### Example code in Java:


        public class Example {
            public static void main(String[] args) {
        
        int[] numbers = {10, 20, 30, 40, 50};
        
        // Summing up
        int sum = 0;
        for (int number : numbers) { // This loop runs N times
            sum += number;
        }

        // Displaying 
        System.out.println("Sum of array elements: " + sum);
        }
        }

O(N²)

The runtime of the Algorithm grows quadratically with the size of the input.
This occurs when you have nested loops, where the inner loop iterates through all or most of the elements for every iteration of the outer of loop.

Real-World Analogy

Imagine a group of students where every student has to greet every other student. If there are 5 students, there will be 5×5=25 greetings. If the group size increases, the total greetings grow quadratically.

    public class Example2 {
    public static void main(String[] args) {
        int[] numbers = {1, 2, 3, 4};

        // Nested loops (O(N²))
        for (int i = 0; i < numbers.length; i++) { // Outer loop
            for (int j = 0; j < numbers.length; j++) { // Inner loop
                System.out.println("Pair: (" + numbers[i] + ", " + numbers[j] + ")");
            }
        }
    }
    }


O(N³)
represents algorithms whose runtime grows cubically with the size of the input.

Example

       public class Example2 {
    public static void main(String[] args) {
       int n = 3;
        // Triple nested loops 
        for (int i = 0; i < n; i++) { // Outer loop
            for (int j = 0; j < n; j++) { // Middle loop
                for (int k = 0; k < n; k++) { // Inner loop
                    System.out.println(" (" + i + ", " + j + ", " + k + ")");
                }
            }
        }
    }
}
O(n * m)

Traversing a rectangular grid

Its used with a scenario where two dimensions need to be processed, such as traversing elements in a rectangular grid with N rows and M columns.

Key Characteristics 
- Two Nested Loops
- Grid-like Strcutures (2d arrays, or any DS represeting a rectangular region)

### Example

      public class Example2 {
    public static void main(String[] args) {
        int[][] grid = {{1,2,3}, {1,2,3}};


        for(int i = 0; i < grid.length; i++){ outer loop N rows
            for(int j = 0; j < grid[i].length;j++){ inner loop M columns
                System.out.print("("+grid[i][j]+")");
            }
            System.out.println();
        }
    }
}

Pratical Examples
- Matrix operations and Image Operations


O(log n)

O(n log n)

O(2n)




