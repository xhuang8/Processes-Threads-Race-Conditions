Name  : XiaoQian Huang
Date  : 3/27/2018
Class : CSC 415

Compile Instructions: This project lets us create a group of threads and then try to coax them into
producing as many race conditions as possible. After finishing the code, we should open the terminal
and run the command. Then, we can know something wrong on our project. The command should be£º
gcc pthread_race.c -o race


Run Instructions: The coding should run under the GCC enviroment. I use the CodeBlocks to finish it. 
Then, I can successfully run the project, and the output also like the forms which showed on slack. If 
we run on the linux envirnment. We should type: ./race. There was going to appear the output as following:
Hello, I am thread #0
Hello, I am thread #1
Hello, I am thread #4
Hello, I am thread #7
Hello, I am thread #9
Hello, I am thread #2
Hello, I am thread #5
Hello, I am thread #6
Hello, I am thread #8
Hello, I am thread #3
I am thread #6   read value            : 0
I am thread #0   read value            : 0
I am thread #5   read value            : 0
I am thread #2   read value            : 0
I am thread #3   read value            : 0
I am thread #9   read value            : 0
I am thread #7   read value            : 0
I am thread #4   read value            : 0
I am thread #1   read value            : 0
I am thread #8   read value            : 0
I am thread #8   added 10 value is now : 10
I am thread #6   added 10 value is now : 10
I am thread #4   added 10 value is now : 10
I am thread #1   added 10 value is now : 10
I am thread #7   added 10 value is now : 10
I am thread #9   added 10 value is now : 10
I am thread #3   added 10 value is now : 10
I am thread #2   added 10 value is now : 10
I am thread #5   added 10 value is now : 10
I am thread #0   added 10 value is now : 10
Final Global Value : 10


Project Description: On this project, we should have 10 threads, and each of which increases the
shared variable by 10. Waiting for all the threads to complete and then prints out the final value
of the global counter. We should pay attention each thread should initially fprintf out stderr a 
"hello I'm thread #x." After we finish the coding, we should inplement the
code using Pthreads on Linux. The output shows on last instruction.
