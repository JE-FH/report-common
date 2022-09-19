# 🎊 Welcome to the Common Report Sections 🥳

This repo contains all of the collaborative report sections. These sections are to be included in your project reports. They document the collaborative aspects of the semester project. This README documents the structure of these sections aswell as what should be included in each section.

## Structure

This repo contains a folder called common. This folder contains all of the common sections.

## Inclusion in Your Report

If you are using git for version controlling your report, including this content is quite easy. In the terminal, simply navigate to the directory that contains your report and type.

git clone #URL common

you will then have a folder called common (Unless you specified another name when you cloned the repo).

Input the sections in the report using \input{path/to/file}

### If you are using overleaf for your project

1. Open your overleaf project.
2. Press the 'Menu' button in the top left corner.
3. Under the 'Sync' category, select 'Git'
4. Copy the command.
5. In the terminal, navigate to some location where you can clone your project

   (could be `C:\\repos\`, but that is up to you.)

6. Paste the command and remember to give your project a recoginizable name.
   ``` bash
   git clone https://git.overleaf.com/63260da163b20whatever p5-project
   ```
   Authenticate using overleaf login.

7. In the terminal, cd into your project folder (cd p5-project)
8. add the common repo as a remote for your repo
   ``` bash
   git remote add -f common #URL
   ```
   and then:
   ``` bash
   git merge common/master --allow-unrelated-histories
   ```
   if you forgot to write `-f` when you added the remote you need to fetch before you merge.

9. Finally, to push your changes back to overleaf, just use git to push.

### If you are using git
Just skip to step 8 in the section above 😉

### Updating the common sections.
Using git, first make sure that you pull origin
``` bash
git pull origin/master
```
Then pull common
``` bash
git pull common/master
```
And finally,
``` bash
git push origin
```


### Why don't I just download the source files off GitHub and include them manually?

Because then you won't be able to just write git pull and update all of the collaborative sections automatically, silly 🤪

(but you could also do that, i guess)

## 🎉🎉 Contribution 🎉🎉
If you want to contribute, please fork this repo and create a pull request.

## Comments and Suggestions
If you have comments or suggestions, let's talk about it!
Feel free to create issues and comment on other issues.

hehe
