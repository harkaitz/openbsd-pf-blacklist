PF-BLACKLIST
============

Blacklist for OpenBSD's PF firewall.

## Help

pf-blacklist

    Usage: pf-blacklist -v (verbose) -i (install rules)
    
    Download IP blacklist files from the internet, update pf tables
    with pfctl(8) and add the rules to pf.conf(5). The following
    blacklists are used.
    
        1. https://github.com/stamparm/ipsum
    
    To update this list daily, put the following in /etc/crontab(5):
    
        30 02 * * * root -n /usr/local/bin/pf-blacklist
        @reboot     root -n /usr/local/bin/pf-blacklist
    
    You can add additional blacklists to "/var/run/iplist/black". You
    can add the needed rules to pf.conf(5) with -i.

## Collaborating

For making bug reports, feature requests, support or consulting visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
