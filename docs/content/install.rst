Installation
============

.. _install:

Centrifuge was developed and tested on Linux and Mac OS X operating systems. The work on
other systems is not guaranteed. On windows Centrifuge works with Memory Engine only.

It is written in Python. Python 2.6, 2.7, 3.3, 3.4 supported.

You can find nice guide about how to install Python on Mac OS X or Linux
`here <https://python-guide.readthedocs.org/en/latest/starting/install/osx/>`_ and
`here <https://python-guide.readthedocs.org/en/latest/starting/install/linux/>`_ respectively

To isolate Centrifuge environment it is recommended to use virtualenv.
If you are not familiar with it yet - please, make time and read about it
`here <https://python-guide.readthedocs.org/en/latest/dev/virtualenvs/>`_

.. code-block:: bash

    virtualenv --no-site-packages centrifuge/env
    . centrifuge/env/bin/activate


On Python 3 make sure you have `pip` installed:

.. code-block:: bash

    curl -O http://python-distribute.org/distribute_setup.py
    python distribute_setup.py
    easy_install pip


.. code-block:: bash

    pip install centrifuge


Now you can run centrifuge:

.. code-block:: bash

    centrifuge --config=config.json


We will talk about configuration file later in documentation.

Btw, you can speed up Centrifuge using 'ujson' module. As Centrifuge works a lot
with JSON data - you can install `ujson` module to improve performance significantly.
`pip install ujson` will do the work. This step is optional as Centrifuge uses
built-in `json` module if no `ujson` available.
