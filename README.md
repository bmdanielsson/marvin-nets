### Overview

This repository contains NNUE networs for the [Marvin chess engine](https://github.com/bmdanielsson/marvin-chess).

### v1 nets

The v1 format uses a standard HalfKP 128x2-32-32-1 architecture. This format
is used by Marvin 5.0.0 - 5.1.0.

**net-3f7389e.nnue**
The default net for Marvin 5.0.0. If was trained using 600M positions searched
to depth 10 using Marvin 4.0.1.

**net-ca6610a.nnue**
The default net for Marvin 5.1.0. If was trained using 600M positions searched
to depth 10 using Marvin 4.0.1.

### v2 nets

The v2 format uses a standard HalfKP 128x2-32-32-1 architecture with a few
modifications. Firstly flip is used instead of rotate for symmetry and secondly
the Shogi drop piece has been removed from the input feature set. This format
is used for Marvin > 5.1.0.

**net-f2a8e0f.nnue**
This net was trained using 600M positions searched to depth 10 using
Marvin 4.0.1. It was trained with --use-factorizer.
