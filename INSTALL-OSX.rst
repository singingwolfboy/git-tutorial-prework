Installation for OS X
=====================

This page will walk you through installing software for the
`Get Started With Git`_ tutorial  on your OS X computer. Using the Homebrew_
package manager is *strongly* recommended, but if you want to install the
required software without using a package manager, you can do so.

Install Homebrew
----------------

Homebrew_ is a `package manager`_ for OS X, and it makes it easy to install,
update, and uninstall software on your computer. To install Homebrew, first
`install the XCode app`_ from the Mac App Store. Then go to the Homebrew_
website and follow the instructions on the page to install it.

Once Homebrew is installed, you will be able to use the ``brew`` command. You
can run the following command to test:

.. code-block:: bash

    $ which brew
    /usr/local/bin/brew

Once you are able to use the ``brew`` command, run the following command to
check your system:

.. code-block:: bash

    $ brew doctor

Install Git
-----------

Once you have Homebrew installed, installing Git is easy!

.. code-block:: bash

    $ brew install git

That will install the latest version of Git to ``/usr/local/bin/git``.
Check to be sure that you are using the version of Git that Homebrew installed:

.. code-block:: bash

    $ which git
    /usr/local/bin/git

If you get ``/usr/bin/git`` instead, you should modify your ``$PATH`` variable
to put ``/usr/local/bin`` in front of ``/usr/bin``. If you're not sure how to
do that, simply install Zsh_ and oh-my-zsh_ at the end of this install guide.

Install Atom
------------

You'll need a text editor to use Git effectively, and `Atom`_ is an
excellent choice. We can use `Homebrew Cask`_ to install it, like this:

.. code-block:: bash

    $ brew tap caskroom/cask
    $ brew cask install atom

Homebrew will install Atom to the "Applications" folder in your home directory.
For example, if you use the account "Steve" on your computer, then Atom will be
installed to ``/Users/Steve/Applications/Atom.app``. You can drag that icon
to your Dock, so that it's easer to open in the future.

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

Install Zsh (optional)
----------------------

Zsh_ is a shell for your command line, and `oh-my-zsh`_ is a framework for
installing themes and plugins for that shell. You don't need to install these
things, but they make it easier to keep track of where you are and what you're
doing when you use Git.

With Homebrew, installing Zsh_ is a breeze:

.. code-block:: bash

    $ brew install zsh

Then install `oh-my-zsh`_ by following the directions on the homepage:

.. code-block:: bash

    $ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

Open a new command line window, and verify that it looks different -- and
probably a lot nicer! If you don't like the way it looks, you can edit the
``.zshrc`` file in your home directory and pick a different theme.

You're all done!


.. _Get Started With Git: https://us.pycon.org/2016/schedule/presentation/1620/
.. _install the XCode app: https://itunes.apple.com/us/app/xcode/id497799835
.. _Homebrew: http://brew.sh/
.. _Homebrew Cask: http://caskroom.io/
.. _package manager: https://en.wikipedia.org/wiki/Package_manager
.. _Atom: https://atom.io/
.. _Zsh: http://www.zsh.org/
.. _oh-my-zsh: http://ohmyz.sh/
