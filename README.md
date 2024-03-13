# Module 5

Hasil JMeter sebelum Profiling
Best Practice menggunakan CLI

1. /all-student
   ![image](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/2f217a14-07a9-4aaa-9cb3-d0c5b8f64b87)

2. /all-student-name
   ![image](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/758717d6-ce3c-4ef9-a28c-e6e82314ab41)

3. /highest-gpa
   ![image](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/bba9842e-33c5-4c74-9ae5-0b9d6c140fa9)

<br>

GUI Results
1. /all-student
   ![WhatsApp Image 2024-03-12 at 22 18 49_ea13629c_0](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/14d56da4-787a-4df2-9101-690ab3470705)
   
2. /all-student-name
   ![WhatsApp Image 2024-03-12 at 22 45 48_b56220ca_0](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/9c1c4867-5097-45ee-86d0-8eddb2a43be3)

3. /highest-gpa
   ![WhatsApp Image 2024-03-12 at 22 42 55_13fbeece_0](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/a315704b-9042-41e6-8dac-000bcc41f8cc)
 
<br> 

Hasil JMeter setelah Profiling
Best Practice menggunakan CLI

1. /all-student
   ![image](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/bb00c674-0b0c-44c2-9d1f-95275f99bce9)

2. /all-student-name
   ![image](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/8a4cb7e0-9161-47ad-994d-08ec27364824)

3. /highest-gpa
   ![image](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/e971cd1b-800d-49f7-9612-33e7a4805a55)

<br>

GUI Results

1. /all-student
   <img width="976" alt="Screenshot 2024-03-13 141952" src="https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/7a840cda-f590-438e-bed3-48b23d3e4546">
   
2. /all-student-name
   ![image](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/91fe4fcf-6bc8-4120-a33a-bdc3e5943e92)

3. /highest-gpa
   ![image](https://github.com/MRadhityaUtomo/exercise-profiling/assets/124948533/cd27ab2e-80cc-47e7-9636-ad8f6c7caed0)


<br>
<br>

## Reflection

1. 
- JMeter is used to test system performance. The use of JMeter simulates many users and various types of loads by sending requests to predefined endpoints and then checking whether these requests can be executed and receive responses. Jmeter also displays the statistical results via listeners like tables and graphs. 
- Profiling provides where the problems lie by detecting which code takes the most time in running by identifying statistics like CPU Time and Execution Time.
2. Profiling gives insights like CPU Time and Execution Time. Visually it detects bottlenecks by tagging them with high saturated colors in a graph.
3. Definitely, like mentioned above, it gives clear statistics and pinpoints the bottlenecks after running a request. For example and clarity the `getAllStudentName()` method had a 3k+ CPU time and thanks to Intellij's profiler it was detected as such.
4. My main issue the first time trying to identify a bottleneck was trying to understand the meanings and how to read the graphs like the flame graph. Overcoming it was me analyzing it in detail, both Jmeter and Intellij Profiler
5. Easier time identifying unoptimized code by giving in depth data and statistics.
6. To address situations where the profiling results are not entirely consistent with the results from JMeter, I conduct and perform more performance testing using JMeter and also avoid benchmarking using the initial performance test results when the program is running because the JIT compiler on the JVM is not yet fully optimized, which can make it slower.
7. After analyzing the results of performance testing and profiling, my first step is to identify the bottleneck points contributing the most to the overall performance degradation. Then, I attempt to optimize the identified code sections that are slowing down performance by refactoring them to improve efficiency. Subsequently, I conduct performance testing and profiling again to verify if there has been an improvement in performance.
To ensure that the applied changes do not affect the program's functionality, I verify that the output remains the same as before the code alteration or achieves the expected output by creating and executing unit tests.
