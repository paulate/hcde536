# HCDE 536 Interaction Design and Prototyping Spring 2026

This is an example repository for HCDE 536 students who want to host their work as a website using GitHub Pages. This is one approach — not the only one. You're welcome to present your work however makes sense to you, like exporting a document or Figma file as a PDF. This tutorial is here if you want a lightweight, customizable portfolio site.

Student: [Your Name]

## What is Git? What is Github?

**Git** is a version control software that tracks changes to your files over time. It runs on your computer.

**GitHub** is a website that hosts Git repositories online and adds collaboration features. Think of it as a combination of:

- **Cloud storage** for your code (like Google Drive, but for code)
- **Version control** that tracks every change you make (like "Track Changes" in Word, but much more powerful)
- **Collaboration tools** that let multiple people work on the same project

### Some useful Git & Github terms

- **Repository (repo)**: A folder that contains your project files and the history of all changes made to them
- **Clone**: Download a copy of a repository to your computer so you can work on it
- **Commit**: Save a snapshot of your changes with a descriptive message (like saving a version of your work)
- **Push**: Upload your committed changes from your computer to GitHub's servers
- **GitHub Pages**: A free feature that turns your repository into a live website (e.g. yourusername.github.io/hcde536)

## Getting Started

This tutorial covers:

- Installing Git and VS Code
- Creating a GitHub account and forking this repository
- Optionally setting up GitHub Pages to publish your site
- Making your first changes

If you run into any issues, ask questions on Canvas or bring them to class.

## Git Installation

[Make a Github account](https://github.com/) and
[install Github Desktop](https://desktop.github.com/). This should install git,
but in past classes some people using MacOS ran into an issue where git did not
install correctly. If you are having issues with git, try following
[this guide](https://github.com/git-guides/install-git) for your operating
system.

## Clone this example repository

If you are experienced with git and Github and comfortable using the command line, you may do these steps using git commands. If not, follow the instructions below for using Github Desktop.

Once you have Github Desktop installed, you can clone this example repository
to your computer. In Github Desktop, go to `File > Clone Repository...`, then
select the `URL` tab. Copy and paste the URL of this repository into the box and click "Clone".

At the bottom of the Github Desktop window in the repository, it should say "You don't have write access to this repository. Want to create a fork?". Click "create a fork" and select "for my own purposes" when prompted. (You are essentially creating your own copy of this repository that you can make changes to freely, without affecting the original repository.)

### Optional but recommended: Set up a global .gitignore file

When using git, there are certain files you generally do not want to commit to
your repository. For example, on MacOS, `.DS_Store` files are automatically
created by the operating system to store folder view options. These files are
not useful to include in your repository.

If you see a file you do not want to commit showing up in your list of changes, left click on it and select "Ignore file". This will create a `.gitignore` file in your repository that tells git to ignore those files in the future. [Read more about ignoring files.](https://help.github.com/en/github/using-git/ignoring-files).

## VS Code Installation

Visual Studio Code (VS Code) is a good free editor for working with HTML and CSS. VS Code is
a _highly extensible_ text editor. This means that its base function is quite
simple: you can open and edit files. You can install extensions via the
extension marketplace, which let you add bits of functionality as you need them,
such as support for different languages.

[Download and install Visual Studio Code.](https://code.visualstudio.com/).

If you have a different editor preference (e.g., Sublime), you are welcome to
use it.

Once you have installed VS Code, sign in with your Github account.

Install the following extensions from the extension marketplace:

- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) — lets you preview your site locally as you edit
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) — auto-formats your code

## Your first commit and push

Open the repository you cloned earlier in VS Code: in Github Desktop, right click on the repository name in the left sidebar and select "Open in Visual Studio Code". Alternatively, you can open VS Code first and open the folder
by going to `File > Open Folder...` and
selecting the folder where you cloned the repository.

Open the `README.md` file in VS Code. Change `Student: [Your Name]` to your actual name and save the file.

There are two common ways to commit and push your changes to Github:

### Option 1: Using Github Desktop

Go back to Github Desktop. You should see that the `README.md` file shows up
in the list of changes. Enter a commit message (e.g., "First commit: added my name") and click the "Commit to main" button. Finally, click the "Push origin" button at the top to push your changes to Github's servers. If you go to the repository page on Github in your web browser, you should see your changes reflected there.

### Option 2: Using VS Code Source Control

1. Open the "Source control" panel in VS Code's left sidebar. You should see a
   list of changes you have made.
2. Hover over the header that says "Changes". You should see a Plus icon (+)
   appear to the right. Click it to stage your changes.
3. Enter a commit message (e.g. "First commit: added my name") in the text entry
   box above (which should say "message"), and click the "Commit" button.
4. The "Commit" button should turn into a button that says "sync changes" —
   click it. This will push your work to Github.
5. If you go to the repository page on Github in your web browser, you should see your changes reflected there.

## Github Pages Setup

If you want to publish your site publicly, GitHub Pages is a free way to do it. Anything in the `docs` folder of your repo will be available as a live website.

To enable it: go to your GitHub repo in your web browser, click the **Settings** tab, then **Pages** in the left sidebar. Under "Source", select **main** as the branch and **/docs** as the folder. Click **Save**. Your site will be published at `yourusername.github.io/hcde536` after a few minutes.

Every time you push changes to GitHub, your site will automatically update.

## Customizing your site

The `docs` folder contains a starter `index.html` and template pages you can edit. Here's how to preview and customize them.

In VS Code, right click on `index.html` (in the `docs` folder) in the explorer sidebar and click "Open with Live Server". The page should open automatically in your browser. You can now edit the files and your changes will update in the browser immediately — a good way to preview your work before publishing.

Start by reading through `docs/index.html` and understanding how each part corresponds to what you see in your browser. Then:

- Edit the page to include your name and 1–2 sentences about yourself
- Replace the placeholder image with a photo of yourself (or an avatar)

When you are done, commit and push your changes to publish your site.

### File size limitations

[Github limits file uploads](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github) to 25mb, so if you're showing video or photo larger than 25mb, you'll have to either downsize or host it elsewhere (e.g. youtube, vimeo, wikimedia) and embed it or link to it.

### Web resources

The MDN Web Docs are a fantastic resource:

- [HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)
- [CSS Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics)
- [Creating hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)
- [Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)
- [CSS Layout](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Introduction)

#### Acknowledgments:

- Machine Agency's HCDE 439 github repo
- AI used to generate some content, reviewed by instructor
