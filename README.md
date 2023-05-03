Download Link: https://assignmentchef.com/product/solved-cs342-homework-3
<br>
Q1. Write a C program that will define a global integer array of size 1000 and will initialize it with random values. Then it will create 3 threads. Threads will run concurrently. The first thread will find the average, the second thread will find the minimum, and the third thread will find the maximum value in the array. The main thread will then print these 3 values out.

Q2. Consider the following structure definition.

struct student {

int id;               char name[64];            char lastname[64];  int age;            double cgpa;

};

Write a producer program and a consumer program. You will use shared memory  to pass student information from the producer to the consumer for 3 students. You can set the values for the students to anything you like. You will use POSIX shared memory API. Learn more about it by typing “man shm_overview” at Linux command line.




Note that if <em>shmptr</em> is a variable pointing to some location in the shared memory, then you can put (write) student information into that location as below.  You can use a similar approach for getting (reading) the information.




struct student *sp;

sp = (struct student *) shmptr;




sp-&gt;id = 1045;  strcpy (sp-&gt;name, “Ali”);  ….




Q3. Assume for a program, the fraction of the program that must run serially is 0.25. What is the maximum speed up that we can achieve for that program if we use 8 processors (8 threads)? What is the limit?




Q4. Consider the following 5 processes and their arrival and CPU times.




<table width="433">

 <tbody>

  <tr>

   <td width="54"> </td>

   <td width="142">Arrival time</td>

   <td width="236">CPU time (CPU burst length)</td>

  </tr>

  <tr>

   <td width="54">A</td>

   <td width="142">0</td>

   <td width="236">50</td>

  </tr>

  <tr>

   <td width="54">B</td>

   <td width="142">15</td>

   <td width="236">80</td>

  </tr>

 </tbody>

</table>

1

<table width="433">

 <tbody>

  <tr>

   <td width="54">C</td>

   <td width="142">35</td>

   <td width="236">40</td>

  </tr>

  <tr>

   <td width="54">D</td>

   <td width="142">55</td>

   <td width="236">20</td>

  </tr>

  <tr>

   <td width="54">E</td>

   <td width="142">65</td>

   <td width="236">50</td>

  </tr>

 </tbody>

</table>




<em>Assume that in case of a tie, a process with lower ID enters the ready-queue first. A has lower ID than B, for example.  </em>




For each of the following scheduling algorithms, find out the finish time and total waiting time in the ready queue for each process.




<ol>

 <li>RR scheduling with q = 30 ms.</li>

 <li>RR scheduling with q = 10 ms.</li>

 <li>RR scheduling with q = very very small (much smaller than 1, i.e., close to 0; perfect sharing). d) SRJF.</li>

 <li>e) FCFS.</li>

</ol>




Q5. Assume initial estimation is 20 ms for bursts of a process. What would be the estimate after 3 bursts of lengths 24, 18, and 30, assuming alpha = 0.4.





