# READ(*L*)ME *This,* <sub><sup>*How does one host a resume using GitHub-Pages?*</sub></sup> 🤨

## Contents Table 📂
- [Prerequisites](#prerequisites-)
- [Steps](#steps-)
  1. [Software Instalation](#1-software-instalation)
  2. [Setting up GitHub-Pages](#2-setting-up-github-pages)
  3. [Setting-Up Local Repository](#3-setting-up-local-repository)
  4. [Create Default Files With Git Bash](#4-create-default-files-with-git-bash)
  5. [Test Site](#5-test-site)
  6. [Push To Main](#6-push-to-main)
- [More Resources](#more-resources-)
- [Credits](#contents-table-)
- [FAQ](#faq-)


## Prerequisites ❗
- Prior to starting this tutorial __you should__ already have a resume that is in Markdown format. If you don't have one I recommend checking out the *Markdown Tutorial* in the [More Resources](#more-resources-). 

---
# Steps 👣

## 1. Software Instalation
 1. Download [GitHub Desktop](https://desktop.github.com/)
 2. GitBash
    1. ?
 3. Download [Visual Studio Code](https://code.visualstudio.com/)
 

## 2. Setting-Up GitHub-Pages
  1. Navigate to your repositories (github.com/__*yourUsername*__?tab=repositories)
  2. Click on the green button that say's __New__
  
  ![Image](/readmeAssets/GitHubNewRepo.png)
  3. Type *__yourUsername__.github.io* into the text box labled *Repository name*
  4. Check-off the box labled *Add a README file*
  5. Click the green button labled *Create repository* 

## 3. Setting-Up Local Repository
  1. Navigate to your newly created repository (github.com/__*yourUsername*__/__*yourUsername*__.github.io)
  2. Click on the greed button that says __Code__
  3. Click *Open with GitHub Desk* -- (__Note:__ a popup may arise, if so, just click *Open GitHubDesktop.exe*) 
  4. Click the blue button labled __*Clone*__ once the GitHub Desktop application opens up -- (__Note:__ keep track of the *Local path* you are cloning to. This will be required in an upcomming step)

## 4. Create Default Files With Git Bash
  1. Open the *Git Bash* terminal
  2. Navigate to the *Local path* where your repository was cloned. This is an example of how to navigate files in a terminal with the cd command, ```cd 'C:\Users\yourAccount\Documents\GitHub\yourUsername.github.io'```
  3. Type the command ```gem install jekyll bundler```


## 5. Test Site
  1. Open the *Git Bash* terminal
  2. Navigate to the *Local path* where your repository was cloned. This is an example of how to navigate files in a terminal with the cd command, ```cd 'C:\Users\yourAccount\Documents\GitHub\yourUsername.github.io'```
  3. Type the command ```bundle exec jekyll serve```
  4. Wait till the terminal says ```Server running... press ctrl-c to stop.```
  5. Type http://localhost:4000/ into your browser.
  6. Once the page is loaded you should see your site.
  7. Close the site by pressing *ctrl-c*, followed by *Y* and the *enter* key


## 6. Push To Main
  1. Open GitHub Desktop
  2. Write a Summary of what you've completed so far, in text box labled *Summary (required)*
  3. Click the blue button labled *Commit to __main__*
  
  ![Image](/readmeAssets/GitHubDesktopCommit.png)

---
# More Resources 📚
* Markdown
  * [Markdown Tutorial](https://www.markdowntutorial.com/) (Start Here)
  * [Basic Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) (Usefull)
  * [Advanced GitHub Flavored Markdown Cheatsheet](https://github.github.com/gfm/) (Extra)
* [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title)

---
# Credits 📜
* [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title)
* [Jekyll Docs](https://jekyllrb.com/docs/)
* [GitHub's Jekyll Docs](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)

---
# FAQ ❓
- __Q:__ Why is Markdown better than a word processor?
  - __A:__ Most static site generators use Markdown files as inputs, because of this it makes it easy to update a static sites content without needed to rewrite any HTML or CSS, saving you much time.
- __Q:__ Why is my resume not showing up?
  - __A:__ It could be that your GitHub-Page is still being built. Open your repository and click the *Actions* tab. Under the *workflow runs* if you see any *orange circle* or text saying *queued* then your GitHub-Page is still being built.
  - __Solution:__ Leave it running for 5-10 minutes and comeback.