Personal Emacs Configuration
----------------------------

Stuff I've gathered over the many years of using emacs.
A lot of the 3rd party scripts are directly copied in order to save users from hunting this across the net.


Assuming thiis cloned to ~/rdiankov-emacs-config, execute the following to setup in system:

Ubuntu:

.. code-block::

  sudo apt-get install python-mode pymacs

All:

.. code-block::

  git clone https://github.com/rdiankov/emacs-config.git $HOME/rdiankov-emacs-config
  ln -f -s $HOME/rdiankov-emacs-config/.emacs-lisp $HOME/.emacs-lisp
  ln -f -s $HOME/rdiankov-emacs-config/.emacs $HOME/.emacs
  cd $HOME/.emacs-lisp/cedet-1.1
  make EMACS=emacs
  cd $HOME/.emacs-lisp/auto-complete-1.3.1
  make install DIR=$HOME/.emacs-lisp

Can byte-compile everything in the .emacs-lisp directory to accelerate the startup by running::

  C-u 0 M-x byte-recompile-directory

  
Warning: This repository holds the emacs configuration I used everyday for my computer systems. It is not meant to be cross-platform or supported on old systems.
