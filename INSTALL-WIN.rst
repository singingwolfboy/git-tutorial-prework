Installation for Windows
========================

This page will walk you through installing software for the
`Get Started With Git`_ tutorial  on your Windows computer.

Install Babun
-------------

Babun_ is a Windows shell that comes bundled with a whole bunch of useful
features, including Git, Zsh_, and `oh-my-zsh`_.
It's the simplest way to get a Unix-style development environment
up and running on Windows.

`Download Babun`_ and run the `.exe` file to install it. Babun integrates with
the Windows Start menu, so you can search for "babun" in the Start menu to
run it and open a new command line.
(Do *not* use ``cmd.exe``, use Babun instead!)

Install Atom
------------

You'll need a text editor to use Git effectively, and Atom_ is an
excellent choice. Download the latest stable release from the website and
run the `.exe` file to install it. Atom also integrates with the Windows Start
menu, so you can search for "Atom" in the Start menu to run it and open a new
editor window.

Next, we need to tell Git how to find and use Atom. First, verify that you can
run Atom from the command line, like this:

.. code-block:: bash

    $ atom

That should launch a new Atom window. If it does, you can teach Git about this
``atom`` command by running this command:

.. code-block:: bash

    $ git config --global core.editor "atom --wait"

Check that it worked by asking Git what the "core.editor" config value is:

.. code-block:: bash

    $ git config core.editor
    atom --wait

If you're unable to run Atom from the command line, you may have have hit
`issue 11756`_, which you can resolve by editing the ``atom.sh`` file to remove
the ``-W`` flag. Alternatively, you can install a different text editor.

Install Sublime Text
--------------------

`Sublime Text`_ is also a good text editor, and it's a good second choice if
you can't get Atom to work. (Note that you only need *one* text editor, so
if Atom is working for you, then you can skip this entire section!) Sublime
Text isn't free, but it has an unlimited free trial -- legally, you're supposed
to buy a license if you decide you want to use it actively.

`Download Sublime Text`_ and install it. You should use version 3,
not version 2. Sublime Text also integrates with the Windows Start menu,
so you can search for "Sublime Text" in the Start menu to
run it and open a new editor window.

Next, we need to tell Git how to find and use Sublime Text.
First, verify that you can run Sublime Text from the command line, like this:

.. code-block:: bash

    $ subl

That should launch a new Sublime Text window.
If it does, you can teach Git about this ``subl`` command
by running this command:

.. code-block:: bash

    $ git config --global core.editor "subl --wait"

Check that it worked by asking Git what the "core.editor" config value is:

.. code-block:: bash

    $ git config core.editor
    subl --wait

If not, `check this StackOverflow question for assistance
<https://stackoverflow.com/questions/8951275/how-can-i-make-sublime-text-the-default-editor-for-git>`_.


.. _Get Started With Git: https://us.pycon.org/2016/schedule/presentation/1620/
.. _Atom: https://atom.io/
.. _Zsh: http://www.zsh.org/
.. _oh-my-zsh: http://ohmyz.sh/
.. _Babun: https://babun.github.io/
.. _Download Babun: http://projects.reficio.org/babun/download
.. _issue 11756: https://github.com/atom/atom/issues/11756
.. _Sublime Text: https://sublimetext.com/
.. _Download Sublime Text: https://sublimetext.com/3
