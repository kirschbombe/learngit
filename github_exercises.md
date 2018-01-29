## Hands-on with GitHub

### Create a new repository

1. Login to GitHub: https://github.com
2. Click the green **New repository** button  --or-- click the **+** on the top, right corner of the GitHub page and select **New repository**
3. Give your new repo a name -- you can also add a description if you want
4. Choose whether your repo will be public or private. Free accounts are limited to public repos only (unless you get an education account!)
5. Initialize with a **README**. A README tells others what your repo is all about. You can also add a license at this point.
6. Click **Create repository**
7. Now you have a new GitHub repository!

### Editing/adding content to your new repo

1. Edit the `README.md` file
    * Click on the `README.md` file. This will open up a preview of the file.
    * To edit the file, click on the **pencil icon** in the top, right corner of the file ![](https://osu.ppy.sh/help/wiki/osu!wiki_Contribution_Guide/GitHub_Web_Interface/img/online-editing.jpg)
    * Now we can edit our file. `.md` files are **Markdown** files that use a simple markup language for formatting text. For more info on Markdown, [consult this guide](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).
    * When you are done editing, scroll to the bottom and click on the green "Commit changes" button. You will want to make sure that "Commit directly to the `master` branch" is selected.
2. Now let's add a new file to the repo
    * Go back to your repo "home", then click the "Create new file" button
    * This will take us directly to the edit view, but this time we need to give our file a name first - don't forget the file extension! We'll create another Markdown file (`newfile.md`).
    * Add some content to your file and commit your changes
3. Now let's add a folder
    * Where's the **Create new folder** button?!
    * There isn't one - but we can create a folder by prepending the filename with a folder + `/` while we are in edit mode :) For example, `newfolder/file.md`. Once you type in the `/`, the filename will automatically separate into a folder and filename.
    
### A simple website with GitHub Pages

1. Go to the top-level of your GitHub repo and create a new folder/file called `docs/index.html`
2. Add some html to the new file, something like this:

```
<html>
  <head>
    <title>Hello, World</title>
  </head>
  <body>
    <h1>Hello, World</h1>
    <img src="https://cdn.dribbble.com/users/983703/screenshots/2852241/hello-dribble.gif">
    <p>This is my project homepage.</p>
  </body>
</html>
```

3. Commit your changes, then go to your repo **Settings** tab
4. Scroll down until you reach the **GitHub Pages** section
5. Under Source, choose the "master branch /docs folder" option, and click on the **Save** button
6. You should see a blue box with the text "Your site is ready to be published at..." + a URL - you'll want to refresh the page until the box is green and says "Your site is published at..."
7. Click on the URL and see your new webpage!

### Collaborating, Forking, Merging

1. Time to partner up! Choose who will be **Partner1** and **Partner2**
2. **Partner1**: Share your repo URL with Partner2
3. **Partner2**: Fork Partner1's repo using the **Fork** button - you'll see an animation of GitHub copying your partner's repo into your account
4. **Partner2**: You now have a copy of Partner1's repo - make a few changes (add files, edit files, etc.)
5. **Partner2**: Once you've committed all your edits, submit a **Pull request**. This will send a request to Partner1 asking to merge your edits into their repo.
6. **Partner1**: Check the **Pull requests** tab in your repo and open the request (just click on it)
7. **Partner1**: View the edits and accept or close the pull request
8. Now switch roles and repeat :)
