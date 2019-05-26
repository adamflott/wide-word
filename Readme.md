# wide-word

[![Build Status](https://secure.travis-ci.org/erikd/wide-word.svg?branch=master)](http://travis-ci.org/erikd/wide-word)

A Haskell library providing `Word128` and `Int128` data types with all the
standard type class instances including `Show`, `Read`, `Ord`, `Bounded`,
`Enum`, `Num`, `Bits`, `FiniteBits`, `Real`, `Integral`, `Storable` and
`NFData`.

The `Word128` type should be a drop in replacement for `Word64` unless you are
specifically relying on the rounding/overflow/truncation behaviour of `Word64`.

## Recommended Build Procedure
The recommended way to build this project is to use 'cabal new-build' as follows:
```
cabal new-configure --enable-tests
cabal new-build
cabal new-test
```
