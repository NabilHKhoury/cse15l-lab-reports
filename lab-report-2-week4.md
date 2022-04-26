## Lab Report #2 Week 4
Hi, my name is Nabil, in this lab report, I will be displaying the work that I did in the week 3 lab. In lab 3, We created a java file called MarkdownParse that reads another file and prints out all the links in the file. 
This code was given to us and had bugs that we had to identify and resolve. In this lab report, I will review the bugs that I identified from failure-inducing inputs and the symptoms and the fix in code that I made. 
### Bug #1: When there is no openBracket 
The failure inducing input would be ![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(79).png)
The code change to fix it was 
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot78.png)
The sympton is that the bug is that the link that is shown is not the full link, which shows th bug in our program that we did not account for whne this occurs.

### Bug #2: When there is no closeParenthesis
The failure inducing input is ![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(80).png). The symptom is an error message that the index of closeParen is -1. The bug is that we do not take into account the case that there is no closed parenthesis. 

The code change was as descibed below which fixed the output. 
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(81).png)

### Bug #3: When there is no openParenthesis
The failute-inducing input is `[link1]https://something.com)`. The symptom is that openParen is equal to -1 because there is none. The bug is that our porgram does not take into account the case that there is not an open parenthesis. The code change that fixed it was as follows. 
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/Screenshot%20(82).png) 