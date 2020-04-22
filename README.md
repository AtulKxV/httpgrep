# Description

A python tool which scans for HTTP servers and finds given strings in HTTP body
and HTTP response headers.

# Usage

```
$ httpgrep -H
    __    __  __
   / /_  / /_/ /_____  ____ _________  ____
  / __ \/ __/ __/ __ \/ __ `/ ___/ _ \/ __ \
 / / / / /_/ /_/ /_/ / /_/ / /  /  __/ /_/ /
/_/ /_/\__/\__/ .___/\__, /_/   \___/ .___/
             /_/    /____/         /_/

     --== [ by nullsecurity.net ] ==--

usage

  httpgrep -h <args> -s <arg> [opts] | <misc>

opts

  -h <hosts|file>   - single host or host-range/cidr-range or file containing
                      hosts, e.g.: foobar.net, 192.168.0.1-192.168.0.254,
                      192.168.0.0/24, /tmp/hosts.txt
  -p <port>         - port to connect to (default: 80)
  -t                - use TLS/SSL to connect to service
  -u <URI>          - URI to search given strings in, e.g.: /foobar/, /foo.html
                      (default /)
  -r                - do not search given strings in http response headers
  -s <string|file>  - a single string or multile strings in a file to find in
                      given URIs, e.g. 'tomcat 8', '/tmp/igot0daysforthese.txt'
  -b <bytes>        - num bytes to read from response. offset == response[0].
                      (default: 64)
  -x <threads>      - num threads for concurrent checks (default: 50)
  -c <seconds>      - num seconds for socket timeout (default: 2.0)
  -i                - use case-insensitive search
  -v                - verbose mode (default: quiet)

misc

  -H                - print help
  -V                - print version information
```

# Author

noptrix

# Notes

- quick'n'dirty code
- httpgrep is already packaged and available for [BlackArch Linux](https://www.blackarch.org/)
- My master-branches are always stable; dev-branches are created for current work.
- All of my public stuff you find are officially announced and published via [nullsecurity.net](https://www.nullsecurity.net).

# License

Check docs/LICENSE.

# Disclaimer

We hereby emphasize, that the hacking related stuff found on
[nullsecurity.net](http://nullsecurity.net) are only for education purposes.
We are not responsible for any damages. You are responsible for your own
actions.
