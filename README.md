# ICME Summer Workshop Website Template
This repository is intended for ICME Summer Workshop Instructors, to facilitate
website creation. The steps laid out below are intended to guide you through
the process of creating a publicly viewable [Github
Page(s)](https://pages.github.com/) that are templated with ICME Summer Workshops in mind. 

It is the author's belief that by creating a unified template to work from, that students can focus more 
on learning the content of the courses and worry less about how to navigate through each course's custom website UI; 
this is important since many students involved with Summer Workshops tend to take multiple courses.

## Taking the first step
Initially, you'll want to be at least a little bit familiar with Git; see
[About Git](https://docs.github.com/en/get-started/using-git/about-git) for more information on getting started 
with basic commands if you're unfamiliar with how this tooling works. Then, I would recommend you go through the following two steps:

1. Within the GitHub UI, create a new repository and clone it to your local
machine; the repository name should be reflective of how you wish for your
website-name to be specified. I.e. website URL's will be of the form
`<github_id>.github.io/<repository_name>`.
2. Also within the Github UI, clone the `icme-summer-workshop-template`
repository to your local machine.
3. Copy the contents of the `icme-summer-workshop-template` into the repository
created in the first step. Commit these changes and push them to GitHub.

## Filling in the contents of the website
The file `index.md` is really the file that you want to look at and modify when
changing your website.

Please replace `TODO(instructor)` comments with the relevant text that is being
requested to be filled in. If you're wondering about a complete listing of
`TODO`'s, simply navigate to your working directory in a Command Line Interface
and execute the following command:

```
grep -r 'TODO(instructor)' *
```

This will then pull up a listing of remaining to-do items that need to be
cleared before the website is ready for students to view/use.

## Previewing your website
You'll want to get an idea for what the website currently looks like as you
modify it. There are is a set-up step and two recurring steps that must be done
with each change you wish to make. 

### Initial Github Pages Set-up
To set-up your website initially,
navigate to the Github-UI for your repository (e.g. something like
`github.com/<username>/<repository-name>`), then click the `settings` pane
toward the top-right corner of the page, then click `pages` within the bottom of
the left pane, then under the **Source** section select that you wish to use
`main` branch and hit "save". You should now see text-appear within the page
that says, "Your site is ready to be published at: <url>".

### Previewing Changes
When you make changes to your website, one way to view your changes would be to
actually publish them to your website and inspect the live URL.
  * Commit changes to Github _and push_ said changes to your online repository.
    This would be done via a sequence of commands, e.g.
      * `git add 'my_recently_modified_file'`
      * `git commit -m 'Insert a helpful commit message here.'`
      * `git push` (possibly followed by an authentication step)
    Note: there is some latency between pushing changing and having them deployed to the live website; to view the build process simply navigate to the `Actions` tab within the upper-panel of the GitHub UI, and then you should see "All workflows" and within it the progress of `pages-build-deployment`.
  * Use your web-browser to navigate to the following link:
  ```
  <github_username>.github.io/icme-summer-workshop-template
  ```
  
## Website Structure
### Modifying `index.md`
We mentioned previously that `index.md` is the backbone of the website; please
take your time to go through this raw-file and replace / update the contents
with information that is pertinent to your workshop.

There are, however, some additional sources of input used when constructing the
website.

### The left-panel of the website
There is some meta-data that needs to get updated within the left panel of the
site. Please go through the following steps

  * Within `_layouts/default.html`:
    * Update any _downloads_ that are relevant to your workshop (lines 39-41):
      * To be explicit, you should place your workshop content in an
appropriately named file within the `docs/` folder, making sure to commit and
push your changes to GitHub. Then, whatever you chose for your filename, make
sure to insert that filename on e.g. line 39.
    * Update your name to appear as Lecturer and update the email appearing on lines 50-51, i.e. rreplace `SUNET` with your relevant `SUNET` (or more generally, your email
address).
  * Within `_config.yml`:
    * Replace the `title:` attribute with a name more pertinent to your particular workshop.

# References
This site is built using [Jekyll Minimal
Theme](https://github.com/pages-themes/minimal).
