# How to Hugo




### 1. Create Personal Github Page.

The first step in creating your Git Page is to navigate to your designated [GitHub](https://github.com) repo and create a repository in the format
`<USERNAME>.github.io`. Your reference guide for this step is the [official Git Pages guide](https://pages.github.com/). 

**Pro-Tip**: Note that it is imperative that `<USERNAME>` exactly matches your repo's username, or it will not work.


### 2. Install Hugo.

You can navigate the [Hugo installation guide](https://gohugo.io/getting-started/installing/), to install, setup and launch your local toy webpage.


### 3. Create your site.

Generate a sample website. Once you have your new site, you can navigate to [Hugo Quick Start](https://gohugo.io/getting-started/quick-start/). Once you have Hugo installed, generating a new site is as easy as typing `hugo new site <folder-name>`.


### 4. Add a theme.

You can browse through the free [Hugo themes](https://themes.gohugo.io/).  Optionally, customize themes to suit your needs. 

**Pro-Tip**: Since these are free, you may add multiple themes simultaneously, and designate the desired one in config.toml. Watch out for configuration incompatibilities across themes, though.


### 5. Add content.
After launching your site, you can create your first post markdown file named **my-first-post.md** with the command `hugo new posts/my-first-post.md`.

**Pro-Tip**: Hugo automatically generates posts with the `draft` parameter set to *True*. As soon as you are ready to post, you may change this to *False*.


### 6. Start the Hugo server. 

`hugo server -D` will launch a local version of your site that you can view on `http://localhost:1313/`. Any changes to your content will be automatically posted to your local (temporary) server-hosted site.

You can kill the local website via the command line by typing `CTRL+C`.


### 7. Deploy.

Once you have a starter webpage you are happy with, you should paste all files of your website into your local subdirectory.  

Then, enter the following command `git submodule add -b master https://github.com/<USERNAME>/<USERNAME>.github.io.git public`. This will create a Git submodule that will change your `public` subdirectory's remote origin to your GitHub repository.

Next, you can push the public subdirectory. Alternatively, the Hugo hosting guide (linked below) provides handy code for a `deploy.sh` executable file that pushes the public subdirectory to your GitHub repository, which GitHub will use to render your new website.

Further information about these steps can be found on the [Hosting on GitHub with Hugo](https://gohugo.io/hosting-and-deployment/hosting-on-github/) pages.

### 8. Give me feedback.

Notify me of any errors found or difficulties encountered.




