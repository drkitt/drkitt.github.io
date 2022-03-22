# Hosting a Markdown resume on GitHub Pages

## Purpose

This tutorial will show you how to host your resume online using Markdown with GitHub Pages.

## Prerequisites

- A resume formatted in Markdown
  - Don't worry if you don't have one yet! There are some resume guidelines and Markdown tips in the More Resources section below.
  - Make sure that the file is named `index.md`, in order to have GitHub Pages recognize it.
- A GitHub account

## Instructions

1. Log in to GitHub.
1. Navigate to your profile. On desktop, you can access it by clicking on your profile picture in the top right of the screen and clicking on **Your profile**. On mobile, you'll instead need to click on the hamburger menu icon in the lop left of the screen and click on your username.
1. On your profile, click on the **Repositories** tab.
1. Click the green **New** button.
1. Name the repository `<your username>.github.io`. For example, my GitHub username is `drkitt`, so my repository is named `drkitt.github.io`.
1. Click the green **Create repository** button. You can mess around with the other fields if you want, but they're all optional. Just make sure the repository is set to **Public** and not **Private**.
1. Now that you have a repository, you can add a file. On desktop, click on the **Add file** button (which is next to the green **Code** button) and click **Upload files**. On mobile, the process is similar, but the first button to press is labeled **...** instead; once you've found it, click on it and then click **Upload files**.
1. Click on the link that says **choose your files** and use your system's file browser to upload your Markdown resume.
1. Click the green **Commit changes** button to add the resume to your repository. Feel free to add a message to your commit if there's any other information you think you might need to refer back to later, but the default message should suffice.
1. Your resume is now in your your repository, but there are a couple more things you must configure before it's ready. Click on the **Settings** button, which should be at the end of the row of buttons near the top of the page (labeled **Code**, **Issues**, **Pull requests**, etc.). If it isn't there, click on the three dots at the end of that row and the **Settings** button will appear.
1. On the repository settings, access settings specific to GitHub Pages by clicking on the **Pages** button on the left side of the page.
1. Under *Source*, select the `main` branch to ensure that the file you just uploaded gets displayed on the final page.
1. Under *Theme Chooser*, click the **Choose a theme** button and look through the available themes. Once you've found one that you like, click the green **Select theme** button.
1. Your resume is ready to go! Navigate to `<your username>.github.io` in your web browser to see it. Note that it might take up to 20 minutes for GitHub Pages to apply your changes, so if anything isn't working you can just check back later.

## More Resources

- If you've never used Markdown before, check out [the markdowntutorial.com tutorial](https://www.markdowntutorial.com/).
- If you've used Markdown before but you want a refresher, you can use [the markdownguide.org cheat sheet](https://www.markdownguide.org/cheat-sheet).
- There are lots of Markdown editors out there. I recommend using [Visual Studio Code](https://code.visualstudio.com/) with the [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) extension.
- For help creating your resume, see the [University of Manitoba Career Services resume workbook](https://umanitoba.ca/career-services/sites/career-services/files/2021-05/Online_Resume_Book.pdf). You can also find more general information on the [Career Services website](https://umanitoba.ca/career-services/).

## Authors and Acknowledgements

- Written by Alex Kitt for COMP 3040 at the University of Manitoba
- Peer editing by Group 1

## FAQs

**Markdown? Why can't I use something like MS Word?**

A big strength of Markdown, which this tutorial takes advantage of, is its versatility. It's possible to apply a variety of themes to a Markdown document and switch between them easily because Markdown documents don't store any styling information within the document itself. In contrast, Word documents have styling coupled with content, so making sweeping changes to one is a manual, error-prone process.

**Why is my github.io page giving me a 404??**

There are a few different things you need to configure correctly in order to make your resume show up. Make sure of the following:

- You spelled your username correctly, in both the repository name and the URL.
- Your repository is public. Free accounts are unable to use GitHub Pages with private repositories.

- You configured the site to build from the same branch as the one you're adding files to.
- You chose a Jekyll theme.

GitHub Pages can take up to 20 minutes to apply your changes, so if everything seems to be set up correctly but the page still doesn't show up, it may suffice to just try again later.
