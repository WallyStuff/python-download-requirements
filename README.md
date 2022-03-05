# Python download requirements

Simple script to port a Python 3.9 environment in a machine without network access.

With internet access run `run.ps1` to create directory `deps` with all packages.

Copy `deps` directory to target machine for running installation.

On target machine with exactly the same Python version used for download run:

```
pip install -r requirements-prod.txt --no-index --find-links deps
```

All should be fine by now!
