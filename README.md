Download link : https://programming.engineering/product/cpe-357-laboratory-exercise-7/

Cpe 357 Laboratory Exercise 7
“…one of the main causes of the fall of the Roman Empire was that, lacking zero, they had no way to indicate successful termination of their C programs.”

    Robert Firth

— /usr/games/fortune

Due by (or before) 11:59pm, Monday, December 4th.

The Laboratory Exercises are to be done individually.

Note: When developing these programs, work on the workstations in the lab or on personal work-stations. A runaway process repeatedly fork()ing can bring a large server to its knees. Your classmates will not love you if you crash unix1 or the other shared machines.

Laboratory Exercises

Programs: fork() and exec() in two lessons

    forkit This program demonstrates the process. forkit starts up, announces itself, then splits into two processes. The child announces itself and exits. The parent identifies itself, waits for the child, then signs oﬀ. All this is shown in Figure 1.

                    	
                    	
                    	
                    	
                    	
                    	
                    	

    tryit takes a command-line argument of the path to a program (absolute or relative), forks a child that tries to exec() the given program, and reports on its success or failure. A child that exits with a status of 0 is assumed to be a success, non-zero is a failure. If the exec() fails, the child should print why (via perror()), and exit with a non-zero status.

This program does not have to support command line arguments to the other program. That will be part of Asgn 7’s shell.

The process is shown in Figure 2.

                	
                	
                	
                	
                	
                	
                	
                	
                	
                	
                	

    The ps command (/bin/ps) will show you processes belonging to you. Be sure you know how to use it so you can clean up after yourself.

What to turn in

For the Laboratory Exercises: Submit via handin in the CSL, to the lab07 directory, your two programs, forkit.c and tryit.c

A makefile (called Makefile) that will build your programs when given either the target “all”.

A README file that contains:

    Your name(s). In addition to your names, please include your Cal Poly login names with it, in parentheses. E.g. (pnico)

    Any special instructions for running your program.

    Any other thing you want me to know while I am grading it.

The README file should be plain text, i.e, not a Word document, and should be named “README”, all capitals with no extension.
Solution
