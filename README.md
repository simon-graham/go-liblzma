# go-liblzma
Go bindings for XZ Utils/liblzma

This fork adds a statically compiled version of https://tukaani.org/xz/xz-5.2.5.tar.gz. This is a little bit more convenient when using in docker, CI, etc where you don't want to worry about installing any extra dependencies.
It was compiled using:

```bash
mkdir install_dir
./configure --disable-shared --disable-xz --disable-xzdec --disable-lzmadec --disable-lzmainfo --disable-lzma-links --disable-scripts --disable-doc --prefix=$(pwd)/install_dir
```

Libraries are included for linux/amd64 and darwin/amd64.

liblzma is in the public domain. See https://git.tukaani.org/?p=xz.git;a=blob;f=COPYING
