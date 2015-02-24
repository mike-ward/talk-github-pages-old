title: GitHub Pages  
author:  
  name: Mike Ward  
  twitter: mikeward_aa  
  url: http://mike-ward.net  
output: talk-github-pages.html  
style: style.css  
--

# GitHub Pages
## Websites for you and your projects

--

### What are GitHub Pages?

GitHub Pages are public web pages hosted and published through the GitHub site.

Pages consist of *static* pages and assets only

Pages can be generated using the [Automatic Page Generator](https://help.github.com/articles/creating-pages-with-the-automatic-generator), with a static site generator or by hand.

--

### 5 Reasons to use GitHub Pages

1. It's fast (really fast)
2. It's simple
3. Automatic deployment
4. Uses Git
5. No special tooling/databases etc.

--

### Step 1

#### Create a repository

Head over to GitHub and create a new repository named username.github.io, where username is your username (or organization name) on GitHub.

*If the first part of the repository doesn’t exactly match your username, it won’t work, so make sure to get it right.*

--

### Step 2

#### Clone the repository

Go to the folder where you want to store your project, and clone the new repository:

    git clone https://github.com/username/username.github.io

--

### Step 3

#### Hello World

Enter the project folder and add an index.html file:

    cd username.github.io
    echo "Hello World" > index.html

--

### Step 4

#### Push it

Add, commit, and push your changes:

    git add --all
    git commit -m "Initial commit"
    git push -u origin master

--

### Step 5

...and you're done!

Fire up a browser and go to http://username.github.io.

<video src="flying.mp4" controls autoplay loop />

--

### I can haz Project Pages?

Project Pages are kept in the same repository as their project.

The URL for a personal account's Project Page will be `http(s)://<username>.github.io/<projectname>`

Project Pages differences:

The `gh-pages` branch is used to build and publish Project Pages sites.

Project Pages sites are served under a subpath of the User Pages site: `username.github.io/projectname`

--

### Blogging with Jekyll

[Jekyll Now](https://github.com/barryclark/jekyll-now)

![three amigos](giphy.gif)

--

### Custom URLs

Just create a file named CNAME and include your URL.

After you've created and committed your CNAME file on GitHub, do one of the following with your DNS provider:

1. If your custom domain is a subdomain (recommended), configure a CNAME record.

2. If your custom domain is an apex domain, configure an `ALIAS`, `ANAME`, or `A` records.
