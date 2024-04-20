# Multi-Threading
<img width="1112" alt="Screenshot 2024-04-20 at 9 48 39 PM" src="https://github.com/rishavjain2002/Multi-Threading/assets/73553612/0f8c33db-ab89-4b3b-85ee-e8085498e61e">

# Multi-threaded Matrix Multiplication

## Methodology
The methodology employed in this project involves measuring the performance of matrix multiplication using multiple threads in Python. The matrix multiplication operation is parallelized using threading to utilize multiple CPU cores efficiently.

1. **Matrix Multiplication Function**: The `matrix_multiply` function computes the matrix product of two input matrices using NumPy's `dot` function and stores the result in a specified array.
   
2. **Multi-threaded Matrix Multiplication**: The `multiply_with_threads` function spawns a specified number of threads, each responsible for performing matrix multiplication on randomly generated matrices concurrently. After all threads have finished execution, the total time taken for the operation and the CPU usage are recorded.

3. **Experimental Setup**: The experiment is conducted using various thread counts ranging from 1 to 8. For each thread count, the actual time taken for matrix multiplication and the CPU usage are measured.

## Result Table
The result table presents the experimental results obtained from running the multi-threaded matrix multiplication with different numbers of threads. It includes the following columns:

- **Threads**: The number of threads used for matrix multiplication.
- **Time (s)**: The actual time taken for matrix multiplication in seconds.
- **CPU Usage (%)**: The CPU usage during the computation.
- **Expected Time (ms)**: The expected time for matrix multiplication, used for comparison.

## Result Graph
The result graph visually represents the relationship between the number of threads and the time taken for matrix multiplication. It consists of two lines:

- **Actual Time (s)**: This line graph shows the actual time taken for matrix multiplication with different thread counts.
- **Expected Time (s)**: This line graph represents the expected time for matrix multiplication based on theoretical calculations or benchmarks.

## Interpretation
- **Performance Improvement**: The graph can be analyzed to observe how the performance scales with an increasing number of threads. Ideally, as the number of threads increases, the total computation time should decrease due to parallelization.
- **Concurrency Overhead**: Any overhead or diminishing returns in performance due to increased concurrency can also be observed from the graph.
- **Comparison with Expectations**: The comparison between actual and expected times provides insights into the efficiency of the multi-threaded implementation and any deviations from theoretical expectations.
