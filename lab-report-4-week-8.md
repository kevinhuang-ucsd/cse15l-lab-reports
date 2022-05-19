# Lab Report 4 (Week 8)

## A link to your markdown-parse repository and a link to the one you reviewed in week 7
- my markdown-parse repo: [https://github.com/kevinhuang-ucsd/markdown-parser](https://github.com/kevinhuang-ucsd/markdown-parser)
- reviewed: [https://github.com/mrreganwang/markdown-parser](https://github.com/mrreganwang/markdown-parser)

## For Each Test

### Snippet 1
- should produce: ```[`google.com, google.com, ucsd.edu]```
- turned into code: ![my-test0](./lab-report-4-images/my-test0.png)
- output for my implementation: ![my-output0](./lab-report-4-images/my-output0.png)
- output for the other implementation: ![his-output0](./lab-report-4-images/his-output0.png)

### Snippet 2
- should produce: `[a.com, a.com(()), example.com]`
- turned into code: ![my-test1](./lab-report-4-images/my-test1.png)
- output for my implementation: ![my-output1](./lab-report-4-images/my-output1.png)
- output for the other implementation: ![his-output1](./lab-report-4-images/his-output1.png)

### Snippet 3
- should produce: `[https://www.twitter.com, https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule, https://cse.ucsd.edu/]`
- turned into code: ![my-test2](./lab-report-4-images/my-test2.png)
- output for my implementation: ![my-output2](./lab-report-4-images/my-output2.png)
- output for the other implementation: ![his-output2](./lab-report-4-images/his-output2.png)

## Answering Questions
- Yes. I could add two if conditions: If there's a backtick before an open bracket, continue the loop (ignore the following link, which is invalid). If there's a backtick after a close bracket, ignore the close bracket and keep searching for a valid close bracket.

- Yes. I could add two if conditions: If there's a backslash before an open bracket, ignore this open bracket. If there's a backslash before a close bracket, ignore this close bracket.

- No. I believe in order to deal with the index out of bounds error, I'll have to change the while loop somehow to prevent going out of bounds, which is defintely longer than 10 lines.