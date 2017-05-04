Compatibility
-------------
On May 4, 2017, Optimizely sent out a notice regarding a change in the
format of the raw dumps.  As of this date, the described updates have
not been made to this tool.  See `compat.txt` for more detail.

Dependencies
------------
- Python 3, and Pip for Python 3 ("`pip3`").
- Contents of `requirements.txt`.

Setup
-----

    python3 -m venv venv/optimizely-export
    source venv/optimizely-export/bin/activate
    pip3 install -r requirements.txt

Teardown
--------

    deactivate
    rm -R venv

Usage
-----
Set up S3 credentials according to [boto3's documentation][1], or pass
the `-i` argument when invoking `optimizely-export` to interactively
provide them.

Invoke `optimizely-export`.  Pass the `-h` option to get a fuller
description and explanation of options and arguments.

TODO
----
- Update for new Optimizely raw dump formatting (see "Compatibility",
  above).

Future Work
-----------
- Distribute on PyPI?

References
----------
- [boto3 Credential Setup][1]
- [Optimizely Data Export Guide][2]

[1]: http://boto3.readthedocs.io/en/latest/guide/configuration.html#credentials
[2]: https://developers.optimizely.com/classic/events/export/index.html
