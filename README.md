## Create a GitHub account

1. Log into GitHub with your own GitHub account.  _(Create one if you don't have one.)_

## Note that you do not yet have a web page

1. Visit the following website URL in your web browser and note that it doesn't exist on the internet yet -- there's just a placeholder announcing a "404" error:
    * Take the phrase "`https://your-username.github.io/`" and replace "`your-username`" with your actual GitHub username.
    * So, if your GitHub username is `awesomecoder`, you'll want to visit the web page "**`https://awesomecoder.github.io/`**" instead of "`https://your-username.github.io/`".

## Create a copy of this codebase into a "Git repository" of your own that has a copy of it hosted on GitHub.com under your account

1. ["Fork" the original codebase by visiting this link](https://github.com/kkgthb/web-site-jekyll-04-github-pages/fork) -- but when you get there, make SURE you change the value the "Repository name" prompt from "**`web-site-jekyll-04-github-pages`**" to a value matching the following pattern instead:
    * Take the phrase "`your-username.github.io`" and replace "`your-username`" with your actual GitHub username.  _(It's the value in the "Owner" picklist just to the left of the "Repository name" prompt.)_
    * So, if your GitHub username is `awesomecoder`, you'll want to write "**`awesomecoder.github.io`**" instead of "`your-username.github.io`".
    ![Github documentation screenshot of repository naming](https://docs.github.com/assets/cb-34195/images/help/pages/create-repository-name-pages.png)
1. Click the "Create fork" button once you've changed the repository name as indicated above.

## Tell GitHub that you would like to host a webpage based on the code in your new Git repository

1. Under your repository name, click Settings _(the gear-shaped icon)_.
    ![GitHub documentation screenshot of the settings icon](https://docs.github.com/assets/cb-27528/images/help/repository/repo-actions-settings.png)
1. In the "Code and automation" section of the left sidebar, click "**Pages**."
1. Under "Build and deployment" at right, under "Source", select "`Deploy from a branch`."
1. Under "Build and deployment", under "Branch", change the value of the picklist reading "`None`" to say "`main`" instead.
    ![GitHub documentation screenshot of the branch picklist](https://docs.github.com/assets/cb-70869/images/help/pages/publishing-source-drop-down.png)
1. Under "Build and deployment", under "Branch", click the **Save** button.
1. Visit the following website URL in your web browser _(it might take up to 5-10 minutes)_ and note that now it _does_ exist on the internet, congratulating you on having become a newly-minted CI/CD expert:
    * Take the phrase "`https://your-username.github.io/`" and replace "`your-username`" with your actual GitHub username.
    * So, if your GitHub username is `awesomecoder`, you'll want to visit the web page "**`https://awesomecoder.github.io/`**" instead of "`https://your-username.github.io/`".
1. Pat yourself on the back.  You've just used modern DevOps-oriented tooling to put a web page on the internet based on a little bit of code.

## Edit your website with Git

Now let's play with changing the way that website looks by editing the code and "committing" your codebase changes into the codebase hosted online at GitHub.com _(and known as a "Git repository")_ that you created when you made a "fork" from the original sample codebase.

### Edit and save a change to the codebase

1. Visit the following website URL in your web browser to open a place _(known as an "IDE")_ where you can edit the "`index.md`" file buried within the codebase:
    * Take the phrase "`https://github.dev/your-username/your-username.github.io/blob/main/pages/index.md`" and replace "`your-username`" with your actual GitHub username.
    * So, if your GitHub username is `awesomecoder`, you'll want to visit the web page "**`https://github.dev/awesomecoder/awesomecoder.github.io/blob/main/pages/index.md`**" instead of "`https://github.dev/your-username/your-username.github.io`/blob/main/pages/index.md".
1. In the right-hand pane of the website, you should see a file-editing interface with a tab at the top labeled "`index.md`" whose body contains the following _(if you don't see it within a minute, close the browser tab and try again -- sometimes the system hangs a bit)_:
    ```md
    ---
    permalink: /index.html
    title: Tiny Jekyll web site home page
    layout: fancy_announcement
    ---

    Hello, world
    ```
1. Toward the bottom of that file, delete the word "`world`" from the phrase "`Hello, world`" and type your own name in its place.  Within a few seconds of the moment that you stop typing, this web site will auto-save your work as if you had clicked "File -> Save" in a desktop text editor _(much like Google Docs auto-saves your work when you pause typing)_.
1. In a new web browser tab, visit the following website URL in your web browser and note that it still says "Hello, world" and does not yet contain your name:
    * Take the phrase "`https://raw.github.com/your-username/your-username.github.io/main/pages/index.md`" and replace "`your-username`" with your actual GitHub username.
    * So, if your GitHub username is `awesomecoder`, you'll want to visit the web page "**`https://raw.github.com/awesomecoder/awesomecoder.github.io/main/pages/index.md`**" instead of "`https://raw.github.com/your-username/your-username.github.io/main/pages/index.md`".

### Mark your change important by "committing" it and "push" it onto GitHub.com

1. In the far-left-side vertical strip of navigation icons, click the slightly-"`Y`"-shaped icon just below the magnifying glass icon, which now has a blue number "`1`" in a circle superimposed over it.  When you hover over the icon you need to click, it will be labeled labeled "**Source Control**."
    ![GitHub official screenshot of the Source Control view in the Codespaces Activity Bar](https://docs.github.com/assets/cb-59829/images/help/codespaces/source-control-activity-bar-button.png)
1. The 2nd-from-the-left-hand pane will fill in with contents titled "**Source Control**".
1. Toward the top of that pane, in a box labeled "**Message**," type the phrase "`My first edit`".
1. Click in the blank gray space below that box to make the blue message floating below it go away.
1. Below that box, under "**Changes**," hover over "`index.md`" until icons appear to the right of it.  Click the icon that looks like a "`+`" _(plus sign)_ and that, when you hover over it, is labeled "**Stage Changes**."  You should see "`index.md`" move out of "**Changes**" and upward into a new section called "**Staged Changes**."
1. Up at the top of the "**Source Control**" panel, click its 3rd icon -- the checkmark icon that, when you hover over it, is labeled "**Commit and Push**."
1. If you struggled through any of this, the official GitHub Codespaces documentation has some screenshots of what it looks like to do this at "[The github.dev web-based editor -> Commit your changes](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor#commit-your-changes)."
1. Pat yourself on the back -- you have just used an IDE to edit code, and then used Git's "commit" functionality to comment upon important changes to the codebase's history and Git's "push" functionality to upload those changes to the copy of your "Git repository" that's hosted on GitHub.com.
1. In a new web browser tab, visit the following website URL in your web browser and note that your codebase _**does**_ say your name now:
    * Take the phrase "`https://raw.github.com/your-username/your-username.github.io/main/pages/index.md`" and replace "`your-username`" with your actual GitHub username.
    * So, if your GitHub username is `awesomecoder`, you'll want to visit the web page "**`https://raw.github.com/awesomecoder/awesomecoder.github.io/main/pages/index.md`**" instead of "`https://raw.github.com/your-username/your-username.github.io/main/pages/index.md`".

### Admire that editing your codebase changed your website

1. Visit the following website URL in your web browser and reload it _(it might take up to 5 minutes)_ and note that to the right of the megaphone icon, instead of saying "`Hello, world`," the website greets you by name:
    * Take the phrase "`https://github.dev/your-username/your-username.github.io`" and replace "`your-username`" with your actual GitHub username.
    * So, if your GitHub username is `awesomecoder`, you'll want to visit the web page "**`https://github.dev/awesomecoder/awesomecoder.github.io`**" instead of "`https://github.dev/your-username/your-username.github.io`".
1. Pat yourself on the back.  You've just edited a live website by contributing edits _(via the Git protocol)_ to a codebase that's connected to the website via "CI/CD" tooling.

## Troubleshooting

If it's taking more than 5 minutes for your website to appear on the internet after you "commit and push" a change _(or after you first set up your "repository" to be connected with "GitHub Pages" in the first place)_, you might be able to get some visibility into what's going wrong at [https://github.com/your-username/your-username.github.io/actions/workflows/pages/pages-build-deployment](https://github.com/your-username/your-username.github.io/actions/workflows/pages/pages-build-deployment) _(work you've done flips to having green checkboxes to the left of it as it completes its work going live onto the internet, in the main panel under a count of "workflow runs")_ and at [https://github.com/your-username/your-username.github.io/deployments](https://github.com/your-username/your-username.github.io/deployments) _(work you've done appears under "Deployment History" each time a website update fully finishes going live onto the internet -- with "commit numbers" associated to each effort, and your "commit" history can be seen at [https://github.com/your-username/your-username.github.io/commits/main](https://github.com/stackbittest/stackbittest.github.io/commits/main))_.  Replace "`your-username`" as appropriate in all 3 of these links, of course.

[https://www.githubstatus.com/](https://www.githubstatus.com/) is also a great resource that will let you know if something's broken with GitHub Pages altogether -- those outages can take hours or days to get fully resolved, but should eventually self-heal.

Also, don't forget that none of this works if you don't name your repository correctly when you fork it.  [Delete your repository off of GitHub.com](https://docs.github.com/en/repositories/creating-and-managing-repositories/deleting-a-repository) and start over if you made a typo.