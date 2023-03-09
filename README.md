# READ(*L*)ME *This,* <sub><sup>*How does one host a resume using GitHub-Pages?*</sub></sup> 🤨

![GIF](/readmeAssets/resumeV2.gif)

## Contents Table 📂
- [Prerequisites](#prerequisites-)
- [Steps](#steps-)
  1. [Software Installation](#1-software-installation)
  2. [Setting up GitHub-Pages](#2-setting-up-github-pages)
  3. [Setting-Up Local Repository](#3-setting-up-local-repository)
  4. [Create Default Files With Git Bash](#4-create-default-files-with-git-bash)
  5. [Test Site](#5-test-site)
  6. [Adding Resume](#6-adding-resume)
  7. [Modify _config.yml](#7-modify-_configyml)
  8. [Modify Gemfile](#8-modify-gemfile)
  9. [Push To Main](#9-push-to-main)
  10. [Lets See The Result!](#10-lets-see-the-result)
- [More Resources](#more-resources-)
- [Credits](#contents-table-)
- [FAQ](#faq-)


## Prerequisites ❗
- Prior to starting this tutorial __you should__ already have a resume that is in Markdown format. If you don't have one I recommend checking out the *Markdown Tutorial* in the [More Resources](#more-resources-). 

---
# Steps 👣

## 1. Software Installation
 1. Download [GitHub Desktop](https://desktop.github.com/)
 2. Download [Ruby](https://www.ruby-lang.org/en/)
 3. Download [Visual Studio Code](https://code.visualstudio.com/)
 

## 2. Setting-Up GitHub-Pages
<sup>*Note:* using a Distributed Version Control System (Like GitHub) is a great way to *share* and *host* your files. You can learn more on page 28 of [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title).

  1. Navigate to your repositories (github.com/__*yourUsername*__?tab=repositories).
  2. Click on the green button that says __New__.
  
![Image](/readmeAssets/GitHubNewRepo.png)

  3. Type *yourUsername.github.io* into the text box lablled *Repository name*.
  4. Check-off the box lablled *Add a README file*.
  5. Click the green button lablled __Create repository__.

## 3. Setting-Up Local Repository
  1. Navigate to your newly created repository (github.com/__*yourUsername*__/__*yourUsername*__.github.io).
  2. Click on the green button that says __Code__.
  3. Click __Open with GitHub Desk__ -- (__Note:__ a popup may arise, if so, just click *Open GitHubDesktop.exe*) .
  4. Click the blue button lablled __*Clone*__ once the GitHub Desktop application opens up -- (__Note:__ keep track of the *Local path* you are cloning to. This will be required in an upcoming step).

## 4. Create Default Files With Git Bash
  1. Open the *Git Bash* terminal.
  2. Navigate to the *Local path* where your repository was cloned. This is an example of how to navigate files in a terminal with the cd command, ```cd 'C:\Users\yourAccount\Documents\GitHub\yourUsername.github.io'```.
  3. Type the command ```gem install jekyll bundler```.


## 5. Test Site
<sup>*Note:* Setting up a Static Site Generator (What we completed in the prior step) is one of the best things you can do to save time for future you! With a properly configured Static Site Generator you'll be able to pass it brand new Markdown files and have it automatically generate a delightful site. If you're interested in knowing more I recommend reading pages 31 to 33 of [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title).

  1. Open the *Git Bash* terminal.
  2. Navigate to the *Local path* where your repository was cloned. This is an example of how to navigate files in a terminal with the cd command, ```cd 'C:\Users\yourAccount\Documents\GitHub\yourUsername.github.io'```.
  3. Type the command ```bundle exec jekyll serve```.
  4. Wait till the terminal says ```Server running... press ctrl-c to stop.```
  5. Type http://localhost:4000/ into your browser.
  6. Once the page is loaded you should see your site.
  7. Close the site by pressing *ctrl-c*, followed by *Y* and the *enter* key in the Git Bash terminal.


## 6. Adding Resume
  1. Open GitHub Desktop.
  2. Press __Ctrl__+__Shift__+__A__ (Visual Studio Code should open).
  3. Open index.markdown, found under the EXPLORER tab (Note: If you don't see the EXPLORER tab press __Ctrl__+__B__).
  4. Paste your pre-existing resume into the index.markdown file.
  5. Save the file.


## 7. Modify _config.yml
  1. Open _config.yml.
  2. Comment-out every line. (Note: To comment-out a line place  ```#``` at the start).
  3. Add the following  
     - ```remote_theme: pages-themes/slate@v0.2.0```
     - ```plugins: ```  
     - ```  - jekyll-remote-theme```
  4. Save the file.

## 8. Modify Gemfile
  1. Open Gemfile.
  2. Comment-out the following:
     - ```gem "jekyll", "~> 4.3.2"```
     - ```gem "minima", "~> 2.5"```
     - ```gem "jekyll-feed", "~> 0.12"```
  3. Add ```gem "slate", "~> 0.2.0"``` above ```#gem "minima", "~> 2.5"```.
  4. Add ```gem "jekyll-remote-theme"``` above ```#gem "jekyll-feed", "~> 0.12"```.
  5. Save the file.


## 9. Push To Main
  1. Open GitHub Desktop.
  2. Write a Summary of what you've completed so far, in text box lablled *Summary (required)*.
  3. Click the blue button lablled __Commit to main__.
  
  ![Image](/readmeAssets/GitHubDesktopCommit.png)


## 10. Let's See The Result!
  1. Navigate to your repositorie (github.com/*yourUsername*/*yourUsername*.github.io).
  2. Click the __Actions__ tab.
  3. Wait until there is a green check mark next to the latest __pages build and deployment__.
  4. Click the __<>Code__ tab.
  5. Click the __github-pages__ button, located on the right side of the page under Environments.
  6. Click __View deployment__ on the right hand side of the page.
  7. Congradulations! You now have your personal resume hosted on GitHub Pages! If you wish to go further and make more amazing projects I recommend you check out some of the resources and credits below, Cheers!🎉

---
# More Resources 📚
* Markdown
  * [Markdown Tutorial](https://www.markdowntutorial.com/) (Start Here)
  * [Basic Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) (Usefull)
  * [Advanced GitHub Flavored Markdown Cheatsheet](https://github.github.com/gfm/) (Extra)
* [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title)
* [GitHub Pages](https://pages.github.com/)

---
# Credits 📜
* [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title)
* [Jekyll Docs](https://jekyllrb.com/docs/)
* [GitHub's Jekyll Docs](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)
* [Jekyll Slate Theme](https://github.com/pages-themes/slate)
* [Adobe Convert to GIF](https://express.adobe.com/tools/convert-to-gif)

---
# FAQ ❓
- __Q:__ Why is Markdown better than a word processor?
  - __A:__ Most static site generators use Markdown files as inputs, because of this it makes it easy to update a static sites content without needed to rewrite any HTML or CSS, saving you much time.
- __Q:__ Why is my resume not showing up?
  - __A:__ It could be that your GitHub-Page is still being built. Open your repository and click the *Actions* tab. Under the *workflow runs* if you see any *orange circle* or text saying *queued* then your GitHub-Page is still being built.
  - __Solution:__ Leave it running for 5-10 minutes and comeback.
- __Q:__ What is a lightweight markup language?
  - __A:__ A lightweight markup language is what Technical Writers use tipically when writing documents, it allows writers to format their document without the use of special programs or charaters. Markdown is one of these lightweight markup languages. If your intrested in learning more I reccoment reading [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title)