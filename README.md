# Apache Foundation Website (www.apache.org)

- [Production Website](https://www.apache.org/)
- [Staged Website](https://www.staged.apache.org/)

This repository provides the source for the main website of The Apache Software Foundation.

- [Content](content)
  - **md** pages in GitHub Flavored Markdown which can include HTML.
  - **ezmd** pages in a combination of [ezt](https://github.com/gstein/ezt/blob/wiki/Syntax.md) and GitHub Flavored Markdown.
  - **html** files are treated as static files.
  - static assets of all types.
  - .htaccess files for redirection and rewrite rules.

- [Issues](https://github.com/apache/www-site/issues)

- [Branches](https://github.com/apache/www-site/branches)

- [Pull Requests](https://github.com/apache/www-site/pulls)
  - [Creating a pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request#creating-the-pull-request)

- [Documentation](docs/)
  - [Creating content](docs/markdown.md) - how to create markdown and mix it with html.
  - [Data models and ezt](docs/data.md) - how the global data model works and how to enhance your data.
  - [Preview/feature branches](docs/branches.md) - how to make large or cooperative changes.
  - [Local builds](docs/local.md) - how to develop and test changes locally.

The website is built with [Pelican](https://blog.getpelican.com).
Continuous Integration / Continuous Deployment (CI/CD) is via the [.asf.yaml file](https://cwiki.apache.org/confluence/display/INFRA/Git+-+.asf.yaml+features)
mechanism which runs [Buildbot](https://ci2.apache.org/#/builders/3/).

- [Base Template](theme/apache/templates/base.html) -- single html skeleton
- [Templates](theme/apache/templates) -- see the full template folder
- [Custom Plugins](theme/plugins) -- site data and page processing
- [Pelican Configuration](pelicanconf.py) -- pelican configuration
- [ASF Data Load](asfdata.yaml) -- ASF metadata to be used by ezt and pelican. See [asfdata.py](theme/plugins/asfdata.py).
- [ASF YAML Pelican Build](.asf.yaml) -- ASF infrastructure instructions

The [svn history](http://svn.apache.org/viewvc/infrastructure/site/trunk/) was not migrated and remains available.

Foundation Records including Board Minutes remain in [svn](http://svn.apache.org/viewvc/infrastructure/site/trunk/content/foundation/records/)
except for the [index page](content/foundation/records/index.md).
