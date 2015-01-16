SUBDIRS = backend buftool c3plmod_ipc cngplp

_prefix=/usr

dirs= cngplp buftool backend #cpca
scripts=for dir in $(dirs); do\
				(cd $$dir; make $$target)|| exit 1;\
		done

all-local :
	$(scripts)

clean-local :
	target=$@; $(scripts)

distclean-local :
	target=$@; $(scripts)

install-exec-local :
	target=$@; $(scripts)

uninstall-local :
	target=$@; $(scripts)

gen :
	(cd cngplp; ./autogen.sh; make) || exit 1
	(cd buftool; ./autogen.sh; make) || exit 1
	(cd backend; ./autogen.sh --prefix=${_prefix}; make) || exit 1
#	(cd cpca; ./autogen.sh --prefix=${_prefix}; make) || exit 1

