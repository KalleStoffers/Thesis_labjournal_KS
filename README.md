# Lab Journal

A [lab journal](https://jochemtolsma.github.io/labjournal/) template for students following the course Social Networks. Naturally this template can also be used for other courses using RStudio and Git. To use this template, follow the steps below.

## Preparation:

1.  Make sure [R](https://cran.r-project.org/index.html), [R-studio](https://posit.co/downloads/) and [Git](https://git-scm.com/downloads) are installed;

2.  Make sure the `rmarkdown`-package is installed in R-studio (with "install dependencies");

    ```{r}
    install.packages("rmarkdown", dependencies = TRUE) 
    ```
3.  If you do not have a GitHub account, create one;

4.  Optional: install [GitHub Desktop](https://desktop.github.com).

5.  Connect Git, GitHub, RStudio (we will use the package `usethis` for this):

    ```{r}
    install.packages("usethis") 
    library("usethis")
    #use your username and email of your GitHub account
    use_git_config(user.name = "Your Name", user.email = "yourmail@example.org") 
    create_github_token() #save token in passwordmanager system
    gitcreds::gitcreds_set() #self explanatory I hope
    ```

## Fork the original labjournal repository:

1.  Fork this repository using the fork button in the top right hand corner of Github, to make a personal copy of this lab journal;

2.  Go to your own GitHub account and under your repository name, navigate to 'Settings'; click on 'Pages' on the sidebar; select the main-branch as your publishing source, and serve from the 'docs'-folder:

![](images/pages.png)

You now have a personal copy of this repository on your account, which serves html files (aka Github pages) as a website. Put the link of your lab journal in your own readme file and if you go back to your repository on GitHub, change the '*About*' section and make sure to add the link to your website.

## Inviting collaborators:

Once again, go back to your repository on Github. Navigate to '*Settings*'; click on '*Collaborators*', and invite the lectures of your course (e.g. JochemTolsma). After acceptance, the lecturers have access to you repository and can make contributions. This is not strictly necessary because the lectures can also clone your repository, file issues and make pull requests. But learning how to effectively collaborate via Git is somewhat beyond the scope of this course.

## Clone the repository:

In RStudio go to '*File', 'New Project', 'Version Control', 'Git'.* I create all my projects as subdirectory of "C:\\Github".

## Journal your work:

1.  Open your repository/project in RStudio ('*File', 'Open Project')*. Alternately, you can navigate to the repository at your local path and open the 'labjournal.Rproj' file. This should automatically open R-studio, and your current working environment will be inside this project.
2.  Inside R-studio you should see a files tab in the bottom right hand corner;
3.  Customize the 'index.Rmd' as you wish within R-studio, to make it your own;
4.  Make sure to install the `remotes` and `klippy` packages. Commands are included in the index.Rmd.
5.  Journal your work using .Rmd-files.

You can keep your personal notes and working scripts a separate folder. Make sure to include an underscore in the folder name (e.g., \_test). Scripts contained in this folder will not be compiled.

## Hosting on Github:

1.  Recompile the lab journal website using the Build function in the top right hand corner (if you do not see this '*Build*' tab, you may need to restart RStudio);
2.  Go the '*Git*' tab, commit your changes and push them to GitHub. Alternatively, you could use Git from the command line (open the '*Terminal'* window) or you could use [GitHub Desktop](https://desktop.github.com/download/). Whatever works best for you.
3.  Your personal lab journal website will be published at: <https://%7BUSERNAME%7D.github.io/bigssslabjournal/>

## Useful resources:

1.  Working with [Git](https://git-scm.com/book/en/v2), [Happy Git with R](https://happygitwithr.com/index.html) and [GitHub Desktop](https://docs.github.com/en/desktop)
2.  Getting the hang of R Markdown: [The Definitive Guide](https://bookdown.org/yihui/rmarkdown/) and [Cookbook](https://bookdown.org/yihui/rmarkdown-cookbook/)
