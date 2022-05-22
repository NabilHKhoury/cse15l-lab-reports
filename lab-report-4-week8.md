# Lab Report 4
In this lab report, I am using my `MarkdownParseTest.java` and another persons file to test three Snippets of code. Due to my grandmother passing away, I did not attend Lab 7. Therefore, I did not do the work on someone else, so I decided to do this on `nidhidhamnani` or the repository that I originally forked. To be clear, I did it on the updated version of the file that we cloned in Lab 8. 
## Snippet 1
I put the first Snippet of tests in a file called Snippet1.md. Here is what it looks like. \
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(110).png).\
The test I created is the following. \
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(109).png())\
In my `MarkdownParseTest.java` file, the result was the following. \
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(115).png).\
In the other file, the result was the following .\
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(113).png).\
As we can see, both programs failed for the first Snippet test or Snippet1Test(). In order to fix this, for my program, we would need to take into account the fact that a link could begin with `, but it is not part of the link. We could fix this by using an if statement to take this into account. For the other program, wewould need to do the same thing as they had the same output. 
## Snippet 2
I put the second Snippet of tests in a file called Snippet2.md. Here is what it looks like. \
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(111).png).\
The test I created is the following. 
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(109).png).\
In my `MarkdownParseTest.java` file, the result was the following. \
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(115).png).\
In the other file, the result was the following .\
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(113).png).\
As we can clearly see, there is a problem in both programs. For my program it did not take into account the first test at all becuase it was a nested link so the program did a.com as the otput when it should have been b.com. For the next link, becuase there was multiple closing parenthesis nested in the loop it ended early. For the last link everything was as expected. To fix these problems, we have to take into account that when a program has a nested link we should not end until the actual link is finished. We can do this by using an if statement for this case and then telling the program to go to the actual starting point of the link for the first paren. For the second link, we can take into account that when the paren is nested also with multiple we need to take into account the fact that we need them both the close, so we can use if statement to ensure that this case is covered. 
 In the other program, the first link had the same problem as mine, but the second link worked, and the third link did not work at all and the program brooke out of the while loop before it did it. To fix this, we need to take into account the same fix for the first link as my program, and for the thrid link we need to figure out what caused the break from the while loop and add in a case to prevent this from before all the links have gone through.
## Snippet 3
I put the third Snippet of tests in a file called Snippet3.md. Here is what it looks like. \
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(112).png).\
The test I created is the following. 
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(109).png).\
In my `MarkdownParseTest.java` file, the result was the following. \
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(115).png).\
In the other file, the result was the following .\
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(113).png).\
If there was a problem this is how to fix it. 
As we can see in the file, the error in my program was the second to last link or the github.com link because there was text after the link and before the last paren and there was no last paren, so the link included the last link within it also. To fix this, we need to take into account when there is no last close paren, and that we should end on the .com or .org or.edu. Then this will fix this case and the program for other cases as well. 
For the other program, there was an inde out of bouds exception because there was no close paren. This is becuase they did not have a case to continue the program when this exception occurs as mine did. So I would add this case in as my program has, and also add in the fix that my program needed for this program of adding the case with an if statement for ending with the .com or .edu or.org. 
