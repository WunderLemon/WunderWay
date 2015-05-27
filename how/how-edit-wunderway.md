---
layout: page
section: how
categories:
tags:
title: How To Edit The WunderWay
---

The WunderWay is intended to be collaborative and continuously improved. Any change or addition can be suggestion by anyone, and requires peer review before being merged into the official WunderWay.

To help with this, we use Github's [pull request workflow.](https://help.github.com/articles/using-pull-requests/) This allows us to keep all the different versions of the content that have ever existed, track changes, and discuss them. It also allows us easily catch and fi any mistakes, so don't worry about breaking it.

## Preparing To Work On The WunderWay

## Preparing To Work On The WunderWay
1. You'll need a user account at [Github](https://github.com), which is the service that hosts the version control system for us.

## Editing The WunderWay On Github
You can simply work on the Github website, without needing to set up anything on your own computer:

1. Go to the [WunderWay repository](https://github.com/Wunderkraut/WunderWay)
2. Navigate to the page you want to edit, clicking on the folders until you find the filename you want. Click on that. For example, this page can be edited at https://github.com/Wunderkraut/WunderWay/blob/gh-pages/how/how-edit-wunderway.md
3. Click Edit. Make the changes you want.
4. At the bottom of the screen, in the 'Propose Changes' section, add a description of the changes you've made.
5. Click the 'Propose Changes' button.
6. Your pull request will appear on the WunderWay [pull requests page.](https://github.com/wunderkraut/WunderWay/pulls)
7. A notification of this pull request will appear in the WunderCafe Hipchat room. Reach out to specific people to ensure they see your pull request.

## Editing The WunderWay On Your Local Computer using the Github app
1. Download and install the [Github for Mac](https://mac.github.com/) software.
2. Download and install a text editor of your choice. eg. [Sublime Text](http://www.sublimetext.com/)
3. Open the Github app and, on the repositories screen, select 'Wunderkraut' repositories.
4. On the 'Wunderkraut/WunderWay' repository select 'Clone to Computer'
5. Select a suitable folder to save the files in.
6. Open your text editor. From the File menu choose 'Open...'. Select the folder where you cloned the WunderWay repository.
7. In Sublime and similar text editors, you'll see the folder structure of the WunderWay on the left hand side. Find the file you want to edit, and make the changes. Select File>Save when you are done.
8. In the Github for Mac application, under 'changes' it will show that you have 'uncommitted changes'. Type a heading and description about the changes you made. Click Commit.
9. You can make many edits like this offline. When you are back online and want to open a pull request for your changes you follow the instructions on [Create Pull Requests with GitHub for Mac](https://github.com/blog/1946-create-pull-requests-with-github-for-mac) ![Demonstration of a pull request](https://cloud.githubusercontent.com/assets/13760/5697198/35b8c866-999f-11e4-91c1-7af538f2ced5.gif)
10. Your pull request will appear on the WunderWay [pull requests page.](https://github.com/wunderkraut/WunderWay/pulls)
11. A notification of this pull request will appear in the WunderCafe Hipchat room. Reach out to specific people to ensure they see your pull request.

## Reviewing and merging pull requests
For instructions on how to review and discuss the proposed changes see [Using pull requests.](https://help.github.com/articles/using-pull-requests/#reviewing-proposed-changes)

After a consensus has been agreed, and you have the permissions, you'll want to merge the pull request into the officla WunderWay. For instructions on how to merge and close a pull request see [Merging a pull request.](https://help.github.com/articles/merging-a-pull-request/)

## Previewing your WunderWay changes on your local computer
1. Navigate to the top WunderWay folder in your terminal
2. Install Jekyll by running ``` $ gem install jekyll ```
3. You you encounter an error, you may need to run ``` $ sudo gem install jekyll ```
4. In the same directory, run ``` jekyll serve ```. This compiles the jekyll site and makes it availiable on http://localhost:4000
5. If you want Jekyll to recompile the site every time you save a file, run ``` jekyll serve --watch ``` instead

## Formatting
The WunderWay uses a formatting syntax called 'Markdown' to generate the content. It's simple to use once the basic syntax is learned. You can read Github's [Introduction to Markdown](https://guides.github.com/features/mastering-markdown/) and you can find a full description on the syntax at http://daringfireball.net/projects/markdown/syntax

## Creating New Pages
If you need to create a completely new page, you can create a new file in the right section folder in WunderWay. Call the file 'your-file-name.md' where your-file-name can be anything you like. The '.md' file extension is important.

At the very beginning of your file you need a few lines of text called 'front-matter'. These look like this, and you can copy and paste this as a template to start with and edit as you need...

    ---
    layout: page
    section: how
    categories: Admin
    tags: Expenses, Finance
    title: How To Claim Expenses
    ---

This tells the system that builds the site what type of file it is, what section it's in, the categories it's in, and the title. The Tags will help with navigation.
