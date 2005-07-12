AC_PREREQ([2.57])
AC_INIT([encodings], [7.0], [xorg@lists.freedesktop.org])
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

AC_OUTPUT([Makefile large/Makefile])
