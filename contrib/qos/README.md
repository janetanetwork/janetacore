### Qos ###

This is a Linux bash script that will set up tc to limit the outgoing bandwidth for connections to the Janetacoin network. It limits outbound TCP traffic with a source or destination port of 1960, but not if the destination IP is within a LAN (defined as 192.168.x.x).

This means one can have an always-on litecoind instance running, and another local litecoind/janetacoin-qt instance which connects to this node and receives blocks from it.
