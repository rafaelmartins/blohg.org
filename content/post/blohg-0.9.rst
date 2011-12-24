blohg-0.9
=========

.. tags: announcements, releases

I'm proud to announce the release of blohg 0.9. This version comes with some
pretty cool features:

- Allowed users to remove the ``post_list.html`` template, if wanted.
- Allowed users to disable the ``source`` endpoint, if they don't want to make
  their reStructuredText sources public.
- Added a ``blohg freeze`` command to blohg, that allows people to build a static
  version of blohg, to deploy it on servers without wsgi support. Thanks to
  Benoit Allard.
- Fixed bugs related to the ``config.yaml`` file from the repository being loaded
  late. Thanks to Benoit Allard.
- Rewrote the Mercurial/reStructuredText layer, to make it request-independent as
  possible.
- Improved version detection, when installing blohg from the Mercurial repository.
- Fixed main script to work inside subdirectories of the repository. Thanks to
  Benoit Allard.
- Added a reStructuredText role (``:page:``) to create links to other pages of
  the blog. Thanks to Benoit Allard.
- Started a very minimal test-suite.

See the documentation_ for details:

.. _documentation: http://docs.blohg.org/

Enjoy!
