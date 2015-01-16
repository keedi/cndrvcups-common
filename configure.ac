#!/bin/bash
# 
# File:   configure.ac
# Author: richter
#
# Created on 16.01.2015, 00:41:40
#

AC_INIT([cndrvcups-common], [2.90], [krichter722@aol.de])
AC_CONFIG_MACRO_DIR([m4])
AM_INIT_AUTOMAKE([foreign -Wall]) 
    # `-Wno-portability` causes 
    # `'%'-style pattern rules are a GNU make extension`
AC_PROG_CC
AM_PROG_AR
LT_INIT # needs to be after AM_PROGS_AR
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_SUBDIRS([backed buftool c3plmod_ipc cngplp cngplp/po cngplp/src cngplp/cnjatool])
AC_CONFIG_FILES([Makefile backend/Makefile buftool/Makefile c3plmod_ipc/Makefile cngplp/Makefile cngplp/po/Makefile cngplp/src/Makefile cngplp/cnjatool/Makefile])
    # omitting causes `error: no 'Makefile.am' found for any configure output 
    # Did you forget AC_CONFIG_FILES([Makefile]) in configure.ac?`
AC_OUTPUT