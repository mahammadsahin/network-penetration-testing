# 3 Upgrading Non-Interactive Shells
Linux
-----

*   `cat /etc/shells` - if present bash  or bone shell
    *   `/bin/bash -i` - get bash interactive shell - bash shell
    *   `/bin/sh -i` - get bash interactive shell - bone shell
*   `python --version` - if python is installed
    *   `python -c ‘import pty; pty.spawn("/bin/bash")’` - get bash interactive shell through python
*   `Perl --help`
    *   `perl -e ‘exec “/bin/bash”;’`
*   `ruby: exec “/bin/bash”`
*   metasploit
    *   `msfvnom` - create payload 
    *   send payload to the target system & get `meterpreter` she
*   then check environment variable - `env`
*   `export PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin` - run it when the actual _**path environment variable**_ that is used to specify the default path that will be used to search for a binary when you type in a command is not specified
*   `export TERM=xterm`
*   `export SHELL=bash`