========================
Team and repository tags
========================

.. image:: http://governance.openstack.org/badges/deb-python-traceback2.svg
    :target: http://governance.openstack.org/reference/tags/index.html

.. Change things from this point on

A backport of traceback to older supported Pythons.

 >>> import traceback2 as traceback

Profit.

Things to be aware of!

In Python 2.x, unlike traceback, traceback2 creates unicode output (because it
depends on the linecache2 module).

Exception frame clearing silently does nothing if the interpreter in use does
not support it.

traceback2._some_str, which while not an official API is so old its likely in
use behaves similarly to the Python3 version - objects where unicode(obj) fails
but str(object) works will be shown as b'thestrvaluerepr'.
