#!/bin/bash
# 
# File:   configure.ac
# Author: richter
#
# Created on 16.01.2015, 00:41:40
#

AC_INIT([cndrvcups-common], [2.90], [krichter722@aol.de])
AM_INIT_AUTOMAKE([foreign -Wall -Werror]) 
    # `-Wno-portability` causes 
    # `'%'-style pattern rules are a GNU make extension`
AC_PROG_CC
AC_PROG_RANLIB
AM_PROG_AR
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile backend/Makefile buftool/Makefile c3plmod_ipc/Makefile cngplp/Makefile])
AC_OUTPUT