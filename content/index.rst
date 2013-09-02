About blohg
===========

blohg_ is a Mercurial_ (or alternatively Git_) based blogging engine written in
Python_, built on the top of the Flask_ micro-framework and some of its extensions.
All the content of the blogs are stored inside repositories, and the repository
history is used to build the posts and pages.

.. _blohg: http://blohg.org/
.. _Mercurial: http://mercurial.selenic.com/
.. _Git: http://git-scm.com/
.. _Python: http://python.org/
.. _Flask: http://flask.pocoo.org/


Motivation
----------

Everybody knows that we have a large number of blogging engines lying around the
blogosphere, but there are not a many choices for programmers, who are used to
working daily with source-code editors and version control systems and may be more
productive when blogging using these tools, instead of the fancy WYSIWYG_
editors and administration interfaces.

.. _WYSIWYG: http://en.wikipedia.org/wiki/WYSIWYG

Actually this isn't the first project trying to implement a VCS_-based blogging
engine, but most of the existing projects aren't tied to a VCS_ and are just
using text files that can be versioned with a VCS_, without taking full
advantage of the VCS's revision history.

.. _VCS: http://en.wikipedia.org/wiki/Revision_control

This project uses Mercurial_ (or even Git_) as the VCS_, reStructuredText_ as
the markup language and Jinja2_ as the template engine. All of these are pretty
popular within the Python ecosystem and easy to use.

.. _reStructuredText: http://docutils.sourceforge.net/rst.html
.. _Jinja2: http://jinja.pocoo.org/


