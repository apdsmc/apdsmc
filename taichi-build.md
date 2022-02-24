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
- clang (>11 <12, on macos)
- xcode commandline
```
brew install llvm@11
xcode-select --install
```

## Build

```
python setup.py develop --user
```

## Reference

1. https://docs.taichi.graphics/lang/articles/contribution/dev_install
