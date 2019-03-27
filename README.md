# spart
A user-oriented partition info command for slurm.

Slurm does not contains a command to show user-oriented partition info. I wrote a command. I hope you will find it useful. 

# Usage
The spart command does not have any parameters.:

$ spart
       QUEUE     FREE    TOTAL     FREE    TOTAL RESOURCE    OTHER   MIN   MAX  MAXJOBTIME   CORES    NODE
   PARTITION    CORES    CORES    NODES    NODES  PENDING  PENDING NODES NODES   DAY-HR:MN PERNODE  MEM(GB)
        defq      448     2436       16       87        0        0     1     -     7-00:00      28     128
      shortq      588     2604       21       93        0        0     1     2     0-01:00      28     128
       longq       96      336        4       14        0        0     1     -    21-00:00      24      64
        gpuq       84      112        3        4        0        0     1     -     7-00:00      28     128
     bigmemq      252      280        9       10        0        0     1     -     7-00:00      28     512
       b224q      560     2548       20       91        0        0     8    40     1-00:00      28     128
     core40q      480     1400       12       35      900        0     1     -     7-00:00      40     192
         all     1164     4340       37      142        0        0     1     -    NO-LIMIT      24      64
         
 # Compiling
 gcc -lslurm spart.c -o spart
 

