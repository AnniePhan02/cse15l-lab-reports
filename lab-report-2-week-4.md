# Lab Report 2
Hello, this lab report covers week 3 and 4. We worked on debugging, symptoms, and failure-inducing inputs. 

Here are the GitHub repos for week 3 and week 4. 

[Week3Repo](https://github.com/AnniePhan02/markdown-parse)

[Week4Repo](https://github.com/AnniePhan02/CSE15L-Panther.git 
)



## 1) First Code Change -
In our code, we found a bug that does not print all of the link needed. It does not take in account if there is something between the last closing bracket and opening parenthesis.

Screenshot history of us fixing this bug. 
![Image](CommitFix1.png)

Link to test file for failure-inducing input. [testincorrect.md](https://github.com/AnniePhan02/markdown-parse/blob/main/testincorrect.md)

Symptom of the bug was found when running the command line and the expected was different from actual. The expected was `[]` and the actual was `[)]`. Here is the output of running the file at the command line. 
![Image](CommitFix1Error.png)

Between the bug, symptom, and failure-inducing input, the disagreement between our expected value showed a symptom. The failure inducing-input in `testincorrect.md` showed a symptom of the wrong output. When retracing code, this happened because the indexing was wrong and the program did not account for if there was anything in between a closed bracket and open parenthesis. 

## 2) Second Code Change
After changing our code, we found another bug that did not consider if there were parentheses and brackets in the link title.

Screenshot history of us fixing this bug. 
![Image](CommitFix2.png)

Link to test file for failure-inducing input.
[test2incorrect.md](https://github.com/AnniePhan02/markdown-parse/blob/81c112bf22e6c653d32236ba8aef395d98f6e29f/test2incorrect.md)


Symptom of the bug was found when running the command line and the expected was different from actual. The expected was `some-page.html` and the actual was `[r l(]`. Here is the output of running the file at the command line. 
![Image](CommitFix2Error.png)

Write 2-3 sentences describing the relationship between the bug, the symptom, and the failure-inducing input.

Between the bug, symptom, and failure-inducing input, the expected and actual output differed which illustrates a symptom. When code-tracing, the bug was that the program did not consider if there are parentheses and brackets in the link title. The failure-inducing input showed the symptom of the unexpected input of `[r l(]`, which was that bug. 



## 3) Final Code Change - 
We found another bug that considers an input with spaces to be a link. In markdown, a link cannot have spaces in between. For example in the statement to the right, links cannot have spaces. [##](this is an example link)

Here is a screenshot history of us fixing this bug. 
![Image](CommitHistory3.png)

Link to test file for failure-inducing input: [file-8.md](https://github.com/AnniePhan02/CSE15L-Panther/blob/main/test-file8.md)

Symptom of the bug was found when running the JUnit test. Here is the output of running the file at the command line. 
![Image](JUnitTest8.png)


Between the bug, symptom, and failure-inducing input, the bug is that the the expected was an empty list which is `[]`, but the actual was `[a list on the first line]`. This is an example of a symptom that shows a bug because the symptom shows disagreement between the actual and expected. The bug is that the code takes in account the spaces in between the words, which is not right for a link. Similarly, the failure-inducing input is the input where it has spaces in between the link. 