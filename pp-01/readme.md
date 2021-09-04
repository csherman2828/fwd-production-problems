## ITMD 361, Production Problem 01: Cloning and Committing to a Git Repository

For this production problem, you will learn to fork, clone, commit, and then push and comment on
changes to a remote GitHub repository. Follow the steps below exactly to receive full credit.

1. While logged into your GitHub account in your web browser, point your browser to
   https://github.com/fwd-2021/fwd-production-problems and click the Fork button. You will then
   see that you have forked the Production Problems repository from
   `fwd-2021/fwd-production-problems` into your GitHub account.

   To confirm that you’ve done this correctly, you should see your GitHub account listed on this
   page once you’ve forked: https://github.com/fwd-2021/fwd-production-problems/network/members

2. Once you have forked your own copy of the repository, go to your command line and change to
   whichever directory that you’ve decided you will keep all of your different Git repositories. I
   recommend having in your home directory a `Projects` directory, with subdirectories there for
   each individual project you have under Git control.

   Clone your copy to your computer by clicking Code button on GitHub, and copying either the SSH or
   HTTPS clone address.

   If you choose SSH (preferable), you must have set up your private/public key pair with GitHub.
   See the instructions for setting up SSH keys with GitHub at
   https://help.github.com/articles/connecting-to-github-with-ssh/ You’ll then be able to clone this
   way, using your actual GitHub username where this example says `<USERNAME>`:

     $ git clone git@github.com:<USERNAME>/fwd-production-problems.git

   If you choose HTTPS, you’ll be able to clone the following way, using your actual GitHub username
   where this example says `<USERNAME>`:

     $ git clone https://github.com/USERNAME/fwd-production-problems.git

   The big, annoying difference is that you’ll be prompted for your GitHub password. So strongly
   consider opting to set up your SSH keys like a professional developer.

3. You can now change directories into `fwd-production-problems` and then the `pp-01` directory,
   where you should now have this file, `readme.md`, on your local computer. Open the file in your
   editor, and write below the URL to your fork of the GitHub repository, and the add and commit
   this file:

   My Production Problems repository URL: https://github.com/csherman2828/fwd-production-problems

4. Next, push your commit to GitHub. `git push origin main` from your command line. That is all you
   need to do to submit future Production Problems. **There is no need to open a pull request.** So
   please do not do that.

5. Still on your command line, run the command `git show` with the first 6 digits of your latest
   commit hash. That will look something like `git show ad3bcf`. To figure out your commit hash,
   either look at the message returned when you ran `git commit`, or run `git log -1`.

6. Use your operating system to make screenshot of your command-line window. You **must** use your
   operating system to do this. Don’t go all amateur-hour and snap a photo of your screen with your
   phone. Figure out where it gets saved before you go to the next step.

7. Visit your fork on GitHub, at a URL like `https://github.com/<USERNAME>/fwd-production-problems`.
   Again, use your actual GitHub username, not `<USERNAME>`, in the path to your fork of the
   Production Problems repo. Click the link to your latest commit, which should be the commit you
   just pushed. Scroll to the bottom, and find the comment form. Post as a comment the screenshot
   you took of your terminal window showing your `git show` command and its output.

6. Finallly, and most crucially, back on your command line, you need to add the course’s upstream
   repository as a second remote. From your command line and within the `fwd-production-problems`
   directory, run the command:

     $ git remote add upstream https://github.com/fwd-2021/fwd-production-problems.git

   Once you have done that, you can run the command `git remote -v` and it should list two remotes,
   one called `origin` and one called `upstream`.

   **To receive all future Production Problems, you will change into your `fwd-production-problems`
   directory and run:**

     $ git pull upstream main

7. The instructor will access your Production Problems repository via
   https://github.com/fwd-2021/fwd-production-problems/network/members each week that a Production
   Problem is due; all you need to do to turn in your work is ensure that you’ve pushed your commits
   for each problem to your remote.
