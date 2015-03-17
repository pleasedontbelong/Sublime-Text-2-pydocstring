Sublime-Text-2-pydocstring
==========================

a Sublime Text 2 plugin to automatic generate docstring for module/class/function

docstring.py
============

docstring.py is a python docstring plugin, you can use this plugin to generate docstring
for the module, class or function automatically.

Output
------
Module
```python
# -*- coding: utf-8 -*-
'''
Created on 2015-03-17 12:29
@summary: My super module
@author: pablo
'''
```

Method / function
```python
def my_method(self, param1):
    """
    :param param1: Something
    :type param1: String
    :return : Some magic stuff
    Takes a param and magically turns it into a magic pink poney
    """
```

Installation
------------
Copy **[docstring.py](https://github.com/JerryKwan/Sublime-Text-2-pydocstring/blob/master/docstring.py)** into
your ST2 User packages folder *(Sublime Text 2 > Preferences > Browse Packages... > User)*

Usage
-----
Click on the position you want to generate docstring, but do not select anything, you could
define key bindings or menu entries to use this plugin easy and quick

I've added this to my User Key Bindings:

     {"keys": ["ctrl+alt+s"], "command": "docstring"}

...and this to Context.sublime-menu, which allow context menu access:

     { "command": "docstring", "caption": "Generate Docstring"}
