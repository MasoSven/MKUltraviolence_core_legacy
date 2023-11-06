# MKUltraviolence's legacy core
Source code for the MKUltraviolence legacy core project, a fork of Hellcore and LambdaMOO.

## Recommendations

* Use Debian 12

## Dependencies:

* autoconf
* automake
* bison
* gcc
* gperf
* libstdc++
* make
* sed

If you are unable to build despite having working and recent versions of these
installed, please file a bug report on this repository. If i'm able to i'll try to resolve it.

### Building

Simply run (out of date; use the later one
```shell
./build.sh
```
```shell
su  {enter your shit}
apt install git
cd /home/YOURUSERNAME/
git clone https://github.com/MasoSven/MKUltraviolence_core_legacy.git
chown -R root MKUltraviolence_core_legacy/
chmod -R 0777 MKUltraviolence_core_legacy/
cd /home/YOURUSERNAME/MKUltraviolence_core_legacy/
apt install gcc
apt install bison
apt install autoconf
apt install automake
apt install make
apt install gperf
./autogen.sh
MAKE="gmake" ./configure
make
cd /src
./moo -l moo.log ../NAMEOFYOURDBFILE ../NAMEOFNEWDBFILE 7777
```


The moo binary will be located as `src/moo`.

## Executing

This is a Fork and archive of Necantropes 2010 Hellcore trying to run our remake, we're working on ommiting it.

Before you start the server, read the section on building it.

To start it, you can run
```shell
./restart hellcore
```

You can also start it with something like this:
```shell
./moo -l moo.log hellcore.db hell.db.test 7777
```

```
(./moo -l <logfile> <original DB> <new DB> <port>)
```

You should be able to login with 'connect Wizard', then change your password.

### USE AT YOUR OWN RISK. I DENY RESPONSIBILITY FOR:
* Spontaneous hairy nose
* Micropenis
* Liver vs pancreas internal war
* Making baby Jesus retch
* Getting on the No-Fly list
* Lizard people living under the Appalachian Mountains following you around

Cheers,

Sven Maso
