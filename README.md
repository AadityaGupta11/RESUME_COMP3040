# HOW TO HOST A RESUME ON GITHUB 

## PURPOSE:
1. Describe the practical steps to host and format a resume on GitHub Pages.
2. Guide the audience to create a github account and host their Markdown file from Github with a theme to style their file from Jekyll

## PREREQUISITES:
- A resume formatted in Markdown.
- A web browser.
- A stable Internet Connection

## INSTRUCTION:

#### STEP 1: Create a Github Account.

If you already had a GitHub account, then you can skip to step 2.

1. Open <https://github.com> in a web browser, and then select `Sign up`.
2. Enter your email address.
3. Create a password, enter your username for your new GitHub account and select `Continue`.
4. Verify your account by solving a puzzle. Select the `Start Puzzle` button to do so, and then follow the prompts.
5. After you verify your account, select the `Create account` button.
6. Next, GitHub send a launch code to your email address. Type that to launch code in the `Enter code` dialog, and then press `Enter`.
7. On the Where teams collaborate and ship screen, you can choose whether you want to use the Free account or the Team account. And then, GitHub opens a personalized page in your browser.

#### STEP 2: Create a New Repositoty
1. In the upper-right corner of any page, use the `+` drop-down menu, and select `New repository`. 
2. Type a short, memorable name for your repository. For example, "my-resume".
3. Choose a repository visibility. You will have 3 options: 
   - Public .
   - Internal.
   - Private.
4. Select `Initialize this repository with a README`.
5. Click `Create repository`.

#### STEP 3: Add a resume file to a repository
1. On GitHub.com, navigate to the main page of the repository.
2. Above the list of files, using the `Add file` drop-down, click `Upload files`.
3. Drag and drop the file or folder you'd like to upload to your repository onto the file tree
4. At the bottom of thep age, type a short, meaningful commit message that describes the change you made to the file. 
5. Below the commit message fields, decide whether to add your commit to the current branch or to a new branch. If your current branch is the default branch, you should choose to create a new branch for your commit and then a pull request. 
6. Click `Commit changes`

#### STEP 4: Rename the resume file.
1. In your repository, browse to the resume file.
2. In the upper right corner of the resume file, click the pen icon button to open the file editor.
3. In the filename field, change the name of the resume to `index.md`. At the same time, you can also update the contents of your resume.
4. This step is similar to the forth step of the previous step.
5. This step is similar to the fifth step of the previous step.
6. Click `Propose file change`.

#### STEP 5: Creating the Configuration File for Jekyll
We need to build a _config.yml in order to use Jekyll to construct a static site and apply a theme. From the repository:
1. Click on the `Add file` dropdown button and select `Create new file`
2. A text editor will appear. At the top of it, there is an empty field. Write the name your file as _config.yml
3. In the text editor, copy this code below

```
remote_theme: the theme name
plugins:
- jekyll-remote-theme # add this line to the plugins list 
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
3. [Jekyll template guide](https://jekyllrb.com/)


## AUTHORS AND ACKNOWLEDGMENT:
This README was created by Hung Lu Dao and reviewed by Ton Nguyen, Sahil Sharma and Nathan Giesbrecht


## FAGs
1. Why is Markdown better than a word processor?
Because there are some reasons below:
- Markdown is much simpler than using a word processor, as it requires only a few basic syntax elements
- With Markdown, you can focus on the content and structure of your document, as the formatting is applied automatically
2. Can I upload multiple files to the same repository at the same time on GitHub?
- Yes, you can upload multiple files to the same repository at the same time since you just need to follow the step 3 from INSTRUCTION above and you can drag a whole folder to the repository on GitHub.

<br>
<br>
<br>


# PRINCIPLES OF CURRENT TECHNICAL WRITING FROM ANDREW ETTER'S BOOK 

## PURPOSE
- Relate the practical steps described above to the general principle of current Technical Writing, as explained in Andrew Etter's book Modern Technical Writing

## PREREQUISITES
- The Andrew Etter's book from any version: physical book or pdf version, ...
- Read over the book and have a general understanding of Modern Technical Writing

## RELATION TO BOOK
1. Using a lightweight markup language.
- The aim and significance of employing lightweight markup languages (LMLs) in technical writing are discussed in Andrew Etter's book "Modern Technical Writing". LMLs are a kind of markup language created to be simple to read and write while still being extremely malleable and changeable 
- Using LMLs in technical writing mostly serves to boost output and effectiveness. Technical writers don't have to worry as much about formatting and layout because LMLs are straightforward and simple to master. This can help you save a lot of time and work.
2. Format a doucment using a static site generator.
- To format documents using Jekyll, a static site generator that may be used with a distributed version control system (DVCS).
- There are various pre-built themes in Jekyll that you can use to format your documentation. By changing the theme field in your "_config.yml" file, you can select a theme according to the instructions above. If you'd rather, you could also design your own unique theme.
3. Share/host documents on a distributed version control system (DVCS).
- You can use version control to track changes made to your document over time by employing a DVCS. To keep track of changes, commit your changes frequently and use informative commit notes. By step 6 above, we were already hosting our resume on the platform GitHub, a version control system. Our resume may be shared with others, created, and managed more effectively by hosting it on GitHub.
