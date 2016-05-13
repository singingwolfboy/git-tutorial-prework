Installation for Windows
========================

This page will walk you through installing software for the
`Get Started With Git`_ tutorial  on your Windows computer. Using the Chocolatey_
package manager is *strongly* recommended, but if you want to install the
required software without using a package manager, you can do so.

Install Chocolatey
------------------

Chocolatey_ is a `package manager`_ for Windows, and it makes it easy to install,
update, and uninstall software on your computer. To install Chocolatey,
go to the Chocolatey_ website and follow the instructions on the
home page. Note that there are two different commands to copy-paste, but you
only need to run *one* of them, not both. (However, there's no harm in running
both.)

Once you've installed Chocolatey successfully, you'll have access to the
``choco`` command. Try running that command to test it:

.. code-block:: bash

    C:\> choco

Install Git
-----------

Once you have Chocolatey installed, installing Git is easy!

.. code-block:: bash

    C:\> choco install git

Then you can use the ``where`` utility to test that it's installed:

.. code-block:: bash

    C:\> where git
    C:\Program Files\Git\cmd\git.exe

Install Atom
------------

You'll need a text editor to use Git effectively, and `Atom`_ is an
excellent choice. We can use Chocolatey_ to install it, like this:

.. code-block:: bash

    C:\> choco install atom

Once it's finished installing, you should be open to run Atom from
the Start menu, like any other Windows program.

Next, we need to tell Git how to find and use Atom. Fortunately, this only
requires running one command:

.. code-block:: bash

    C:\> git config --global core.editor "atom --wait"

Check that it worked by asking Git what the "core.editor" config value is:

.. code-block:: bash

    C:\> git config core.editor
    atom --wait

Install Zsh (optional)
----------------------

Zsh_ is a shell for your command line, and `oh-my-zsh`_ is a framework for
installing themes and plugins for that shell. You don't need to install these
things, but they make it easier to keep track of where you are and what you're
doing when you use Git.

To run Zsh and oh-my-zsh on Windows, we're going to use a piece of software
called Babun_. With Chocolatey, installing Babun is a breeze:

.. code-block:: bash

    C:\> choco install babun

Now you'll be able to run Babun from the Start menu. Use it *instead* of your
normal `cmd.exe` command line. Babun is already set up with Zsh and oh-my-zsh,
so you're all done!

If you don't like the way it looks, you can edit the
``.zshrc`` file in your home directory and pick a different theme.

.. _Get Started With Git: https://us.pycon.org/2016/schedule/presentation/1620/
.. _Chocolatey: https://chocolatey.org/
.. _package manager: https://en.wikipedia.org/wiki/Package_manager
.. _Atom: https://atom.io/
.. _Zsh: http://www.zsh.org/
.. _oh-my-zsh: http://ohmyz.sh/
.. _Babun: https://babun.github.io/
