About Crypt
=========

A simple OSX desktop app for encrypting and decrypting files and folders which uses AES 256bit encryption in CBC mode and an open file format that can be decrypted on any platform using openssl. Internationalized for english, french and german.


Technical details
---------------------

All encryption and folder archiving are done by running a task which calls a command line script within the app wrapper (scripts/crypt3.sh) which uses tar, gzip and openssl. This means you can use that shell script on any platform to encrypt/decrypt these files.

A short suffix that is a hash of the encrypting password is included in the encrypted file suffix. This is long enough to use to effectively verify the password (so you don't decrypt to random data by entering the wrong password) but short enough not to greatly reduce the encryption strength.


Dependencies
-----------------

The openssl folder contains a precompiled version of openssl, libssl and libcrypto. If your goal is to verify the build (a good idea) you'll want to compile those yourself.


History
---------

I sold this app for a number of years but after reading about the unethical and criminal blanket civilian surveillance activities of various malicious government sponsored agencies, I've decided to make the it free and open source. I hope you find it useful.

- Steve
