Cryptbit development tree

Cryptbit is a PoS-based cryptocurrency.

CBIT is dependent upon an older version of libsecp256k1 by sipa, the sources for which can be found here:
https://github.com/bitcoin/secp256k1

To fetch and set the version that will build without errors. Do the following before building:

$ git clone  https://github.com/bitcoin/secp256k1.git 
$ cd secp256k1
$ git reset --hard a1d5ae1527240d81ef38af42942db7e4357c9ae4

Then when building cryptbitd remember to set the following
variables if the library is not in a default path.

$ export SECP256K1_INCLUDE_PATH=your_path_here/include
$ export SECP256K1_LIB_PATH=your_path_here/lib









