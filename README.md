# Hosting a Markdown Resume on GitHub Pages

## Purpose

This tutorial will show you how to host your resume online using Markdown with GitHub Pages. Along the way, it'll demonstrate some of the principles for technical writing and documentation that can be found in the book *Modern Technical Writing* by Andrew Etter.

## Prerequisites

- A resume formatted in Markdown
  - Don't worry if you don't have one yet! There are some resume guidelines and Markdown tips in the More Resources section below.
  - Make sure that the file is named `index.md`, in order to have GitHub Pages recognize it.
- A GitHub account

## Instructions

#### Making a repository

Etter's book recommends using a distributed version control system (DVCS) to track changes and collaborate. As explained in his book, technical writers should put documentation in the same repository as code in order to keep documentation and code in sync and allow developers to contribute to documentation. Etter further explains that developers generally prefer DVCS for their performance, ability to work offline, and ability to work concurrently on individual files, and thus technical writers should use it too. For this tutorial, we'll use the popular GitHub DVCS.

1. Log in to GitHub.

2. Navigate to your profile. On a large screen, you can access it by clicking on your profile picture in the top right of the screen and clicking on **Your profile**. On a small screen, you'll instead need to click on the hamburger menu icon in the lop left of the screen and click on your username.

![New repository demo](New%20repository%20demo.gif)

3. On your profile, click on the **Repositories** tab.

4. Click the green **New** button.

5. Name the repository `<your username>.github.io`. For example, my GitHub username is `drkitt`, so my repository is named `drkitt.github.io`.

6. Click the green **Create repository** button. You can mess around with the other fields if you want, but they're all optional. Just make sure the repository is set to **Public** and not **Private**.

#### Adding files

7. Now that you have a repository, you can add a file. On a large screen, click on the **Add file** button (which is next to the green **Code** button) and click **Upload files**. On a small screen, the process is similar, but the first button to press is labeled **...** instead; once you've found it, click on it and then click **Upload files**.

![Upload file demo](Upload%20file%20demo.gif)

8. Click on the link that says **choose your files**.

9. Use your system's file browser to upload your Markdown resume.

10. Click the green **Commit changes** button to add the resume to your repository. Feel free to add a message to your commit if there's any other information you think you might need to refer back to later, but the default message should suffice.

#### Configuring the static site

Etter's book praises static websites. Since they don't require databases, server-side logic, or any of the other complications of dynamic websites, they're fast, portable and don't require a sophisticated server setup. These qualities make them ideal for hosting documentation. Etter goes on to recommend using a static site generator, rather than creating the static site yourself, because the generator will take care of tedious tasks like writing HTML and CSS yourself. For this tutorial, we'll leverage GitHub Pages' built-in support for Jekyll, the most popular static site generator.

10. Your resume is now in your your repository, but there are a couple more things you must configure before it's ready. Click on the **Settings** button, which should be at the end of the row of buttons near the top of the page (labeled **Code**, **Issues**, **Pull requests**, etc.). If it isn't there, click on the three dots at the end of that row and the **Settings** button will appear.

![Settings demo](Settings%20demo.gif)

11. On the repository settings, access settings specific to GitHub Pages by clicking on the **Pages** button on the left side of the page.

12. Under *Source*, select the `main` branch to ensure that the file you just uploaded gets displayed on the final page.

13. Under *Theme Chooser*, click the **Choose a theme** button and look through the available themes. Once you've found one that you like, click the green **Select theme** button.

#### That's all!

Your resume is ready to go! Navigate to `<your username>.github.io` in your web browser to see it. Note that it might take up to 20 minutes for GitHub Pages to apply your changes, so if anything isn't working you can just check back later.

## More Resources

- If you've never used Markdown before, check out [the markdowntutorial.com tutorial](https://www.markdowntutorial.com/).
- If you've used Markdown before but you want a refresher, you can use [the markdownguide.org cheat sheet](https://www.markdownguide.org/cheat-sheet).
- There are lots of Markdown editors out there. I recommend using [Visual Studio Code](https://code.visualstudio.com/) with the [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) extension.
- For help creating your resume, see the [University of Manitoba Career Services resume workbook](https://umanitoba.ca/career-services/sites/career-services/files/2021-05/Online_Resume_Book.pdf). You can also find more general information on the [Career Services website](https://umanitoba.ca/career-services/).

## Authors and Acknowledgements

- Written by Alex Kitt for COMP 3040 at the University of Manitoba
- Peer editing by Group 1 (Jarett Koley, Daniel Makarchuk, Nitya Seth, and James Watts)
- [Slate theme by Jason Costello](http://jekyllthemes.org/themes/slate/) used for resume

## FAQs

**Markdown? Why can't I use something like MS Word?**

Markdown is a popular markup language. Markup languages, as Etter's book argues, are excellent for documentation because they're fit for publishing on the web, which is integral for keeping documentation up to date for all of its users. In particular, markup documents convert seamlessly to HTML, work well with version control, and have a convenient separation of content and style that makes it easy to set and change the documentation's appearance.

In contrast, Word documents have poor support for publishing on the web, as they have limited HTML export capabilities, use a binary format that doesn't work well with version control, and couple content and style together that makes design changes a manual, error-prone process.

Markdown is the most popular markup language in the world, and its simple syntax makes it easy to learn, hence its use here.

**Why is my github.io page giving me a 404?**

There are a few different things you need to configure correctly in order to make your resume show up. Make sure of the following:

- You spelled your username correctly, in both the repository name and the URL.
- Your repository is public. Free accounts are unable to use GitHub Pages with private repositories.

- You configured the site to build from the same branch as the one you're adding files to.
- You chose a Jekyll theme.

GitHub Pages can take up to 20 minutes to apply your changes, so if everything seems to be set up correctly but the page still doesn't show up, it may suffice to just try again later.
