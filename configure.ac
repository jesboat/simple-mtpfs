AC_PREREQ([2.60])
AC_INIT([simple-mtpfs], [0.1], [phatina@gmail.com])

AC_CONFIG_MACRO_DIR([m4])

AM_INIT_AUTOMAKE([dist-bzip2])
AC_CONFIG_HEADERS(config.h)
AM_SILENT_RULES([yes])

AC_LANG([C++])
AC_PROG_CXX
AC_PROG_INSTALL

m4_include([m4/cxx11.m4])
AX_CXX_COMPILE_STDCXX_11([noext])
PKG_CHECK_MODULES([FUSE], [fuse >= 2.8])
PKG_CHECK_MODULES([MTP], [libmtp >= 1.1.4])

AC_SUBST([FUSE_CFLAGS])
AC_SUBST([FUSE_LIBS])

AC_OUTPUT([
    makefile
    src/makefile
    man/makefile
])
