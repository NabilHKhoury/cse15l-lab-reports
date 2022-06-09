# Lab Report Five 
Now that the quarter has come to a close, I want to thank whoever has been grading these. I am sorry you have had to go through my lab reports, and thank you that you did. 
### Finding the Bugs
To find the bugs I updated the bash script and ran it. I moved the outputs repositorto a seperate file that I called `results.txt` by using `>` command. After this, I needed to compare the reults. Therefore I used the command `diff` to check the diferences. I got many errors; however, for this la I chose to work with the bug in `22.md` and `516.md`. \
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/screenshots/Screenshot%20(124).png) \
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/screenshots/Screenshot%20(125).png).
The link to these tests is 
[516.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/516.md)
and [22.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/22.md).
For the `22.md` test, my repository the output was `[/bar\* "ti\*tle"]` and the shared repositories output was `[]`.  
For the `516.md` test, my repositories output was `[moon.jpg, /uri]` and for the shared repository it was `[moon.jpg]`. 
### Which Implemented Correctly?
For the `22.md` test it is clear that my repository was correct as the file return the link, which was the desired output. However, the shared repository got it incorrect.
For the `516.md` test, my output was incorrect as it included both links in 2 seperate parenthesis, while the shared doc did not make this error and only included the `moon.jpg` link in the parenthesis. 
(I came to these conclusions by previewing the files). \
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/screenshots/Screenshot%20(126).png)
\
![Image](https://nabilhkhoury.github.io/cse15l-lab-reports/screenshots/Screenshot%20(127).png)
### How to fix bugs
For the `22.md` test we do not have to fix any bugs; however, we have to for the `516.md` test. 
The bug for the `516.md` case is that it includes both links in the non-nested double parenthesis. So to fix this we need to take this case into account.
For the `516.md` test, we can add an if statement that takes into account the case in which there is 2 parethesis that are not nested. In this case, we can then excluse the second parentehsis to get the correct answer. 