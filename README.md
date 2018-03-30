# (De)bug-off Template Repo

Fork this repo and make it your own.  You will use it for the remainder of this curriculum to practice collaborative workflow, and to build a de-bugging reference.  Keeping your repo up to date and contributing to your classmates' repos will take some effort, but will save you so much time in the future when you have a complete & well organized reference of common JS bugs.
 

Initial setup
* Fork this repo
* Set gh-pages settings to build from "master /docs"
  * This will host your notes live at "user_name".github.io/"repo_name"
* Clone the repo
* Run "npm install -g gitbook && gitbook install" in the cloned directory
* Run "chmod a+x ./scripts/publish.sh" in the cloned directory

To Publish:  
* Type "./scripts/publish.sh" from terminal in your Journal directory

Debugging Reference:
* Your GitBook will look [something like this](https://elewa-academy.github.io/de-bug-off-template).

Code Snippets:
* You will use [gitbook-plugin-include-codeblock](https://github.com/azu/gitbook-plugin-include-codeblock) to embed interactive code snippets into your debugging reference book.

Directory Structure Explained: 
```
(De)bug-off Repo
|
|-- /Challenges
|   * This is where you will host your debug challenges
|   * Give them unhelpful names so people have to figure out what's wrong
|
|-- /Cagegory-x
|   |-- /use-case-y
|   |   |-- fix.js          - your fix
|   |   |-- test-cases.js   - to play around with in the browser
|   |   |--- README.md      - where someone will go to study your solution
|   * Challengees will offer these files and directories in their pull requests
|   * You will accept or reject their requests to build your debugging reference book
|
|-- /docs
|   * The publis.sh script will buid the GitBook into this folder
|   * GitHub Pages will build from this folder
|
|-- /node_modules
|   * A lot
|
|-- /scripts
|   |-- build.sh    - Build the GitBook into /docs without publishing
|   |-- publish.sh  - Build & push the new notes GitBook to GitHub
|   |-- serve.sh    - Preview your GitBook at localhost:4000 without building
|
|-- .gitignore  - Tell Git not to push your node_modules folder to GitHub
|-- book.json   - A file written in JSON format that configures your GitBook
|-- CONTRIBUTING.md - Guidelines for people who'd like to contribut to your notes
|-- LICENSE.md  - A license, so people can respect your wishes
|-- README.md   - The "cover page" of your repo & GitBook
|-- SUMMARY.md  - Determines what will show up in your GitBook index


```


___
___
### <a href="http://elewa.education/blog" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/34921062-506450ae-f97d-11e7-875f-6feeb26ad72d.png" width="100" height="40"/></a>
