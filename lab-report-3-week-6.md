# Lab Report 3 (Week 6)

## Group Choice Options 1 - 3

### Task 1. Streamlining ssh Configuration
- Show your `.ssh/config` file, and how you edited it (with VScode, another program, etc)
![ssh-config](./lab-report-3-images/ssh-config.png) 
![config-vscode](./lab-report-3-images/config-vscode.png)
- Show the `ssh` command logging you into your account using just the alias you chose. Command: `ssh ieng6`
![ssh-fast-login](./lab-report-3-images/ssh-fast-login.png)
- Show an `scp` command copying a file to your account using just the alias you chose. Command: `scp filename ieng6:~/`
![scp-fast](./lab-report-3-images/scp-fast.png)

### Task 2 Setup Github Access from ieng6

- Show where the public key you made is stored on Github and in your user account (screenshot).
![ssh-keys-github](./lab-report-3-images//ssh-keys-github.png)
![ssh-keys-account](./lab-report-3-images/ssh-keys-account.png)
- Show where the private key you made is stored on your user account (but not its contents) as a screenshot.
![ssh-private-account](./lab-report-3-images/ssh-private-account.png)
- Show running git commands to commit and push a change to Github while logged into your ieng6 account.
![git-account](./lab-report-3-images/git-account.png)
- Show a link for the resulting commit. [https://github.com/kevinhuang-ucsd/lab-report3-task2/commit/6fc60b09d934b06b2d7491478077afa3e3a7b06e](https://github.com/kevinhuang-ucsd/lab-report3-task2/commit/6fc60b09d934b06b2d7491478077afa3e3a7b06e)

### Task 3: Copy whole directories with `scp -r`

- Show copying your whole markdown-parse directory to your ieng6 account.
Command: `scp -r markdown-parse ieng6:~/`
![copy-dir-0](./lab-report-3-images/copy-dir-0.png)
![copy-dir-1](./lab-report-3-images/copy-dir-1.png)
![copy-dir-2](./lab-report-3-images/copy-dir-2.png)

- Show logging into your ieng6 account after doing this and compiling and running the tests for your repository.
![test-account](./lab-report-3-images/test-account.png)

- Show (like in the last step of the first lab) combining `scp`, `;`, and `ssh` to copy the whole directory and run the tests in one line.
Command: `scp -r markdown-parser ieng6:~/; ssh ieng6 "cd markdown-parser/; javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java; java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest"`
![combined-commands](./lab-report-3-images/combined-commands.png)
Result:
![combined-result](./lab-report-3-images//combined-result.png)