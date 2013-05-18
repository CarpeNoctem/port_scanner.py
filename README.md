port_scanner.py
===============

Simple multi-threaded port scanner that I wrote for myself as an exercise in Python sockets and threading.

TODO:
* Fix issue with worker division sometimes not being accurate
* Catch SIGTERM and kill all children
* Further optimizations/cleanup?

```
CarpeNoctem@github:~$ ./port_scanner.py --help
Usage: port_scanner.py [options] hostname low_port [high_port]

Scan port range (low_port - high_port) on hostname.

Options:
  -h, --help            show this help message and exit
  -t SECS, --timeout=SECS
                        connection timeout, in seconds. default 0.2
  -n THREADS, --threads=THREADS
                        number of threads to use. default 1.
  -v, --verbose         increase verbosity.
```
