Arcade-Learning-Environment
===========================

The Arcade Learning Environment (ALE) -- a platform for AI research.

See http://www.arcadelearningenvironment.org for details.


On mac, follow below to get it started:

* `cd $Arcade-Learning-Environment`
* build the binaries: `cp makefile.mac Makefile`
* create a roms directory in ALE:: `mkdir roms`
* Download ROMS from internet, e.g., [here](http://www.atarimania.com/rom_collection_archive_atari_2600_roms.html), unzip it. 
* You have a hierarcy of files like this:
``` Roms
    HARMONY CART ROMS
      1977-1992 NTSC VERSIONs ..
      Garfield.txt
      ROMS SORTED BY ALBHABET
        A-G
          3-D Tic-Tac-Toe.bin
          Acid Drop (PAL).bin
          ...
          Alien.bin
          ... 
```
* copy a sample ROM file to our $Arcade-Learning-Environment/ROMS
  `cp  ~/Downloads/Roms/HARMONY\ CART\ ROMS/ROMS\ SORTED\ BY\ ALBHABET/A-G/Alien.bin ./roms/alien.bin`
* Run ALE: 
```
./ale -player_agent random_agent ./roms/alien.bin
A.L.E: Arcade Learning Environment (version 0.4)
[Powered by Stella]
Use -help for help screen.
Game console created:
  ROM file:  ./roms/alien.bin
  Cart Name: Alien (1982) (20th Century Fox)
  Cart MD5:  f1a0a23e6464d954e3a9579c4ccd01c8
  Display Format:  AUTO-DETECT ==> NTSC
  ROM Size:        4096
  Bankswitch Type: AUTO-DETECT ==> 4K

Running ROM file...
Random Seed: Time
Game will be controlled by an internal agent.
Episode 1 ended, score: 70
Episode 2 ended, score: 100
Episode 3 ended, score: 110
Episode 4 ended, score: 90```

  
