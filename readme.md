install:

```
   git clone git@github.com:laixintao/python3.9-import-test.git
   cd import_test
   # create your virtualenv...
   # then:
   pip install -e .
   cd ..
   python
   >>> import import_test
```

You will see different behaviour of Python3.9.0 and Python3.9.6
   

test:

in python3.9.0 :

```python
Python 3.9.0 (default, Apr 12 2021, 01:43:53)
[Clang 12.0.0 (clang-1200.0.32.29)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import import_test
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  File "/Users/xintao.lai/Downloads/import_test/__init__.py", line 1, in <module>
    from foo import text
ModuleNotFoundError: No module named 'foo'
```

in python3.9.6 :

``` python
Python 3.9.6 (default, Sep  2 2021, 16:40:58)
[Clang 12.0.5 (clang-1205.0.22.11)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import import_test
asdf
```
