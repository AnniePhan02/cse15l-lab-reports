# Lab Report 4
Hello, today I will be making some edits to my group's implementation of `markdown-parse` and another group's `markdown-parse`.

Here are the link to the repos:
- My group [PantherRepo](https://github.com/AnniePhan02/CSE15L-Panther)
- Other group [OtherRepo](https://github.com/ShashankVenkatramani/markdown-parse/)


## Snippet 1
I believe that it should produce `[url.com, google.com, ucsd.edu]`

Here is how I turned it into a test in `MarkdownParseTest.java`
![Image](lab4.1.png)

### My group's implementation
Here is the output when running the tests. It did not pass as the expected and actual differed. The JUnit test that failed was on line 95.
![Image](lab4.2.png)

### Other group's implementation
Here is the output when running the tests. It did not pass as the expected and actual differed. The JUnit test that failed was on line 91.
![Image](lab4.3.png)


## Snippet 2
I believe that it should produce `[b.com, example.come]`

Here is how I turned it into a test in `MarkdownParseTest.java`
![Image](lab4.4.png)

### My group's implementation
Here is the output when running the tests. It did not pass as the expected and actual differed. The JUnit test that failed was on line 103.
![Image](lab4.5.png)

### Other group's implementation
Here is the output when running the tests. It did not pass as the expected and actual differed. The JUnit test that failed was on line 99.
![Image](lab4.6.png)

## Snippet 3
I believe that it should produce `[https://www.twitter.com, https://ucsd-cse15l-w22.github.io/, https://cse.ucsd.edu/]`

Here is how I turned it into a test in `MarkdownParseTest.java`
![Image](lab4.7.png)

### My group's implementation
Here is the output when running the tests. It did not pass as the expected and actual differed. The JUnit test that failed was on line 111.
![Image](lab4.8.png)

### Other group's implementation
Here is the output when running the tests. It did not pass as the expected and actual differed. The JUnit test that failed was on line 107.
![Image](lab4.9.png)
