AST326-Practicals Repository
-

Directory organization, per practical:
- `code` contains Python/Jupyter scripts.
- `slides` contains the in-class presentation slides.
- `src` contains all data from the lab handout, as well as practical recorded data.
The name of each subdirectory is the number of the activity corresponding to that data. 
- `tex` can be used to store your LaTeX file and the PDF it makes (if you're using Overleaf you probably won't need 
this at all).
- The root directory of the practical also contains practical notes, and the lab handout.

To use the .ipynb files, drop them into Jupyter and they should work just fine!

For the LaTeX files, I would recommend using [Overleaf](https://www.overleaf.com/home). Create an account/log in, and 
create a new project from .zip - just drop the `report_template.zip` folder into the website, and it should load up!

As far as writing in LaTeX, Overleaf has [a pretty good 
tutorial](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes), although AASTeX might have some specific
things defined too, which you can check out on [the AASTeX v7 guide](https://journals.aas.org/aastexguide/).

Using GitHub
-

The place where we store all these files is the **repository** (aka "repo").

To work on this repository, there's a couple things to do.

The first thing you're going to need is a integrated developing environment (IDE, like VSCode, PyCharm, etc.). 
Follow a tutorial video for the environment you pick. I personally use PyCharm Community because it's made to work well 
with Python scripts.

Then, you'll want to clone the repo to your local device. For this, first open up a terminal, and paste the following:

Windows: <code>git --version</code>

MacOS/Linux: <code>git version</code>

If it doesn't return some sort of version code, check [this tutorial on how to install 
git](https://github.com/git-guides/install-git).

Then, open your IDE, and you should have an option to create a project from **version control**. Select that, and when 
prompted for a link to a repository, enter the following: https://github.com/flypt7/AST326-Practicals.git

All the files should be there once it's done!

Changing stuff on GitHub
-

GitHub has a pretty cool feature that lets you make a copy of the code that will keep one copy witohut changes and
the update the other with your changes. They're called **branches**, and I think it's pretty useful for us to take
advantage of them, since it allows us to all have the data while changing stuff only for ourselves (like when writing
the reports).

To make a branch, open a terminal **within your IDE** and type the following:

<code>git checkout -b your_branch_name</code>

Changing `your_branch_name` to the name you want the branch to have. You can check which branch you are currently in 
with `git branch`. **Make sure that your current branch is not someone else's or the main branch.**

If you need to switch branches, type `git checkout branch_name`, replacing `branch_name` with the name of the branch to 
switch to.

Now it's time to make changes! You can do these directly within the IDE. Once you are done with your changes, you will 
want to update the repository.

Your IDE will definitely have some tab in the sidebar called "Commit" or something similar where you can see what files
you've changed (this is called **staging** the changes). Select them, and type an explanation of the modifications you 
did in the text box below the list of files. Finally, press the "Commit and Push" button.

If you want, all of this can also be done in a terminal! The steps are as follows:

<code>git add file_or_folder</code> replacing `file_or_folder` with the file/folder to add;

<code>git commit -m "your comment here"</code> typing your comment withing the quotes;

<code>git push</code>

Adding is **staging** the changes, a **commit** makes GitHub aware that there's modifications you've made, and 
**pushing** makes these changes on GitHub.

And that's about it! I'm sorry if this isn't super clear, we can have a look at setting up everything next time we see 
each other :)
