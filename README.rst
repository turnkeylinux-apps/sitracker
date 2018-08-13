SiT! - Support Incident Tracker
===============================

`SiT!`_ Support Incident Tracker is a help desk web application that
helps track technical support requests, contacts, sites, support
contracts and support incidents in one place. Send emails directly from
SiT!, attach files and record every communication in the incident log.
SiT is aware of Service Level Agreements and flags incidents that stray
outside them.

This appliance includes all the standard features in `TurnKey Core`_,
and on top of that:

- SiT! Support Incident Tracker configurations:
   
   - Installed from upstream source code to /var/www/sitracker

     **Security note**: Updates to SiT! Support Incident Tracker may
     require supervision so they **ARE NOT** configured to install
     automatically. See `SiT upgrade documentation`_ for upgrading.


- SSL support out of the box.
- `Adminer`_ administration frontend for MySQL (listening on port
  12322 - uses SSL).
- Postfix MTA (bound to localhost) to allow sending of email (e.g.,
  password recovery).
- Webmin modules for configuring Apache2, PHP, MySQL and Postfix.

Credentials *(passwords set at first boot)*
-------------------------------------------

-  Webmin, SSH, MySQL: username **root**
-  Adminer: username **adminer**
-  SiTracker: username is email set on first boot


.. _SiT!: https://sitracker.org/
.. _TurnKey Core: https://www.turnkeylinux.org/core
.. _`http://bugs.sitracker.org/view.php?id=1746`: http://bugs.sitracker.org/view.php?id=1746
.. _SiT upgrade documentation: https://github.com/sitracker/sitracker/blob/master/doc/UPGRADE
.. _Adminer: https://www.adminer.org/
