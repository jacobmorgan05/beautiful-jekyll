# Build your website in 3 steps

There's a very easy way to use this theme, and there's a hard way. For most people (including myself!), the easy route is recommended. If you're an advanced user and want to tinker with the hard way (using ruby gems), then [skip the easy way](https://github.com/daattali/beautiful-jekyll#the-hard-way-using-ruby-gems) if you know what you're doing.

## The easy way (recommended!)

Getting started is *literally* as easy as 1-2-3 :smile:

Scroll down to see the steps involved, but here is a 40-second video just as a reference as you work through the steps. If you don't already have a [GitHub account](https://github.com/join), you'll need to sign up.

![Installation steps](assets/img/install-steps.gif)

### 1. Fork this project

Fork this project by clicking the __*Fork*__ button at the top right corner of this page. Forking means that you now copied this entire project and all the files into your account.

### 2. Rename the project to `<yourusername>.github.io`

Click on __*Settings*__ at the top (the cog icon) and on that page you'll have an option to rename the project (*Repository name*). This will create a website with the **Beautiful Jekyll** template that will be available at `https://<yourusername>.github.io` within a couple minutes (check out the [FAQ](https://beautifuljekyll.com/faq/#custom-domain) if you want to use a different project name). If after a few minutes your website is still not ready, try making any edit to any file, just to force GitHub to re-build your site.

### 3. Customize your website settings

Edit the `_config.yml` file to change any settings you want. To edit the file, click on it to view the file and then click on the pencil icon to edit it (watch the video tutorial above if you're confused).  The settings in the file are self-explanatory and there are comments inside the file to help you understand what each setting does. Any line that begins with a hashtag (`#`) is a comment, and the other lines are actual settings.

Note that in the video above only one setting in the `_config.yml` file is edited. **You should actually go through the rest of the settings as well. Don't be lazy, go through all the settings!**

### 4. Congratulations! You have a website!

After you save your changes to the `_config.yml` file (by clicking on *Commit changes* as the video tutorial shows), your website should be ready in a minute or two at `https://<yourusername>.github.io`. Every time you make a change to any file, your website will get rebuilt and should be updated in about a minute or so. Your website will be initialized with several sample blog posts and a couple other pages.

Note that this was the easy way to *create* your website, but it does come at a cost: when Beautiful Jekyll gains new features in the future, *updating* your website to include all the latest features is cumbersome. See the [FAQ](https://beautifuljekyll.com/faq/#updating) for help with upgrading in the future.

## The hard way (using ruby gems)

If you followed the easy method above, then you already have your site and you can skip this section! If you want to use Beautiful Jekyll as a ruby gem instead, follow the [advanced installation instructions](https://beautifuljekyll.com/getstarted/#install-steps-hard). This is harder to set up initially, but it makes it super easy to keep your site up to date with Beautiful Jekyll when more features are added in the future.

# Plans

Beautiful Jekyll is, and always will be, free. But if you want to remove the Beautiful Jekyll ad from your website, use a Dark Mode skin, unlock other special rewards, or simply support the development efforts, [check out the different plans](https://beautifuljekyll.com/plans).

# Add your own content

To add pages to your site, you can either write a markdown file (`.md`) or you can write an HTML file. It's much easier to write markdown than HTML, so that's the recommended approach ([here's a great tutorial](https://markdowntutorial.com/) if you need to learn markdown in 5 minutes).

To see an example of a markdown file, click on any file that ends in `.md`, for example [`aboutme.md`](./aboutme.md). On that page you can see some nicely formatted text (there's a word in bold, a link, a few bullet points), and if you click on the pencil icon to edit the file, you'll see the markdown code that generated the pretty text. Very easy!

In contrast, look at [`tags.html`](./tags.html). That's how your write HTML - not as pretty. So stick with markdown if you don't know HTML.

Any markdown or HTML file that you create will be available on your website under `https://<yourusername>.github.io/<pagename>`. For example, if you create a file `about.md` (or `about.html`) then it'll exist at `https://<yourusername>.github.io/about`.

Files you create inside the [`_posts`](./_posts) directory will be treated as blog entries. You can look at the existing files there to get an idea of how to write blog posts. Note the format of the blog post files - they must follow the naming convention of `YEAR-MONTH-DAY-title.md`. After you successfully add your own post, you can delete the existing files inside [`_posts`](./_posts) to remove the sample posts, as those are just demo posts to help you learn.

# Customizing parameters for each page

**One last important thing**: In order to have your new pages use this template and not just be plain HTML pages, **you must add [YAML front matter](https://jekyllrb.com/docs/front-matter/) to the top of each page**:
