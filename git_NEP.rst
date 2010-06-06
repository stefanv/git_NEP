======================================================================
NumPy Enhancement Proposal: The use of Git/Github for revision control
======================================================================

Introduction and motivation
---------------------------

Since its inception, NumPy's code base was stored in a revision
control system; first CVS and later SVN.  Importantly, these systems
provided the ability to track (and possible reverse) changes, and to
inspect code at different times in development history.

Another important feature was the ability to develop code in parallel
by the creation of *branches*.  Unfortunately, this functionality
proved hard to use: only registered developers could commit to the
repository, commits could not be made offline, and merging different
branches was difficult.

The introduction of distributed revision control systems addressed
many of these problems.  One such a system, `Git
<http://git-scm.com>`__, developed originally for managing the Linux
kernel sources, gained popularity amongst many NumPy developers.  So
far, it was used as an `SVN "bridge"
<http://www.kernel.org/pub/software/scm/git/docs/git-svn.html>`_; this
proposal provides a roadmap for a possible full transition.

The proposal also considers an online hosting solution, `GitHub
<http://github.com>`__, which is freely available to Open Source
projects.  It provides many of the services desired by the NumPy
developers, such as account management, commit e-mails and code
review.

Implementation
--------------

 - Convert repositories to Git with appropriate username handling
 - Add access to repo for current developers when requested (this also
   gives a chance to clean up the dev list); we work things the SVN
   way to start with
 - Add GitHub trac plugin
 - Setup commit mailing list on GitHub
 - Provide instructions on how to get hold of source via SVN
 - Point to good Git documentation (generate GitWash + existing docs
   on projects.scipy.org + tutorials elsewhere)
 - Update repository links in several places (docs, webapp, webpage,
   trac, launchpad, etc.)

Timeline
--------

Conclusion
----------
