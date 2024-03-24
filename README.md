# Overview

This repository contains NNUE networks for the [Marvin chess engine](https://github.com/bmdanielsson/marvin-chess).

# v1 nets

The v1 format uses a standard HalfKP 128x2-32-32-1 architecture. This format
is used by Marvin 5.0.0 - 5.1.0.

**net-3f7389e.nnue**

The default net for Marvin 5.0.0. If was trained using 600M positions searched
to depth 10 using Marvin 4.0.1.

**net-ca6610a.nnue**

The default net for Marvin 5.1.0. If was trained using 600M positions searched
to depth 10 using Marvin 4.0.1.

# v2 nets

The v2 format uses a standard HalfKP 128x2-32-32-1 architecture with a few
modifications. Firstly flip is used instead of rotate for symmetry and secondly
the Shogi drop piece has been removed from the input feature set. This format
is used for Marvin > 5.1.0.

**net-f2a8e0f.nnue**

This net was trained using 600M positions searched to depth 10 using
Marvin 4.0.1. It was trained with --use-factorizer.

**net-422c365.nnue**

The default net for Marvin 5.2.0. This net was trained using 1B positions searched to depth 8 using
Marvin 5.1.0 and net-f2a8e0f.nnue for evaluation. It was trained with --use-factorizer.

# v4 nets

The v4 format uses the HalfKP 256x2-32-32-1 architecture. Additionally
quantization have been moved to the engine. Not used for any public version
of Marvin.

**net-9ef737e9.nnue**

This net was trained using 3B positions searched to depth 8. It was
trained with --use-factorizer.

# v5 nets

The v5 format uses the HalfKP 256x2-16-16-1 architecture. This format is
used for Marvin > 6.0.0.

**net-710faff.nnue**

This net was trained using 3B positions searched to depth 8. It was
trained with --use-factorizer.

# v7 nets

The v7 format uses the HalfKP 256x2-8-16-1 architecture. This format is
used for Marvin > 6.2.0.

**net-0d21cd7.nnue**

This net was trained using 3B positions searched to depth 8. It was
trained with --use-factorizer.

