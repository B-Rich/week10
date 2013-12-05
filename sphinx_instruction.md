How to set up Sphinx
====================


Installation
------------

* Install with `pip install sphinx` or `easy_install sphinx`, or
apt-get, macports...
* In your project folder, you should have something like this:
  
  ~~~
  ]$ ls
  source/ README.md TODO.md
  ~~~

  Create a documentation folder
  ~~~
  ]$ mkdir documentation
  ~~~

  And use the automatic tool for generating documentation
  ~~~
  ]$ sphinx-apidoc -F -o documentation -H MyProject -A "Me Myself" source 
  ~~~
* Modify things to your taste in `documentation`:
  * in conf.py, make sure to append the path of your python source
    code
  * you can select the theme, colors, options (automodule, etc...)
* compile with `make html`, and open `_build/html/index.html`. Et
  voila !
