Package building environment for LISE++ Qt project, based on Ubuntu 16.04 (Xenial Xerus); as of Qt 6.5.2 introduced, Ubuntu 20.04 Focal Fossa is being used, not based on Xenial anymore, but still remains the repo name unchanged.

```bash
- tonyzhang/xenial-builder:1.0, linuxdeployqt-7, Qt 5.15.2 (qtcharts)
- tonyzhang/xenial-builder:2.0, + gsl 2.6
- tonyzhang/focal-builder:4.0, Qt 6.5.2 (+Qt Data Visualization, +Qt5Compatlibs)
```

Example:
```bash
VERSION=15.1.2 ./build_lise.sh --input lise_${VERSION}.tar.gz --src-version ${VERSION} --output pkg
```

This container has been used in LISEcute repo at MSU gitlab site in the
CI/CD section.

Starting LISE version 16.16.20, Qt 6.5.2 is being used,
and support Linux OSes released later than Ubuntu 20.04 (Focal), or glibc version >= 2.31