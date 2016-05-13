Installation for Arch Linux
===========================

This page will walk you through installing software for the
`Get Started With Git`_ tutorial on your Arch Linux computer.

Install Git
-----------

Use the Pacman_ package manager to install Git by running the following command:

.. code-block:: bash

   $ sudo pacman -S git

This will show the dependecies for Git and then confirm that you would like to
download the package. Typing ``y`` will pass the prompt and install Git.

Install Atom
------------

You'll need a text editor to use Git effectively, and Atom_ is an
excellent choice. Unfortunately, Atom is not available in the Pacman repository
by default, but it is in the `Arch User Repository`_ (AUR). To install Atom
from the AUR, follow the folloing steps:

1. Download the `Atom package from the AUR`_ and save it on your computer.
2. Extract the tarball by running ``tar -xvf atom-editor.tar.gz``
3. Install it by running ``makepkg -sri``. This command will download the
   source code, resolve dependencies, compile the code, package it,
   install the package, and finally remove any build-only dependencies.

When the installation is complete, you should be able to run Atom with
the ``atom`` command. Test it to be sure!

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
.. _Pacman: https://wiki.archlinux.org/index.php/pacman
.. _Arch User Repository: https://aur.archlinux.org/
.. _Atom package from the AUR: https://aur.archlinux.org/cgit/aur.git/snapshot/atom-editor.tar.gz
.. _package manager: https://en.wikipedia.org/wiki/Package_manager
.. _Atom: https://atom.io/
.. _Zsh: http://www.zsh.org/
.. _oh-my-zsh: http://ohmyz.sh/
