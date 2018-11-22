# reuse
Collection of useful python functions (reuse again and again).

[![Build Status](https://travis-ci.com/vra/reuse.svg?branch=master)](https://travis-ci.com/vra/reuse)

# supported platform
 * Linux
 * python2.7 and higher
 * python3.5 and higer
 
# installation
```bash
pip3 install --user py-reuse
```

# how to use
```python
import reuse as rs

rs.check_exist('/path/to/dir') # Check if a file or directory exist
rs.create_dir_if_not_exist('/path/to/new/dir') # Create a directory only when it didn't exist
...

```
docs: <https://py-reuse.readthedocs.io>.

