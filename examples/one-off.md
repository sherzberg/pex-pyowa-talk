# one-off

```
$ pex inflect -v
  inflect -> inflect 2.1.0ving distributions
pex: Building pex: 87.3ms                   
pex:   Resolving distributions: 79.9ms
Running PEX file at /tmp/tmppNAaQv with args []
pex: PEX.run invoking /usr/bin/python2.7 /tmp/tmppNAaQv
Python 2.7.12 (default, Dec  4 2017, 14:50:18) 
[GCC 5.4.0 20160609] on linux2
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole
```

```
$ pex --python=python3 inflect -v
  inflect -> inflect 2.1.0ving distributions
pex: Building pex: 378.8ms                  
pex:   Resolving distributions: 137.6ms
Running PEX file at /tmp/tmpdZqKT3 with args []
pex: PEX.run invoking /usr/bin/python3.5 /tmp/tmpdZqKT3
Python 3.5.2 (default, Nov 23 2017, 16:37:01) 
[GCC 5.4.0 20160609] on linux
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)
```

```
$ pex inflect
Python 2.7.12 (default, Dec  4 2017, 14:50:18) 
[GCC 5.4.0 20160609] on linux2
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)
>>> import inflect
>>> p = inflect.engine()
>>> p.plural('boat')
u'boats'
>>> p.number_to_words(12345)
u'twelve thousand, three hundred and forty-five'
```

```
$ pex flask -- app.py
 * Serving Flask app "__main__" (lazy loading)
 * Environment: production
   WARNING: Do not use the development server in a production environment.
   Use a production WSGI server instead.
 * Debug mode: off
 * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
```
