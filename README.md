# Jambox

Jambox is a collection of Unity code and assets developed by [Ted Brown](http://tedbrown.co). Guided by years of fast prototyping, game jams, and working as a lead engineer at game studios, it is a living open source project that has been slowly growing over time.

## How to start a new Unity project on Git with Jambox as a submodule

Using Jambox as a submodule allows developers to pull fixes and updates to Jambox, as well as push valuable changes or additions. This is important for Jambox to thrive, as it has always been guided by practical lessons in fast prototyping.

### Create a new Unity project on Git
- Create a Github repo at github.com. We'll refer to its URL as {URL} in this doc.
- Create Unity project.
- Open a command line to the Unity project's root directory.
- Download the .gitattributes file

`curl -O https://raw.githubusercontent.com/Oreganik/Jambox/master/.gitattributes`

- Download the .gitignore file

`curl -O https://raw.githubusercontent.com/Oreganik/Jambox/master/.gitignore`

- Initialize git

`git init .`

- Initialize git-lfs

`git lfs install`

- Add existing files and commit them

`git add . && git commit -m "Initial commit"`

- Upload the files

`git remote add origin {URL}.git`

- Change the branch name to main

`git branch -M main && git push -u origin main`

### Add Jambox as a submodule

- Make a directory called `Submodules` parallel to `Assets`.
- While still in the root directory of the git project, clone Jambox as a submodule.

`git submodule add https://github.com/Oreganik/Jambox Submodules/Jambox`

