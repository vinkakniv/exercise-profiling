# Advanced Programming - Tutorial 


------------
## Overview

This repository contains the code and reflection for Tutorial 5 in Advanced Programming course by Vinka Alrezky As (NPM: 2206820200)❄️
- [Tutorial 5](#tutorial-5)

------------
# Tutorial 5

- `All-Student` Result - Before Optimization

   <img src="https://i.imgur.com/AaSWwYb.jpeg" width="200" alt="">
   <img src="https://i.imgur.com/XmseIlr.jpeg" width="200" alt="">
   <img src="https://i.imgur.com/bGHGRgs.jpeg" width="200" alt="">
   <img src="https://i.imgur.com/oEpEo1x.jpeg" width="200" alt="">
   <img src="https://i.imgur.com/kYU3pBg.jpeg" width="200" alt="">

  `All-Student` Result - After Optimization

  <img src="https://i.imgur.com/EHgbk2p.png" width="200" alt="">
  <img src="https://i.imgur.com/tjjdprx.png" width="200" alt="">
  <img src="https://i.imgur.com/1b4RZrH.png" width="200" alt="">
  <img src="https://i.imgur.com/gq7pFpv.png" width="200" alt="">
  <img src="https://i.imgur.com/8QJWAe2.png" width="200" alt="">

- `All-Student-Name` Result - Before Optimization

  <img src="https://i.imgur.com/9dXEOTI.jpeg" width="200" alt="">
  <img src="https://i.imgur.com/qCvbPaf.jpeg" width="200" alt="">
  <img src="https://i.imgur.com/ultzFHq.jpeg" width="200" alt="">
  <img src="https://i.imgur.com/y74Ycvv.jpeg" width="200" alt="">
  <img src="https://i.imgur.com/6XwZ4Je.jpeg" width="200" alt="">
  
  `All-Student-Name` Result - After Optimization

  <img src="https://i.imgur.com/XWegM3X.png" width="200" alt="">
  <img src="https://i.imgur.com/dz5iXJU.png" width="200" alt="">
  <img src="https://i.imgur.com/O1RPJ41.png" width="200" alt="">
  <img src="https://i.imgur.com/glACL95.png" width="200" alt="">
  <img src="https://i.imgur.com/JMWcIbw.png" width="200" alt="">
  
- `Highest-GPA` Result - Before Optimization

   <img src="https://i.imgur.com/Swf7V1w.jpeg" width="200" alt="">
   <img src="https://i.imgur.com/jva3IEJ.jpeg" width="200" alt="">
   <img src="https://i.imgur.com/ciw2EIZ.jpeg" width="200" alt="">
   <img src="https://i.imgur.com/zYOPRP0.jpeg" width="200" alt="">
   <img src="https://i.imgur.com/AjfH7nT.jpeg" width="200" alt="">
  
  `Highest-GPA` Result - After Optimization

  <img src="https://i.imgur.com/I11q0xB.png" width="200" alt="">
  <img src="https://i.imgur.com/E6SKThx.png" width="200" alt="">
  <img src="https://i.imgur.com/3T3wqmx.png" width="200" alt="">
  <img src="https://i.imgur.com/Vkd8MBA.png" width="200" alt="">
  <img src="https://i.imgur.com/dfEd8uV.png" width="200" alt="">

  
  > After the optimization process, the performance testing results from JMeter showed a significant improvement compared to the initial measurements.
From the images above, we can clearly see the difference in performance before and after the optimization process. The `/all-student`, `/all-student-name` and `/highest-gpa` results show a noticeable improvement in response times and overall system efficiency after the optimization.
The response times were lower, and the system was able to handle a larger load without any degradation in performance. This indicates the effectiveness of the profiling and performance optimization process in improving the efficiency and scalability of the application.

### Reflection

1. What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?
  > Performance testing with JMeter provides me with response times but doesn't offer insight into how the code processes these requests. On the other hand, IntelliJ Profiler helps me identify the parts of the code that cause delays. It allows me to focus on optimizing the sections of code that contribute to longer execution times. While JMeter checks overall performance, IntelliJ Profiler digs into the code to solve specific problems.
2. How does the profiling process help you in identifying and understanding the weak points in your application?
  > Profiling provides detailed insights into its runtime behavior, resource usage, and performance characteristics. Profiling helps me pinpoint the parts of my code that could be causing slow performance. It eliminates the need for manual inspection or execution of every piece of code to find what's causing the slowdown. This is a significant time-saver compared to testing each code segment individually.
3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?
  > I find IntelliJ Profiler to be effective in helping me analyze and identify bottlenecks in my application code. When I run the application with profiling and send requests, I can stop the profiling process after getting the response and easily understand why the application might be slow. The IntelliJ IDE highlights slow-running methods in the profiling results, showing the total execution time in milliseconds.
  This feature not only simplifies the identification of performance bottlenecks but also helps in prioritizing optimization efforts effectively.
4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?
  > The main challenge I face is optimizing slow-running code based on the results of performance testing and profiling. I overcome this by exploring different optimization methods. For example in getAllStudentsWithCourses(). At first, I thought I could improve things just by changing how the loop worked. But then I found out that I could use the studentCourseRepository to get the same thing done, without needing a loop at all. This new way of thinking let me find better ways to make the code run faster, not just by changing the existing methods.
5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?
  > One aspect of IntelliJ Profiler that I find particularly beneficial is its user-friendly nature. With a single button press, I can initiate the profiling process, and there's no need for any additional configuration. Besides that, the most significant advantage is its integration with the IDE, which means I don't need to switch between applications. I can conduct all my profiling tasks within a single application, which greatly enhances my productivity and efficiency.
6. How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?
  > When the outcomes from IntelliJ Profiler don't match with those from JMeter, I consider the variations that might occur during profiling. I try profiling multiple times to see if the discrepancies are consistent or temporary. If the discrepancies continue to appear after multiple trials, I start to consider other elements that might be contributing to the divergence, such as the distinct functionalities of JMeter and IntelliJ Profiler. I also make it a point to restart my IntelliJ and repeat the process. Hence, it's crucial to understand that profiling results may vary due to a multitude of factors, and it's essential to consider these factors when analyzing and interpreting these results.
7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?
  > After analyzing results from performance testing and profiling, I implement several strategies to optimize the application code. These include refactoring the code to make it more efficient, reducing redundancy, and using more efficient data structures and algorithms. For example, the method `joinStudentNames()` was optimized by removing the loop and using Java streams instead. The `stream()` method is used to convert the list of students into a stream. Then, the `map()` function is used to transform each student into their name. Finally, `collect()` is used with `Collectors.joining(", ")` to join all the names into a single string, separated by commas. This approach is more efficient as it leverages the powerful stream API in Java, which is designed to efficiently process data in a declarative way.
