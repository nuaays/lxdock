lxdock status
=============

**Command:** ``lxdock status [name [name ...]]``

This command can be used to show the statuses of the containers of your project.

By default this command will display the statuses of all the containers of your project but you can
limit this operation to some specific containers by specifying their names. The statuses that are
returned by this command can be ``not-created``, ``stopped`` or ``running``.

Options
-------

* ``[name [name ...]]`` - zero, one or more container names

Examples
--------

.. code-block:: console

  $ lxdock status               # shows the statuses of all the containers of the project
  $ lxdock status mycontainer   # shows the status of the "mycontainer" container
  $ lxdock status web ci        # shows the statuses of the "web" and "ci" containers
