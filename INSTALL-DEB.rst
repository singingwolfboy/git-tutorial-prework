Installation for Debian/Ubuntu
==============================

This page will walk you through installing software for the
`Get Started With Git`_ tutorial on your Ubuntu Linux or Debian Linux computer.

Install Git
-----------

Use the Apt_ package manager to install Git by running the following command:

.. code-block:: bash

   $ sudo apt-get install git

This will show the dependecies for Git and then confirm that you would like to
download the package. Typing ``y`` will pass the prompt and install Git.

Install Atom
------------

You'll need a text editor to use Git effectively, and Atom_ is an
excellent choice. Unfortunatly Atom_ is not in Apt_\'s repository by default;
however, you can download it yourself and then install it with ``dpkg``.

First, download `Atom for Debian/Ubuntu`_. Next we need to create the
package. We do this with the ``dpkg`` command like so:

.. code-block:: bash

   sudo dpkg --install atom-amd64.deb

Now we can run Atom with the ``atom`` command!

Next, we need to tell Git how to find and use Atom. Fortunately, this only
requires running one command:

.. code-block:: bash

    $ git config --global core.editor "atom --wait"

Check that it worked by asking Git what the "core.editor" config value is:

.. code-block:: bash

    $ git config core.editor
    atom --wait

Install Zsh (optional)
----------------------

Zsh_ is a shell for your command line, and `oh-my-zsh`_ is a framework for
installing themes and plugins for that shell. You don't need to install these
things, but they make it easier to keep track of where you are and what you're
doing when you use Git.

With Apt, installing Zsh_ is a breeze:

.. code-block:: bash

    $ sudo apt-get install zsh

Then install `oh-my-zsh`_ by following the directions on the homepage:

.. code-block:: bash

    $ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

Open a new command line window, and verify that it looks different -- and
probably a lot nicer! If you don't like the way it looks, you can edit the
``.zshrc`` file in your home directory and pick a different theme.

You're all done!

.. _Get Started With Git: https://us.pycon.org/2016/schedule/presentation/1620/
.. _Apt: https://wiki.debian.org/Apt
.. _Atom: https://atom.io/
.. _Atom for Debian/Ubuntu: https://github.com/atom/atom/releases/download/v1.7.3/atom-amd64.deb
.. _Zsh: http://www.zsh.org/
.. _oh-my-zsh: http://ohmyz.sh/
