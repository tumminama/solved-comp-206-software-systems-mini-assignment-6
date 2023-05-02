Download Link: https://assignmentchef.com/product/solved-comp-206-software-systems-mini-assignment-6
<br>
Fork() and the Producer-Consumer Problem




This assignment explores malloc, makefile, modular programming, git, fork() and shell memory.




In class we saw examples of how to write producer-consumer algorithms using fork() and we saw a critical section implementation using shell memory.  For this assignment you will work with one other person to solve a variation of the producer and consumer problem.




Both of you will submit the same solution algorithm to myCourses.




Do the following:

<ul>

 <li>Team work

  <ul>

   <li>Divide the work between the two of you. o Each of you will have their own private git. We will not implement a shared git.</li>

   <li>You will share your code using email once it is good and the other team member will add your good code to their git. Your git needs to show these transactions for you to get points for working together.</li>

  </ul></li>

 <li>Implementation o c will implement the distribution of work.

  <ul>

   <li>It contains only the main() function</li>

   <li>It will fork the producer and consumer o c will implement the producer algorithm</li>

   <li>It contains only the forked producer() function</li>

   <li>Producer reads one character at a time from a text file named mydata.txt.</li>

  </ul></li>

</ul>

You can populate that file with any information you like.

<ul>

 <li>c will implement the consumer algorithm

  <ul>

   <li>It contains only the forked consumer() function</li>

   <li>Consumer displays to the screen all the characters it receives from the producer. The output must be in the same format (it should look the same) as the file when displayed to the screen.</li>

  </ul></li>

 <li>Inter-process communication o Shell variable TURN and DATA will be used to communicate between producer and consumer. Producer will have TURN number 0 and consumer will have TURN number 1. They will use the TURN .txt  in order to take turns accessing the DATA.txt.     Main() initializes the TURN.txt to 0 before it launches the clones.

  <ul>

   <li>The DATA.txt contains the  single character producer wants to give to consumer. Producer assigns a character to DATA then gives the TURN to the consumer. The consumer extracts the value from DATA and gives the TURN back to the producer.</li>

   <li>This continues until the producer is done. Then the programs must terminate.</li>

  </ul></li>

</ul>





