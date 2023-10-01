# Abseil - C++ Common Libraries

Mainly used for hashOf() computations.

mkdir build && cd build
cmake .. -DCMAKE_INSTALL_PREFIX=../include/abseil-cpp
make && make install

when you compile your .cpp file including <absl/hash/hash.h>, you are supposed to link that with the other three libraries like:
LDFLAGS = -L./include/abseil-cpp/lib -labsl_hash -labsl_city -labsl_low_level_hash

## Table of Contents

- [About Abseil](#about)
- [Quickstart](#quickstart)
- [Building Abseil](#build)
- [Support](#support)
- [Codemap](#codemap)
- [Releases](#releases)
- [License](#license)
- [Links](#links)

<a name="about"></a>
## About Abseil

Abseil is an open-source collection of C++ library code designed to augment
the C++ standard library. The Abseil library code is collected from Google's
own C++ code base, has been extensively tested and used in production, and
is the same code we depend on in our daily coding lives.

In some cases, Abseil provides pieces missing from the C++ standard; in
others, Abseil provides alternatives to the standard for special needs
we've found through usage in the Google code base. We denote those cases
clearly within the library code we provide you.

Abseil is not meant to be a competitor to the standard library; we've
just found that many of these utilities serve a purpose within our code
base, and we now want to provide those resources to the C++ community as
a whole.
