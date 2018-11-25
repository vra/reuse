.. reuse documentation master file, created by
   sphinx-quickstart on Thu Nov 22 15:46:10 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to reuse's documentation!
=================================
reuse is a collection of useful python functions in you work.

Here is a demo about how to use reuse: `demo`_.

.. _demo: https://asciinema.org/a/m0fEneiY03JwiEzc20ERG99Vl


Installation
------------
.. code-block:: python

   pip3 install --user py-reuse

Examples
--------

.. doctest::

   >>> import reuse as rs
   >>> rs.check_exists('/etc/apt/source.lists')
   False
   >>> rs.check_exists('/etc/apt')
   True
   >>> rs.concat_path(['/home', 'user', 'project'])
   '/home/user/project'
   >>> rs.create_dir_if_not_exist('./tmp-dir/test')
   >>> ll = [[1,2], [3,4], [6,7]]
   >>> rs.flat_list(ll)
   [1, 2, 3, 4, 6, 7]
   >>> rs.full_name('/etc/apt/sources.list')
   'sources.list'
   >>> rs.pure_name('/etc/apt/sources.list')
   'sources'
   >>> rs.parent_dir('/etc/apt/sources.list')
   '/etc/apt'
   >>> rs.run_cmd('ls -l')
   总用量 1068
   -rw-rw-r--  1 wang wang  15200 9月   4 20:21 00218.jpg
   -rw-rw-r--  1 wang wang  15071 9月   4 20:21 00219.jpg
   drwxrwxr-x  2 wang wang  36864 11月 22 16:49 960
   -rw-rw-r--  1 wang wang   5496 11月 25 16:07 A.odf
   -rw-rw-r--  1 wang wang   1380 11月 22 16:40 a.txt
   drwxrwxr-x  2 wang wang   4096 7月  14 09:05 bin
   -rw-rw-r--  1 wang wang   5358 11月 25 16:08 B.odf
   drwxrwxr-x  3 wang wang   4096 11月 10 13:19 cpp-test
   drwxrwxr-x  2 wang wang   4096 11月 19 11:54 diff_masks
   drwxr-xr-x  2 wang wang  40960 11月 15 18:44 dp
   drwxrwxr-x  6 wang wang  61440 11月 19 17:32 dy4
   drwxrwxr-x  2 wang wang  69632 11月 18 22:48 dy4_1G
   drwxr-xr-x  2 wang wang   4096 11月 20 13:04 epoch-500
   drwxrwxr-x  7 wang wang   4096 11月 18 09:22 FlameGraph
   drwxrwxr-x  4 wang wang   4096 11月 23 23:56 go
   -rw-rw-r--  1 wang wang     14 11月 23 00:17 hello.txt
   -rw-rw-r--  1 wang wang 309348 11月 20 10:34 img1_kp_50.png
   drwxrwxr-x  3 wang wang   4096 7月  14 09:05 opt
   -rw-rw-r--  1 wang wang 383100 11月 20 19:53 ORB.png
   -rw-rw-r--  1 wang wang    337 11月 20 21:02 ORB.py
   drwxrwxr-x  2 wang wang   4096 11月 19 10:48 outputs
   -rw-rw-r--  1 wang wang     35 11月 20 10:56 project.py
   drwxrwxr-x  3 wang wang   4096 11月  1 22:05 PycharmProjects
   drwxrwxr-x 11 wang wang   4096 11月 18 09:24 pyflame
   drwxrwxr-x  4 wang wang   4096 11月 14 12:00 results
   drwxrwxr-x  2 wang wang   4096 11月 16 14:09 S001C001P008R002A060_rgb_out
   drwxrwxr-x  2 wang wang   4096 11月 16 14:05 S017C003P020R002A060
   drwxrwxr-x  2 wang wang   4096 11月 12 21:49 tmp
   drwxrwxr-x  3 wang wang   4096 11月 25 18:01 tmp-dir
   drwxrwxr-x  2 wang wang   4096 10月 26 13:49 videos
   drwxrwxr-x 12 wang wang   4096 11月 20 21:40 workspace
   drwxrwxr-x  2 wang wang  20480 11月  9 17:22 ws_1_step_8
   drwxr-xr-x  5 wang wang   4096 11月  1 20:08 视频
   drwxr-xr-x 11 wang wang   4096 11月 24 13:30 图片
   drwxr-xr-x 16 wang wang   4096 11月 12 23:29 文档
   drwxr-xr-x  7 wang wang  12288 11月 25 16:23 下载
   drwxr-xr-x  2 wang wang   4096 10月  2 09:19 桌面
   0



.. toctree::
   :maxdepth: 1
   :caption: Function APIs:

   reuse



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
