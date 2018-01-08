# Creating a New Repository

To create a new repository, click "Create a project".

![](/assets/7.PNG)

You can create a repository under your **username **or under a **group**. For now just enter a Respository name and a Description under the** Blank project** tab.

![](/assets/6.PNG)

Initializing a new repository will look like this:

\(copy url for project:  [https://gitlab.com/user-name1/test.git\](https://gitlab.com/user-name1/test.git%29\)

![](/assets/8.PNG)

The README file can be created with your project. It's optional and can be added later if necessary. Mostly, if you're creating a new repo you'll want to initialize it with a README.  If you already have a repo you're wanting to upload you can skip this step. The README can be used in various ways, but it will allow you and others to clone the project immediately.

Now that we've setup your **GitLab **account and created a new repository, go to: [http://gitforwindows.org/](http://gitforwindows.org/)  to download and install the **Git Bash. **Then navigate to your project folder through the command prompt or Git Bash and type:

![](/assets/9.PNG)

This will create a hidden directory where Git operates.

Next type:

```
git status
```

![](/assets/10.PNG)

This will show you the status of your repository and also we can use it to verify Git has initialized correctly.

Next save these Git commands to notepad as a text file.

Command line instructions

Git global setup



git config --global user.name "Robert Jakob"

git config --global user.email "rsjakob@outlook.com"



Create a new repository



git clone https://gitlab.com/user-name1/test.git

cd test

touch README.md

git add README.md

git commit -m "add README"

git push -u origin master



Existing folder



cd existing\_folder

git init

git remote add origin https://gitlab.com/user-name1/test.git

git add .

git commit -m "Initial commit"

git push -u origin master



Existing Git repository



cd existing\_repo

git remote rename origin old-origin

git remote add origin https://gitlab.com/user-name1/test.git

git push -u origin --all

git push -u origin --tags




