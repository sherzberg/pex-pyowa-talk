
```
$ pex . -e example:greet -v
  example==0.0.1 -> example 0.0.1stributions :: Packaging example
pex: Building pex: 526.5ms                                       
pex:   Resolving distributions: 299.0ms
pex:       Packaging example: 273.8ms
Running PEX file at /tmp/tmpqlkSid with args []
pex: PEX.run invoking /usr/bin/python2.7 /tmp/tmpqlkSid
hi thereroot
```

```
$ pex . -e example:greet -v --no-wheel
  example==0.0.1 -> example 0.0.1stributions :: Packaging example
pex: Building pex: 492.7ms                                       
pex:   Resolving distributions: 268.0ms
pex:       Packaging example: 244.9ms
Running PEX file at /tmp/tmpwRH47X with args []
pex: PEX.run invoking /usr/bin/python2.7 /tmp/tmpwRH47X
hi there root

