# TravelMaker
- Project repository
- In order to attach content to a project, project owner should be added as a distributor.
- The e-mail you are trying to add should be released in the personal profile > setting.
- Repository must be performed to become a distributor.

## Before push
- Before pushing, make sure to make a backup folder on your PC.
- This is because it reflects all unnecessary and deleted parts while downloading the latest data on the git.
- Of course you can use redo, but I recommend backup because it is tricky.

***
## Get config env
1. Go to the folder where you want to download projects locally
```
$ cd {path}
```
2. Set git init
```
$ git init
```
3. Git global settings
```
$ git config --global user.name {username}
$ git config --global user.email {email}
```
4. Project clone
```
$ git clone git@github.com:gau/TravelMaker.git
```
5. Set push url for a project
How to create a backup project, work it, and win a branch here.
- Project push is a worked project (ex) gahu/travelMaker
- Merge request is (ex) gahu/travelMaker for this project.
```
$ git remote add origin git@github.com:gau/TravelMaker.git
$ git remote set-url --push orgin git@github.com:gau/TravelMaker.git
```
5. If the remote path is:
- push url is a project that has been forked.
- fetch(pull) url is this project
```
$ git remote -v
Origin git@github.com:gau/TravelMaker.git (fetch)
Origin git@github.com:gau/TravelMaker.git (push)
```
It is irrelevant even if it is not done as it is, and it can be done even if fetch and push are equated.

6. Go to the Downloaded Project folder
```
$ cd BIBS
```
***
## Installation
Firstly make sure that you have Node and Git installed.
```
git clone https://github.com/gahu/TravelMaker.git
```
Then change into that folder
```
cd TravelMaker
```
install yarn (select)
``Javascript
npm install -g yarn
```
install the secret packages locally
```
npm install
yarn install
```
And start up a local server
```
npm start
yarn start
```
Now your app should be up and running.

***
## project push policy
1. All of the registers are worked locally by taking a personal branch.
- Merge request is registered in a factory with a new Branch.
```
$ git branch {operation brand name}
```
2. before local to push master the latest move to branch pull, to push branch make up to date.
```
$ get checkout master
$ git pull
$ get checkout {operation brand name}
$ git base master
```
3. Push with remote project. (Push with a brand other than the master brand in the remote project)
```
$ git add .
$ git commit -am "{Work content}"
$ git push orgin {operation bracket name}
```
4. Create a "pull request" in [gahu/TravelMaker] (https://github.com/gahu/TravelMaker.git/pulls).
- Tagging about what issues have been resolved through the full request commit message. ex) Resolve #{Issue} {Commit content}
5. The project owner checks the request and puts the contents of the push.
6. Remove the fresh bran after the Merge request as much as possible and allow the new branched to proceed.
```
$ get checkout master
$ git pull
$ git branch -D {operation brand name}
$ get checkout -b {New Branch Name}
```
- If you remove a Branch, remove the remote Branch information that is being tracked locally.
```

## coding convention
- The development tool uses AndroidStudio 3.0.