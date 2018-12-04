# pex'd tools

```
$ pex speedtest-cli -o st.pex -v
  speedtest-cli -> speedtest-cli 2.0.2utions
pex: Building pex: 206.4ms                  
pex:   Resolving distributions: 199.0ms
Saving PEX file to st.pe

$ ls -lahs st.pex
448K -rwxr-xr-x 1 root 448K Dec  4 04:40 st.pe
```

```
$ python st.pex
Python 2.7.12 (default, Dec  4 2017, 14:50:18) 
[GCC 5.4.0 20160609] on linux2
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)
>>> import speedtest
>>> speedtest()
Traceback (most recent call last):
  File "<console>", line 1, in <module>
TypeError: 'module' object is not callable
>>> speedtest.main()
Retrieving speedtest.net configuration...
Testing from Digital Ocean (XXX)...
Retrieving speedtest.net server list...
Selecting best server based on ping...
Hosted by AT&T (New York City, NY) [17.50 km]: 5.524 ms
Testing download speed................................................................................
Download: 492.54 Mbit/s
Testing upload speed................................................................................................
Upload: 344.92 Mbit/s
```

```
$ pex speedtest-cli -o st.pex -e speedtest:main -v
  speedtest-cli -> speedtest-cli 2.0.2utions
pex: Building pex: 66.8ms                   
pex:   Resolving distributions: 58.8ms
Saving PEX file to st.pex

$ python st.pex
Retrieving speedtest.net configuration...
Testing from Digital Ocean (XXX)...
Retrieving speedtest.net server list...
Selecting best server based on ping...
Hosted by QTS Data Centers (Jersey City, NJ) [12.85 km]: 9.198 ms
Testing download speed................................................................................
Download: 583.54 Mbit/s
Testing upload speed................................................................................................
Upload: 271.39 Mbit/s
```

```
$ chmod +x st.pex 

$ ./st.pex
Retrieving speedtest.net configuration...
Testing from Digital Ocean (XXX)...
Retrieving speedtest.net server list...
Selecting best server based on ping...
Hosted by QTS Data Centers (Jersey City, NJ) [12.85 km]: 4.53 ms
Testing download speed................................................................................
Download: 899.82 Mbit/s
Testing upload speed................................................................................................
Upload: 699.07 Mbit/s
```


