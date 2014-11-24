A backport of traceback to older supported Pythons.

 >>> import traceback2 as traceback

Profit.

Things to be aware of!

In Python 2.x, unlike traceback, traceback2 creates unicode output.

Exception frame clearing silently does nothing if the interpreter in use does
not support it.
