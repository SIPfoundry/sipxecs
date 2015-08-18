AC_PREREQ(2.57)

AC_INIT(sipX, 15.06, sipx-dev@list.sipfoundry.org)

# Pass standard and sipxecs common params to ./configure switches on all sub-projects.
# Doesn't have to handle ./configure vars like SIPX_PBXUSER because those
# can be passed handled 

OPTIONS=
	for a in $@; do
		case $a in
			--prefix*)OPTIONS+=" $a" ;;
			--disable-dep-check*)OPTIONS+=" $a" ;;
			--enable-debug*)OPTIONS+=" $a" ;;
			PACKAGE_REVISION*)OPTIONS+=" $a" ;;
			DART*)OPTIONS+=" $a" ;;
		esac
	done

AC_SUBST(OPTIONS)
AC_SUBST(TOP_SRCDIR, $top_srcdir)

AC_CONFIG_FILES([Makefile])

AC_OUTPUT
