Package Removal Command
=======================

This document provides a handy command for removing a package from an Ubuntu system using the terminal. This is especially useful when you want to uninstall a specific application.

Usage
-----

To remove a package, open a terminal and run the following command:

.. code-block:: bash

   sudo apt remove package -y && sudo apt autoremove -y && sudo apt purge package* -y

Replace ``package`` with the actual name of the package you want to remove.

- The ``-y`` flag indicates that you want to automatically answer "yes" to any prompts for confirmation.
- The command consists of three parts:
    1. Removing the package
    2. Automatically removing any dependencies that are no longer needed
    3. Purging any residual configuration files

Examples
--------

For instance, to remove the Transmission BitTorrent client:

.. code-block:: bash

   sudo apt remove transmission-gtk -y && sudo apt autoremove -y && sudo apt purge transmission-gtk* -y

Replace ``transmission-gtk`` with the package name you want to remove.

Remember
--------

- Be cautious when using this command, as it will uninstall the specified package and its associated dependencies.
- Double-check the package name and ensure that you indeed want to remove it.

