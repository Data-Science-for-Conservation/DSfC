
# How to Contribute

Thanks for your interest to contribute to the Data Science for Conservation Project! Please read through the following instructions to get a local version of the project you want to help with set up on your machine and to navigate the pull request (PR) process.

## Software Overview and Prerequisites

- This project uses the version control software Git to track changes - make sure to download a version of it from the [Git website](https://git-scm.com/). Check out the [Pro Git book](https://git-scm.com/book/en/v2) for a Git tutorial
- README.md files are plain text files formatted using standard Markdown syntax. There's a quick tutorial at [commonmark.org](http://commonmark.org/help/tutorial/) for the uninitiated
- Interactive code summaries use [Jupyter Notebooks](https://jupyter.org/)
- Projects use the data science Python stack, which includes `numpy`, `pandas`, `matplotlib`, `seaborn`, and `scikit-learn` among others. One way to install and manage these packages is with the [Anaconda distribution](https://www.anaconda.com/distribution/), which also includes Jupyter Notebooks. You'll need this software to run the notebooks locally.

## Steps to Contribute

1. Create a GitHub account (it’s free!)
2. Fork the project you want to contribute to (see the button in the upper right corner). This will automatically create a copy of this project in your GitHub account
3. In your forked project, click the green "Clone or download" button, then click the "Copy to clipboard" icon next to the link
4. Open a command prompt window and navigate to where you want to save the project files. Then run the following command to copy the project folder to your local machine:

```bash
git clone <paste the copied link from your forked project>

# Example if you forked the Conservation Funding repository
git clone https://github.com/YOUR-GITHUB-USERNAME/ConservationFunding.git
```

5. Add a remote upstream with the following command. This is so Git knows where the original parent repository is located, so you can keep your fork synchronized with it (see section below). You'll need to replace the "REPOSITORY" part with the name of the project you forked:

```bash
git remote add upstream https://github.com/Data-Science-for-Conservation/REPOSITORY.git

# Example to add an upstream for the Conservation Funding repository
git remote add upstream https://github.com/Data-Science-for-Conservation/ConservationFunding.git
```

6. Create a new branch for your work with the command `git checkout -b NEW-BRANCH-NAME`. Try to name your branch in a way that describes your changes, like `fix/addChartLabels`
7. Make your changes, commit them locally (`git add -A` to stage them, then `git commit -m "Text describing your changes"`), and push your new branch to GitHub with the command `git push origin NEW-BRANCH-NAME`
8. Go to your repository on GitHub and look for the green button to open a pull request

## Keep Your Fork Synchronized

Going forward, you’ll want to maintain your local fork so it stays up-to-date with the project repository. This is why you set a remote upstream in step 5 above.

The next time you want to contribute, checkout your local master branch and run the command `git pull --rebase upstream master` before creating a new branch.

This will grab all the changes on the official master branch without making an additional merge commit in your local repository. Then follow steps 6-8 above to open new pull requests to continue contributing!

