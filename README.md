# Opportunity Cell Website

## Important Info

### Markdown syntax

All front matter is written in [Markdown](https://guides.github.com/features/mastering-markdown/).

### Page variables

At the start of `*.md` files, there will be a section delimited by `---`. These are variables for each page.

1. `title` - title of the page
2. `nav_title`\[Optional\] - the text to be used in the navbar. `title` used as default
3. `nav_index` - the position of the page in the navbar. Sorted alphabetically otherwise.
4. `nav_ignore` - set to `true` if page is not to be shown in the navbar.
5. Other default variables can be found [here](https://jekyllrb.com/docs/variables/#page-variables)

### baseurl variable in config.yaml

Set the `baseurl` variable in `config.yaml` according to wherever you are going to host this site from relative to the root. For example, if the website is to be hosted on `https://web.iisermohali.ac.in/students/oppcell`, then set `baseurl: "/students/oppcell"`.
If viewing on Github, comment out the line as `# baseurl: ...`

## Updating

1. Clone repo and cd into it.
2. Follow the steps as described in the [Jekyll installation page](https://jekyllrb.com/docs/installation/)
3. Run `bundle install` then, `bundle update`
4. Run `bundle exec jekyll serve`
5. Open the browser to the server address as outputted in the previous command.
6. You should be able to see the site. Make changes as necessary, and check using `bundle exec jekyll serve`.
7. **When you are happy, use the files generated in `_site` and place in the production server.** Make sure you have set the `baseurl` in `_config.yaml` as discussed in [Important Info](#important-info).
8. Make sure you update `README.md` if necessary.

## Publishing

Publishing is done by using `sftp` to put files generated in `_site` onto the oppcell server. The login details needs to be provided by the faculty incharge of the OppCell to the webdev. Contact the CC for the same.
