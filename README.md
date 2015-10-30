# Forks and Clones

## Objectives

1. Fork a repo
2. Clone a repo
3. Push to different remote repos


##Forking a Github Repository
Forking a Github repository is just a way to create your own copy of any other Github repo. We do this all the time while using Learn, so you can use your copy as a sandbox to play around while maintaining a canonical repo where the original lab remains intact. In other words, it creates another remote that allows you to work in your own world without having to mess with our learn-co-student stuff.

You can fork any repo by clicking the "Fork" button at the top right any Github repository. 

![](https://github-images.s3.amazonaws.com/enterprise/2.2/assets/images/help/repository/fork_button.jpg)

[More on forking at the Github docs.](https://help.github.com/enterprise/2.2/user/articles/fork-a-repo/)

##Cloning
Now we want to get our forked copy of the repository on our local machine. This is where cloning is useful. To do this:

1. Find your forked repo on you Github profile
2. Click the "Copy to clipboard" button like the one below. This will copy the URL for us to use when we clone.

	![](https://github-images.s3.amazonaws.com/enterprise/2.2/assets/images/help/repository/clone-repo-clone-url-button.png)

3. In the terminal, let's run our clone command. It takes the URL we just copied as an argument:

	```bash
	git clone your-github-url
	```
	This will create a local copy of the repository that corresponds to the URL.
	
	
###Add both remotes
Since we cloned this down from a remote repository, our local copy is already connected to that remote. You can check this by running:

```bash
git remote -v
```

We can add another remote with the command:

```bash
git remote add name-for-your-remote the-github-url
```

If you run `git remote -v` again you will see that we now see that there are now two remotes that we can push to and pull from.


