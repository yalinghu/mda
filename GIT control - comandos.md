**GIT control - comandos** 

from KATAKODA

<u>Scenario1. Committing files</u> 

- Initialized empty git repository  ```git init```

- View the change btw working directory / what´s been previously committed to the repository   ```git status```

- Add file hello-world.js to the staging area   ```git add hello-world.js```

-  Commit the file to the repository    ```git commit -m "commit message"```

- Add and commit a *.gitignore* file to the repository to ignore all *.tmp files  

  ```echo '*.tmp' > .gitignore```

  - we should commit it to garuantee the rules apply across different machines



<u>Scenario2. Committing changes</u>

- Compare changes in the working directory against a previously commited version  ```git diff```

- Load the external tool to view the differences (visualize the difference btw two versions) ```git difftool```

- Compare changes in the staging area  ```git diff --staged```

- View gthe history of the repository and the commit log  ```git log``` <span style='color:green;background:pink;'>该命令用于显示提交日志信息, EXAMPLES：</span>

  - ```git log --no-merge``` Show the entire commit history, but skip the merge

  - ```git log --since="2 weeks ago" --gitk```  Show the changed file gitk in the last two weeks. "--" is necessary to avoid confusion with the branch named gitk

  - ```git log -3``` The three most recent submissions will be displayed

  - ```git log --author=yaling``` Query the submission record of the specified author (Yaling)

- Display one or more objects ```git show```

  





Git command explaintion in CHINESE 🀄️ 【https://www.yiibai.com/git/git_config.html】





