# Build Taichi from source code

## clone
```
git clone --recursive https://github.com/taichi-dev/taichi.git
```

## requirements:

- python (3.6~3.9), work with conda
```
conda create -n ti python=3.9

cond activate ti

pip install -r requirements_dev.txt
```
- llvm (only 10.0), cannot install by homebrew, 
- clang (>11, on macos)
```
brew install llvm@12
brew uninstall --ignore-dependencies python@3.9

```

## Build

```
mkdir build; cd build
cmake -DCMAKE_CXX_COMPILER=/usr/local/opt/llvm@12/bin/clang ..
make -j 32

```
