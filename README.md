This is the collaborative Jekyll site for CMS.636 - Extending the Museum, a digital humanities course at MIT. If you are the site administrator and wish to prepare for an upcoming run of the course by archiving the existing site and setting up a new copy, see the following instructions.

### Archiving the existing site
1. If you don’t yet have a local copy of the cms636.github.io repository, run `git clone https://github.com/cms636/cms636.github.io.git` in the command line
1. In the command line, run `cd cms636.github.io` (swap in the name of the directory containing your local copy of the repo, if different). Run `git pull` to bring it up to date.
1. Make a copy of your local cms636.github.io directory. Name it **cms636-new**.
1. In your web browser, log in to GitHub using the cms636 login (passord in HS wiki). Go to [https://github.com/cms636/cms636.github.io/settings](https://github.com/cms636/cms636.github.io/settings)
1. Under settings > Repository name, change cms636.github.io to Fall-2021. Click rename.
1. In the command line, in your **cms636.github.io** directory, run `git remote set-url origin https://github.com/cms636/Fall-2021.git`
1. In your **cms636.github.io** directory, open `_config.yml` in a text editor. In the lines reading `url:` and `siteurl: "http://cms636.github.io"`, add `/Fall-2021` to the end of the url string. Also add `/Fall-2021` inside the quotes after `baseurl:`. In the line with `relativeLinks:`, add `/Fall-2021` before `/links.jsonp`.
1. In your **cms636.github.io** directory, navigate to the _includes directory and open header.html in a text editor. Add this line of HTML before line 5 (`<a class=“site-tile” …`):<br /> `<p class="archive-notice">This is the archived site for the Fall 2021 session of CMS.636 — for the current site, click <a href="http://cms636.github.io/">here</a>.</p>`
1. In the command line, run the following commands:<br />
`git add .`<br />
`git commit -m "changes for archived site"`<br />
`git push origin master`
1. At [https://github.com/cms636/Fall-2021](https://github.com/cms636/Fall-2021), click the dropdown button that says “Branch: master”. In the text field, type gh-pages. Then click “Create branch: gh-pages.”
1. In the command line, run `cd ../` to back out of the directory.
1. Rename your local **cms636.github.io** directory to **cms636-Fall-2021**.
1. Notify last year's students that URLs for their material on the site have changed (they will need to insert `/Fall-2021` in any links to the site). The students are still collaborators on the archived site. If they wish to edit or remove their content, they should push changes to the gh-pages branch of the repo.

### Preparing the new site
1. Rename the **cms636-new** directory you made to **cms636.github.io**. You should now have two directories: one called **cms636.github.io** (containing the original code) and one called **cms636-Fall-2021** (containing the changed code with all of the Fall 2021 details).
1. In the command line, run `cd cms636.github.io` and open the **cms636.github.io** folder in your file browser. (You can safely close **cms636-Fall-2021** now--consider it fully archived.)
1. Clean out any content here you don’t wish to keep:
    - Images and other from the `assets` folder, except for any used by posts or pages that will remain
    - Posts from the `_posts` folder (selectively, as some resource or bio posts will still be useful; keep in mind that almost all of the site content is in this folder)
    - Anything in the `_drafts` folder
1. Copy the new syllabus PDF to the `assets` folder and name it cms-636-syllabus.pdf (replacing the old one if it’s still there).
1. Open `index.html` in a text editor. In line 20, change the URL for the Stellar site to the correct URL for this year’s course.
1. Open `_includes/header.html` in a text editor. Find the line (30) that reads `<li><a href="http://cms636.github.io/Fall-2020/">Fall 2020</a></li>`. Copy and paste it onto the next line and change both the URL and the text from `2020` to `2021`.
1. Open README.md. First, this line (31) will need to be edited such that the highest year in the following sentence is incremented by 1. Then, find-and-replace all instances of `2021` with `2021` and all instances of `2020` with `2021`.  (Basically, we just need to increment every year by 1.)
1. Save all changes. In the command line, run `git add .`, then `git commit -m “updated site for current year”`.
1. In your web browser, go to [https://github.com/new](https://github.com/new) and in the “Repository name” field, type "cms636.github.io". Enter a description in the “Description" field, e.g. "Course site for CMS 636/855 — Extending the Museum”. Click “Create repository”.
1. If using GitHub credentials in the command line other than those for cms636, add yourself as a collaborator (see below). For attaching GitHub credentials to git, see [https://help.github.com/articles/set-up-git/](https://help.github.com/articles/set-up-git/)
1. In the command line, run `git push origin master`.
1. The new site should appear at [https://cms636.github.io](https://cms636.github.io).

### Adding students as collaborators
1. Each student must first create their own GitHub account (if they don’t already have one) and email their username to you.
1. At https://github.com/cms636/cms636.github.io/settings/collaboration, enter the student’s username and click “Add collaborator".
1. Direct students to the [Contributing to This Site](https://cms636.github.io/about/) for instructions on using prose.io to add content.
