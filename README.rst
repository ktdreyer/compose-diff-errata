``compose-diff-errata`` - Compare builds in a compose to an ET advisory
=======================================================================

A tool to compare the list of builds in an ET advisory to the list of builds
in a `pungi <https://pagure.io/pungi/>`_ compose.

Use this to determine if you should add or remove builds from an advisory.

Example
-------

Ensure you have a Kerberos credential, and then run ``compose-diff-errata``::

    kinit kdreyer@REDHAT.COM

    compose-diff-errata http://example.com/MYCOMPOSE-1234.t.0/ 12345

"+" lines are builds in the advisory and not in the compose

"-" lines are builds in the compose and not in the advisory
