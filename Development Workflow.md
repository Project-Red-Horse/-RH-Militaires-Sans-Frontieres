I've created four branches - three of which are **dev,** **testing,** and **master.**

All development activity will be done on dev.
Once we decide development on a feature is complete, we will move it to test, and test it there.

Master will be linked to Steam, meaning **anything put to master will automatically be served to Steam.**
This means that we only push to master from testing once we're sure everything is good.

In the event that we were wrong, I created a 4th branch: **hotfix**
If something went wrong with Master, we can fix it on hotfix and merge it directly onto master.



To summarize, for every new code change...

dev -> test -> Master
Make it in Dev, test it in test, finalize it in master.

If something goes wrong...

hotfix -> Master



GIT REMINDER:

The basic unit of work in Git is known as a commit. A commit acts as a sort of "save point." Like save points, you can return to any commit at any time.

Unlike save points, however, git commits save only what you want them to save; they're NOT all-or-nothing. Use "git add FILE" to specify what exactly should be saved with your next commit. In most cases, we don't care, so use "git add *." This tells Git that you want ALL files in the folder to be saved.

Then, use "git commit -m MESSAGE" to save your commit. To then share your commits with the Github website, type "git push origin/dev," which will push your changes to our dev branch.

**ALWAYS USE "GIT PULL" BEFORE RESUMING WORK.**
"git pull" is the opposite of "git push": if push sends your changes to the Github, pull delivers our changes to you. Pull and push synchronize the copy of the project on the website with the one on your computer, so that we're all on the same page.

All git projects are stored as a bunch of different branches. Each branch is a sequence of commits tracing all the way back to the first commit. Every time you commit with git commit, you move your current branch forward by one commit.

Use "git checkout BRANCH" to switch branches.

Until you get the hang of mastering Git, leave the remote stuff, like merging, to us. Contact us when you've finished developing or testing, and we'll move your work into the master branch for you.
This is our workflow. I've tried to keep this simple, but if you've any further comments, suggestions, or concerns, direct them to me(reuy).