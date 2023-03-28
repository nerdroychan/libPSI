# libPSI
A repository for private set intersection. Most protocols were written just for benchmarking them while (RR17,KKRT,Mea86=ECDH) can be run from the command line and take a file as input. Run the program for details. 

## VolePSI
Also consider using https://github.com/Visa-Research/volepsi/ for improved performance.

## Introduction
Protocols:

 * Malicious Secure [RR17](https://eprint.iacr.org/2017/769) based on simple hashing and OTs (fastest)
 * Malicious Secure [RR16](https://eprint.iacr.org/2016/746) based on Bloom filters and OTs
 * Malicious Secure [DKT10](https://eprint.iacr.org/2010/469) based on public key crypto (ECC)
 * Semi-Honest Secure [KKRT16](https://eprint.iacr.org/2016/799) based on cuckoo hashing and OTs (fastest)
 * Semi-Honest Secure [Mea86](http://ieeexplore.ieee.org/document/6234849/) base on public key crypto (ECC)
 * Semi-Honest Secure [DRRT18](https://eprint.iacr.org/2018/579.pdf) based on cuckoo hashing, PIR and OTs (fastest unbalanced)
 
## Install (Use makefile)

```
git clone https://github.com/nerdneilsfield/libPSI
cd libPSI

# compile
make 

# test
make test_all

# clean
make clean

# format code
make format
```


## Install (OLD)

Our library is cross platform and has been tested on both Windows and Linux. The library should work on Mac but it has not been tested. There are several library dependencies including [libOTe](https://github.com/osu-crypto/libOte). 


```
git clone https://github.com/osu-crypto/libPSI.git
cd libPSI
python build.py
```

Unit tests can be run by executing the program.

```
/out/build/<platform>/frontend/frontend.exe -u
```
Other options can be seen by executing with no arguments.
## Help

Contact Peter Rindal `peterrindal@gmail.com` for any assistance on building or running the library.
