backenddir = $(libdir)/cups/backend

ACLOCAL_AMFLAGS = -I m4

backend_PROGRAMS = cnusb

cnusb_SOURCES = cnusb.c

cnusb_LDADD = -lcups

AM_CFLAGS = -O2 -Wall -fPIC
#AM_CFLAGS = -g -Wall -fPIC -D_CNUSB_DEBUG_

