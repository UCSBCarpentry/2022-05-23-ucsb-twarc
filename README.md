[![Website](https://github.com/carpentries/workshop-template/actions/workflows/website.yml/badge.svg)](https://github.com/carpentries/workshop-template/actions/workflows/website.yml)

# Twitter with twarc: May, 2022

This repository is for a pilot TWARC Workshop, made using The Carpentries' ([Software Carpentry][swc-site], [Data Carpentry][dc-site], and
[Library Carpentry][lc-site]'s) template for creating websites for workshops.

1. Please *do your work in your repository's `gh-pages` branch*, since that is what is
   [automatically published as a website by GitHub][github-project-pages].

The pages on [customizing your website][customization],
the [FAQ][faq],
and the [design notes][design] have more detail on what we do and why.
And please note:
if you are teaching Git,
please [create a separate repository](#setting-up-a-separate-repository-for-learners)
for your learners to practice in.

## Video Tutorial

There is a [YouTube video](https://www.youtube.com/watch?v=_Ag1JiZzyUQ) that demonstrates how to
create a workshop website.

## Creating a Repository

-customized up to here-

5. Edit the `schedule.html` file to edit the schedule for your upcoming workshop. This file is
   located in the `_includes` directory, make sure to choose the one from the appropriate `dc` (Data
   Carpentry workshop), `lc` (Library Carpentry), or `swc` (Software Carpentry) subdirectory.

### Working locally

> Note: you don't have to do this, if you have already updated your site using the web interface.


If you are already familiar with Git, you can clone the repository to your desktop, edit `index.md`,
`_config.yml`, and `schedule.html` following the instruction above there, and push your changes back to the repository.


In order to view your changes once you are done editing, if you have bundler installed (see the
[installation instructions below](#installing-software)), you can preview your site locally with:

```shell
make serve
```
and go to <http://0.0.0.0:4000> to preview your site.

Before pushing your changes to your repository, we recommend that you also check for any potential
issues with your site by running:

```shell
make workshop-check
```

Once you are satisfied with the edits to your site, commit and push the changes to your repository.
A few minutes later, you can go to the GitHub Pages URL for your workshop site and preview it. In the example above, this is `https://gvwilson.github.io/2016-12-01-oomza`. [The finished
page should look something like this](fig/completed-page.png?raw=true).


## Optional but Recommended Steps


### Update your repository description and link your website

At the top of your repository on GitHub you'll see

~~~
No description, website, or topics provided. — Edit
~~~

Click 'Edit' and add:

1.  A very brief description of your workshop in the "Description" box (e.g., "Oomza University workshop, Dec. 2016")

2.  The URL for your workshop in the "Website" box (e.g., `https://gvwilson.github.io/2016-12-01-oomza`)

This will help people find your website if they come to your repository's home page.

## Additional Notes

**Note:**
please do all of your work in your repository's `gh-pages` branch,
since [GitHub automatically publishes that as a website][github-project-pages].

**Note:**
this template includes some files and directories that most workshops do not need,
but which provide a standard place to put extra content if desired.
See the [design notes][design] for more information about these.

Further instructions are available in [the customization instructions][customization].
This [FAQ][faq] includes a few extra tips (additions are always welcome)
and these notes on [the background and design][design] of this template may help as well.


## Creating Extra Pages

In rare cases,
you may want to add extra pages to your workshop website.
You can do this by putting either Markdown or HTML pages in the website's root directory
and styling them according to the instructions give in
[the lesson template][lesson-example].


## Installing Software

If you want to set up Jekyll so that you can preview changes on your own machine before pushing them
to GitHub, you must install the software described in the lesson example [setup
instructions](https://carpentries.github.io/lesson-example/setup.html#jekyll-setup-for-lesson-development).


## Getting and Giving Help

We are committed to offering a pleasant setup experience for our learners and organizers.
If you find bugs in our instructions,
or would like to suggest improvements,
please [file an issue][issues]
or [mail us][email].

[email]: mailto:team@carpentries.org
[customization]: https://carpentries.github.io/workshop-template/customization/index.html
[dc-site]: https://datacarpentry.org
[design]: https://carpentries.github.io/workshop-template/design/index.html
[faq]: https://carpentries.github.io/workshop-template/faq/index.html
[github-project-pages]: https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site
[issues]: https://github.com/carpentries/workshop-template/issues
[lesson-example]: https://carpentries.github.io/lesson-example/
[self-organized-workshop-form]: https://amy.carpentries.org/forms/self-organised/
[swc-site]: https://software-carpentry.org
[lc-site]: https://librarycarpentry.org
