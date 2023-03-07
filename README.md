# HOW TO HOST A RESUME ON GITHUB 

## PURPOSE:
1. Describe the practical steps to host and format a resume on GitHub Pages.
2. 

## PREREQUISITES:
- A resume formatted in Markdown.
- A web browser.

## INSTRUCTION:

#### STEP 1: Create a Github Account.

If you already had a GitHub account, then you can skip to step 2.

1. Open <https://github.com> in a web browser, and then select `Sign up`.
2. Enter your email address.
3. Create a password, enter your username for your new GitHub account and select `Continue`.
4. Verify your account by solving a puzzle. Select the `Start Puzzle` button to do so, and then follow the prompts.
5. After you verify your account, select the `Create account` button.
6. Next, GitHub send a launch code to your email address. Type that to launch code in the `Enter code` dialog, and then press `Enter`.
7. GitHub asks you some questions to help tailor your experience. Choose the answers that apply to you in the following dialogs.
   - How many team members will be working with you?
   - What specific features are you interested in using?
8. On the Where teams collaborate and ship screen, you can choose whether you want to use the Free account or the Team account. To choose the Free account, select the `Skip personalization` button. GitHub opens a personalized page in your browser.

#### STEP 2: Create a New Repositoty
1. In the upper-right corner of any page, use the `+` drop-down menu, and select `New repository`. 
2. Type a short, memorable name for your repository. For example, "my-resume".
3. Optional, add a description of your repository. For example, "Create my resume with markdown on GitHub".
4. Choose a repository visibility. You will have 3 options: 
   - Public .
   - Internal.
   - Private.

   For more information, see [About repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories#about-repository-visibility).
5. Select `Initialize this repository with a README`.
6. Click `Create repository`.

#### STEP 3: Add a resume file to a repository
1. On GitHub.com, navigate to the main page of the repository.
2. Above the list of files, using the `Add file` drop-down, click `Upload files`.
3. Drag and drop the file or folder you'd like to upload to your repository onto the file tree
4. At the bottom of thep age, type a short, meaningful commit message that describes the change you made to the file. You can attribute the commit to more than one author in the commit message. For more information, see [Creating a commit with multiple authors](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/creating-a-commit-with-multiple-authors)
5. Below the commit message fields, decide whether to add your commit to the current branch or to a new branch. If your current branch is the default branch, you should choose to create a new branch for your commit and then a pull request. For more information, see [Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
6. Click `Commit changes`

#### STEP 4: Rename the resume file.
1. In your repository, browse to the resume file.
2. In the upper right corner of the resume file, click the pen icon button to open the file editor.
3. In the filename field, change the name of the resume to `index.md`. At the same time, you can also update the contents of your resume.
4. This step is similar to the forth step of the previous step.
5. This step is similar to the fifth step of the previous step.
6. Click `Propose file change`.

#### STEP 5: Creating the Configuration File for Jekyll
We'll be utilising Jekyll to create a static site and add a theme to your resume. Jekyll is a static site generator that lets you build websites and blogs by utilising templates to produce the pages from material you write in Markdowwn or HTML. We need to build a _config.yml in order to use Jekyll to construct a static site and apply a theme. From the repository:
1. Click on the `Add file` dropdown button and select `Create new file`
2. A text editor will appear. At the top of it, there is an empty field. Write the name your file as _config.yml
3. In the text editor, copy this code below

```
remote_theme: pages-themes/slate@v0.2.0 # this line adds the slate theme of Jekyll. You can replace "slate@v0.2.0" with your preferred theme.
plugins:
- jekyll-remote-theme # add this line to the plugins list if you already have one
title: "RESUME OF [Your Name]" 
```
4. CLick on the `Commit changes` button at the bottom.

#### STEP 6: Set up GitHub Pages
1. In the repository, navigate to the `Setting` tab.
2. Scroll down to the `Pages` section on the left side of the page
3. Select the `Deploy from a branch` Source and select the main branch with the root folder.
4. Click `Save`

#### STEP 7: Check your GitHub Pages site
1. You could be waited for around 2 minutes for GitHub to build your site
2. Go to <https://username.github.io/repository_name/>, where username is your GitHub username and repository_name is the name of the repository which you created before to upload your resume.
3. You should see your resume display on the site.

### ANIMATED GIF FROM MY RESUME


### MORE RESOURCES
1. [Markdown Tutorial](https://www.markdowntutorial.com/)
2. [Modern Technical Writing: An Introduction to SOftware Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
3. [My resume on GitHub](https://github.com/Luke1401/RESUME_COMP3040)
4. [Jekyll template guide](https://jekyllrb.com/)


## AUTHORS AND ACKNOWLEDGMENT:
This README was created by Hung Lu Dao and reviewed by Ton Nguyen, Sahil Sharma and Nathan Giesbrecht


## FAGs
1. Why is Markdown better than a word processor?
Because there are some reasons below:
- Markdown is simpler: Markdown is a lightweight markup language that uses plain text formatting to create structured documents. It is much simpler than using a word processor, as it requires only a few basic syntax elements
- Markdown is more efficient: When using a word processor, you will often have to spend time formatting your document. With Markdown, you can focus on the content and structure of your document, as the formatting is applied automatically
2. Can I upload multiple files to the same repository at the same time on GitHub?
Yes, you can upload multiple files to the same repository at the same time since you just need to follow the step 3 from INSTRUCTION above and you can drag a whole folder which contain all of your files inside to the repository on GitHub.
