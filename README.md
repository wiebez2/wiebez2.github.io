
# Hosting on GitHub Pages

## Purpose
You will learn the steps needed to host your own site using GitHub pages and Markdown. Additionally, you will have a grasp on static-site generators and the benefits to using Markdown.

## Summary
- [Prerequisites](#prerequisites)
- [Instructions](#instructions)
    - [Make a Repository](#1-make-a-repository)
    - [Cloning a Repository](#2-cloning-a-repository)
    - [Adding to a Repository](#3-adding-to-a-repository)
    - [Launching your Website](#4-launching-your-website)
- [More Resources](#more-resources)
- [Authors and Acknowledgements](#acknowledgments)
- [FAQ](#faq)

## Prerequisites 
 - Resume formatted in Markdown.
 - Signed in GitHub account.
 - Access to command line.

 ## Instructions
These instructions show you the process to host your own site on GitHub. GitHub's own instruction list can be found [here](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages).

### 1. Make a Repository

Upon signing into GitHub, you will be on GitHubs's landing page where you can create a new repository. Here, focus on the box with the title "Start a new repository for `[your username]`"

1. Write `[your username].github.io` as the name of your repository, in the textbox.
    * It's essential that you enter your username prior to `.github.io`
2. Select the **Public** option.

3. Click the green **Create new repository** button.

### 2. Cloning a Repository

 - In your command line, run the following:
    ```
    git clone https://github.com/[your username]/[your username].github.io
    ```
    * in your local files, you will now have a copy of the online repository.


Git is used because of its robust capabilities in managing file versions (version control). Essentially, this entails the ability to store and manage files in an online repository such as GitHub. Moreover, Git monitors the history of these files and records the changes made to them. Andrew Etter emphasizes the significance of version control for technical writers, highlighting that Git handles this aspect seamlessly. He further notes Git's advantages in ensuring documentation and code branches remain aligned and encouraging developer contributions. Overall, Git simplifies collaborative work on a project while preserving a record of previous iterations. 


### 3. Adding to a Repository
1. Create an `index.md` file in the **local** repository.
    - This is really just the contents of your resume but under the name *index*, and of Markdown format.

2. Push `index.md` from your local repository to your online repository.

    - In the command line, run the following:
    ```
    git add [address of index.md]
    git commit -m "Added index.md"
    git push -u origin master
    ```

Again, it is imperative that your resume be named `index.md`. Your hosted site won't run without a file named "index," of Markdown format which has the contents that you want displayed. GitHub automatically looks at the contents of your repository and looks for files with specific names of specific type in order to do things with them.
 - README.md is automatically displayed in the repository's home screen.
 - _config.yml is used to add cosmetic functionality to your website.
 - index.md is displayed in the front page of your website.
    

Markdown shines among other markup languages as it is widely embraced for its simplicity, readability, and cost-free nature. Due to these qualities, Etter notes his preference of Markdown over strictly using XML. Because of their lightweight characteristics, Markdown and similar markup languages are popular for publishing content to webpages. With respect to this guide, Static-site generators and Markdown files facilitate creation of a resume-hosting website quite easily.


### 4. Launching your Website
 - In a browser, go to `https://[your username].github.io`.

Etter suggests that making a website like the one described in this README is an easy way to share lots of different kinds of information. Static websites, like this one, are quick and simple to set up because they don't need a lot of extra stuff and don't rely heavily on other technologies. They provide a basic setup that's good enough to make a website look nice. Plus, they make it easy for people to access documents. Instead of having to send PDFs through email or by mail, static websites let anyone, anywhere, get to the documents whenever they want.

## More Resources
Some extra reading which go in detail on relevant topics.

 - [What is Markdown?](https://www.markdownguide.org/getting-started/#what-is-markdown)

 - [Getting Started With GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages)

 - For a deeper understanding of subject matter, [Andrew Etter's _Modern Technical Writing: An Introduction to Software Documentation_](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)

 - [Jekyll Tutorial](https://cloudcannon.com/tutorials/jekyll-tutorial/)
 

## Acknowledgments 
 - Thank you for the peer editing done by the  members of Stuart Little; Shaun Cheriyan, and Aswin Manoj.
 - Instruction set takes inspiration from Andrew Etter's _Modern Technical Writing: An Introduction to Software Documentation_.
 - This repository uses the [Time Machine theme](https://github.com/pages-themes/time-machine).

## FAQ

_Why would I use Markdown over a word processor?_

 - You use Markdown over a word processor for a various reasons, mostly to do with conveniency.
   -  **Simplicity**: Markdown is incredibly lightweight and easy to learn. It makes use of simple syntax which allows you to write and edit without much complexity.
   - **Portability**: Markdown files are generally plain text files, this means that you can open and edit them in any text editor.
   - **Integration**: Platforms like GitHub, or blogs have fully adopted Markdown. Consequently, this makes it easy to write content that can seamlessly be integrated into websites and other web-based applications.

_Why am I getting a 404 error when trying to host a website on GitHub?_

 - 404 errors when hosting a website on GitHub *usually* have to do with incorrect settings of a file or directory.
   - **Repository Name**: Double check that the repository is named correctly. For GitHub Pages, the repository must be named in the format `<username>.github.io` where `<username>` is your GitHub username.
   - **Bad File/Directory Structure**: GitHub Pages expects certain files to be present in your repository to serve your website correctly. Make sure you have an index.html file in the root directory of your repository.
   - **Incorrect Settings Configuration**: Make sure that your repository settings are set to ensure that GitHub Pages is enabled and configured correctly. You can find this in the settings tab of your repository.

