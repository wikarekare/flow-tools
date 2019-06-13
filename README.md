#Flow Tools

Forked to add format25 and format26 (json version of format 25) to flow-print
Format25: Tab separated
  Start End Sif SrcIPaddress SrcPort DIf DstIPaddress DstPort Protocol Flags tos Pkts Octets sAS dAS
Start and End dates in YYYY-MM-DD HH:MM:SS.ms

```
Format26: Json array of hashes. 
   [
     {  "start": "YYYY-MM-DD HH:MM:SS.ms",
         "end": "YYYY-MM-DD HH:MM:SS.ms",
         "srcIf": "x",
         "srcIPaddress": "x.x.x.x",
         "srcPort": "x", 
         "dstIf": "x", 
         "dstIPaddress": "x.x.x.x",
         "dstPort": "x",
         "protocol": "x",
         "flags": "x",
         "tos": "x", 
         "pkts": "x",
         "octets": "x",
         "srcAS": "xx",
         "dstAS": "xx" 
       },
     ...
  ]
```

flow-tools is a set of programs for processing and managing NetFlow exports
from Cisco and Juniper routers.  The software was originally written by
Mark Fullmer while working at Ohio State University.  Steve Romig and the
OSU network security group have added documentation, functionality, and
provided feedback.  OARnet and the Ohio ITEC have recently funded my
time to add version 8 PDU support and various other features.

For installation notes and a quick start please see INSTALL.

If you are using flow-tools please subscribe to the mailing list by
sending a message to flow-tools-request@splintered.net

flow-tools is currently available at http://www.splintered.net/sw/flow-tools

Mark Fullmer
maf@splintered.net

## install

```
autoreconf --install --force
./configure
make
make install
```


