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
