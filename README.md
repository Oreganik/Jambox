How to start a new Unity project on Git with Jambox as a submodule

Using Jambox as a submodule allows developers to pull fixes and updates to Jambox, as well as push valuable changes or additions. This is important for Jambox to thrive, as it has always been guided by practical lessons in fast prototyping.

# Creating a new Unity project on Git
- Create a Github repo at github.com. We'll refer to its URL as {URL} in this doc.
- Create Unity project.
- Open a command line to the Unity project's root directory.
- Download the .gitattributes file
`curl -O https://raw.githubusercontent.com/Oreganik/JamboxTemplate/master/.gitattributes`
- Download the .gitignore file
`curl -O https://raw.githubusercontent.com/Oreganik/JamboxTemplate/master/.gitignore`
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

# Adding Jambox as a submodule
