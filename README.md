# abelian

<img width="1220" alt="Capture d’écran 2024-01-14 à 12 57 46" src="https://github.com/EloWord/abelian/assets/155255722/3bbbb22d-5116-4b2a-8f71-15ce78e06785">

Version 1.8.4:

- Added support for Abelian mining with Hive Os custom flightsheet
- Added first support of mining pool :  https://www.abelpool.io/


****** Stay tuned for the next mining pool support update - coming soon! *******

|          | Links                               |
|----------------------|------------------------------------|
| <img height="40" width="160" alt="Capture d’écran 2024-01-13 à 21 03 15" src="https://github.com/EloWord/abelian/assets/155255722/c5cdd36d-6de7-4f5b-91be-e92687d4a718"> | [Abelian Website](https://www.abelian.info)   |
| <img height="40" width="160" alt="Capture d’écran 2024-01-13 à 21 29 37" src="https://github.com/EloWord/abelian/assets/155255722/ca8e33de-03a8-4c78-8dda-94009a25b69d"> | [Abelian Medium](https://pqabelian.medium.com/)  |
| <img height="40" width="160" alt="Capture d’écran 2024-01-13 à 21 38 29" src="https://github.com/EloWord/abelian/assets/155255722/fe980c7f-db9d-4607-8dd3-1f822c13ba3b"> | [Mining pool](https://www.abelpool.io)    |
| <img height="40" width="160" alt="Capture d’écran 2024-01-10 à 01 45 22" src="https://github.com/EloWord/hiveos/assets/155255722/b16983a6-74cc-4256-8192-9d02f5c2bc7d">  | [Abelian Github](https://github.com/pqabelian) |
| Abelian discord  | [Abelian Discord](https://discord.gg/96hwCTds) |

<br>

## :star2: Support My Work and Contribute to its Growth :star2:

If you appreciate my work and want to contribute to its ongoing development, consider leaving a tip. Every contribution, big or small, makes a huge difference and motivates me to continue creating and improving.

**To support me, use: **


Abel:`abe138840580d95bf353322f05b4fa1995d3af6448af3d57cd2592598d9364fdca1fdcfa5a3cfa35ee88a6f4140cc543c49660c3446f58a25fdeec459738fddd9db6`


Qubic: `HJDQLJOMSLGVWAVBWUTRCYPFICUAWTLUBKXLQXOJLBIKTGLRAGQHPDODPQNB`

*Support received since this version: 6,000,000 Qubic - Thank you for your future support!*

[<img src="https://github.com/EloWord/hiveos/assets/155255722/dedb996d-c517-4059-a55a-d9adea9a21f1" alt="discord" width="200">](https://discord.gg/uPP8R6ku)

Thank you for being part of this journey!
<br>

## :warning: Mandatory Installation Instructions and settings 

- Hive OS beta (Ubuntu 20.04) 
`hive-replace --list`  (choice 2/ yes to apply -- better to start this fresh install if you'r stuck)
- GLIBC >=2.34 (updated 11/01/2024)
```apt update && apt upgrade && echo "deb http://cz.archive.ubuntu.com/ubuntu jammy main" >> /etc/apt/sources.list && apt update && apt install tmux -y && sudo apt install libc6 -y ```
<br>

## :wrench: Settings

- this version is tested on `https://www.abelpool.io` soon other pools will be supported

- it's a gpu custom miner nvidia/amd, check out the example flightsheets below for seamless setup :
https://github.com/EloWord/abelian/releases/download/v1.8.4abel/eloword-v1.8.4abelfix3.tar.gz

- Drop in the flightsheet the pool command line juste like that:
```"abelian":"curl -sSL  https://download.abelpool.io/cmd_global/allinone_ctl.sh  | bash -s start  YOUROWNTOKEN"```
<br>

## ✈️ Hive Os Flighsheet

Just drop your NVTOOL command in the `Extra config argument` box it's magic

### *** GPU Flightsheet - including Nvidia OverClocks ***

Extra config arguments exemple:
```
nvtool --setcoreoffset 200 --setclocks 2000 --setmem 0
"abelian":"curl -sSL  https://download.abelpool.io/cmd_global/allinone_ctl.sh  | bash -s start  YOUROWNTOKEN"
```

<img width="672" alt="Capture d’écran 2024-01-13 à 19 52 17" src="https://github.com/EloWord/abelian/assets/155255722/42e928a5-717f-4f3b-a7de-e1fe11b35604">

### *** GPU Flightsheet - No OverClocks ***

Extra config arguments exemple:

```
"abelian":"curl -sSL  https://download.abelpool.io/cmd_global/allinone_ctl.sh  | bash -s start  YOUROWNTOKEN"
```

<img width="670" alt="Capture d’écran 2024-01-13 à 19 37 40" src="https://github.com/EloWord/abelian/assets/155255722/3c1d8a61-4f6a-41f2-9b53-e2ebb8997689">

