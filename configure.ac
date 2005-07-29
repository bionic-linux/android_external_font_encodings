AC_PREREQ([2.57])
AC_INIT([encodings], [0.99.0], [https://bugs.freedesktop.org/enter_bug.cgi?product=xorg])
AM_INIT_AUTOMAKE([foreign dist-bzip2])

# mkfontscale

AC_PATH_PROG(MKFONTSCALE, mkfontscale)
if [[ -z $MKFONTSCALE ]]; then
   AC_MSG_ERROR([mkfontscale is needed to build fontenc. FIXME: when we
		 know where it is going to live, put a more informative
		 comment here])
fi

# gzip

AC_PATH_PROG(GZIP, gzip)
if [[ -z $GZIP ]]; then
   AC_MSG_ERROR([gzip is needed to compress font encodings])
fi

XORG_RELEASE_VERSION

AC_OUTPUT([Makefile large/Makefile])
