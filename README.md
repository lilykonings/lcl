# [Life Changing Labs](http://www.lifechanginglabs.com/)

The LCL website is hosted on [Github Pages](https://pages.github.com/) and therefore supports [Jekyll](http://jekyllrb.com/). Please read the corresponding documentations for usage specific to either. This website was created by [Lillian Chen](http://lillian-chen.com/) and should not be used or altered without appropriate permissions from the organization.

## Datastructure
Before attempting to edit general text information, please note the following.

### Dependencies
[UIKit](http://getuikit.com/) serves as the front-end framework, which also requires FontAwesome. Lato is provided by Google.

### YAML Data
All data are loaded from [YAML](http://www.yaml.org/spec/1.2/spec.html) files in the `_data` directory. Right now, the following "databases" are active:

- `blog.yml` - `/blog`
- `companies.yml` - `/companies`
- `guests.yml` - `/network`
- `members.yml` - `/network`
- `partners.yml` - `/network`

Properties in these data files are accessed via `site.data`.

### Blog
The blog is managed by Jekyll's native "blog aware" functionality in the `_posts` directory. Images are stored in `{{ site.url }}/lcl/assets/img/blog`

When creating new posts, you **must** follow the Jekyll convention for naming post files, such as `2014-06-11-example.md`. All posts are written in Markdown with the following front matter: `title, author, layout, categories, id`. `layout` must be "blogpost". `categories` and `id` must always be "blog".

If the author of a post wants to include a short bio, simply add his/her name and bio to `blog.yml`.