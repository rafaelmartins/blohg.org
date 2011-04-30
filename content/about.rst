About blohg
===========

blohg_ is a Mercurial_-based blogging engine written in Python_, built with the
Flask_ micro-framework and some of his available extensions. All the content of
the blogs are stored inside Mercurial_ repositories and the repository history
is used for build the posts and pages. blohg uses Jinja2_ as template engine.

.. _blohg: http://blohg.org/
.. _Mercurial: http://mercurial.selenic.com/
.. _Python: http://python.org/
.. _Flask: http://flask.pocoo.org/
.. _Jinja2: http://jinja.pocoo.org/


Motivation
----------

Everybody knows that we have a big number of blogging engines lying around the
blogosphere, but there's not a lot of choices for programmers, that are used to
work daily with source-code editors and version control systems, and may be more
productive when blogging using these tools, instead of the fancy WYSIWYG_
editors and administration interfaces.

.. _WYSIWYG: http://en.wikipedia.org/wiki/WYSIWYG

Actually this isn't the first project trying to implement a VCS_-based blogging
engine, but most of the existing projects aren't tied to a VCS_ and are just
using text files that can be versioned with a VCS_, without take all his
advantages.

.. _VCS: http://en.wikipedia.org/wiki/Revision_control

This project uses Mercurial_ as VCS_ and reStructuredText_ as markup language.
Both are pretty popular on the Python ecosystem and pretty easy to use.

.. _reStructuredText: http://docutils.sourceforge.net/rst.html

Repository structure
--------------------

The repository structure is pretty easy to understand::

    blohg/repo_template/
    |-- config.yaml
    |-- content
    |   |-- about.rst
    |   `-- post
    |       |-- example-post.rst
    |       `-- lorem-ipsum.rst
    |-- static
    |   `-- screen.css
    `-- templates
        |-- base.html
        |-- post_list.html
        `-- posts.html

- ``config.yaml`` is the main configuration file.
- ``content/`` is the main directory for content (pages and posts). Posts are stored
  at ``content/post/``. Pages are stored anywhere inside ``content/``.
- ``static/`` is the directory with static files used by your blog, like css files
  or images.
- ``templates/`` is the directory with your Jinja2 templates.

