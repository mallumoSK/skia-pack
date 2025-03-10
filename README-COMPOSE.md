# Compose 1.7.3

## Building locally

###
```shell
git clone --branch compose/1.7.3 https://github.com/mallumoSK/skia-pack.git && cd skia-pack
```

### OpenGL ES ARM64
```shell
sudo ./script/prepare_linux_arm.sh
```

###  OpenGL AMD64
```shell
sudo  ./script/prepare_linux.sh
```

```sh
python3 script/checkout.py --version m126-6bfb13368b
python3 script/build.py
python3 script/archive.py --version m126-6bfb13368b
```

To build a debug build:

```sh
python3 script/checkout.py --version m126-6bfb13368b
python3 script/build.py --build-type Debug
python3 script/archive.py --version m126-6bfb13368b --build-type Debug
```
