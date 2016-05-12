Git Tutorial Prework
====================

Thanks for signing up for the `Get Started With Git`_ tutorial at PyCon 2016!
We're going to cover a *lot* of information in this tutorial, and even though
3 hours sounds like a long time, it's going to be tough to get through
everything. To make sure that we move as quickly as possible, you should make
sure that you've done all the following things *before* the tutorial begins:

* Install Git_
* Install a text editor with shell commands (Atom_ is a good choice)
* *Optional:* Install zsh_ and `oh-my-zsh`_
* Know how to use the command line
* Make an account on GitHub_
* *Optional:* Make an account on GitLab_ and/or BitBucket_

**Bring your computer with you to the tutorial!** The tutorial is very hands-on,
so you won't get much out of it without a computer.

Installing Software
-------------------

I strongly recommend using a `package manager`_ for installing software on
your computer. Not only do package managers make it easy to find and install
software, but they also make it easy to uninstall software, ensure that new
software packages don't break old ones, make it easy to upgrade software,
and keep your computer more secure. For OS X, you should use Homebrew_, and
for Windows, you should use Chocolatey_. I've written installation guides
for each of these operating systems that should make it easy to get up and
running:

* `Installation for OS X <https://github.com/singingwolfboy/git-tutorial-prework/blob/master/INSTALL-OSX.rst>`_
* `Installation for Windows <https://github.com/singingwolfboy/git-tutorial-prework/blob/master/INSTALL-WIN.rst>`_

Using the Command Line
----------------------

Git is best used on the command line. There are many different graphical
interfaces for Git, but they generally oversimplify Git and make it more
difficult to understand what is actually going on. The best way to develop a
deep understanding of how Git works is to use it on the command line. As a
result, this tutorial will not use *any* Git GUIs, but solely use Git on the
command line.

Before attending this tutorial, you should understand the basics of
how to use the command line on your operating system.
`Here is a basic tutorial, if you are not already familiar with the command line.
<https://www.davidbaumgold.com/tutorials/command-line/>`_
The instructor will be using the command line on OS X to run examples,
but the examples should also run on the Windows command line with minimal
changes.

You will have the best experience if you use the zsh_ shell with the
`oh-my-zsh`_ framework installed, since it has Git integration built-in.
However, you can use whatever shell you choose, including the default bash shell.

Making Accounts
---------------

During this tutorial, we will be interacting with GitHub_, which requires an
account. You can sign up on the homepage of GitHub.com.

GitHub is not the only website that hosts Git repositories: GitLab_ and
BitBucket_ are other popular options. You may want to create accounts for these
two websites before the tutorial begins, so that you can easily try moving
reposities from one host to another. The instructor will only discuss these
websites briefly during the tutorial, and none of the examples in the tutorial
will use either of these websites. As a result, signing up with these websites
is optional.

Feedback
========

If you have feedback about this tutorial, please `create a GitHub Issue for
this repository`_. Issues are a great way to collect and organize feedback,
so please feel free to contribute ideas and suggestions for how the instructor
can improve! Note that creating a GitHub issue requires a GitHub account.

.. _Get Started With Git: https://us.pycon.org/2016/schedule/presentation/1620/
.. _Git: https://git-scm.com/
.. _Atom: https://atom.io/
.. _Zsh: http://www.zsh.org/
.. _oh-my-zsh: http://ohmyz.sh/
.. _GitHub: https://github.com
.. _GitLab: https://gitlab.com
.. _BitBucket: https://bitbucket.org/
.. _package manager: https://en.wikipedia.org/wiki/Package_manager
.. _Homebrew: http://brew.sh/
.. _Chocolatey: https://chocolatey.org/
.. _create a GitHub Issue for this repository: https://github.com/singingwolfboy/git-tutorial-prework/issues
