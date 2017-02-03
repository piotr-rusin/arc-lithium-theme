AC_INIT(
    [arc-lithium-theme],
    [20161119],
    [https://github.com/piotr-rusin/arc-lithium-theme/issues],
    [arc-lithium-theme],
    [https://github.com/piotr-rusin/arc-lithium-theme],
    []
)

AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_MACRO_DIR([m4])
AM_INIT_AUTOMAKE([no-dist-gzip dist-xz foreign])
AC_PROG_MKDIR_P

ARC_LITHIUM_ENABLE([LIGHT],         [light],         [Arc Lithium Light],     [disable])
ARC_LITHIUM_ENABLE([DARKER],        [darker],        [Arc Lithium Darker],    [disable])
ARC_LITHIUM_ENABLE([DARK],          [dark],          [Arc Lithium Dark],      [disable])
ARC_LITHIUM_ENABLE([CINNAMON],      [cinnamon],      [Cinnamon],      [disable])
ARC_LITHIUM_ENABLE([GNOME_SHELL],   [gnome-shell],   [GNOME Shell],   [disable])
ARC_LITHIUM_ENABLE([GTK2],          [gtk2],          [GTK2],          [disable])
ARC_LITHIUM_ENABLE([GTK3],          [gtk3],          [GTK3],          [disable])
ARC_LITHIUM_ENABLE([METACITY],      [metacity],      [Metacity],      [disable])
ARC_LITHIUM_ENABLE([UNITY],         [unity],         [Unity],         [disable])
ARC_LITHIUM_ENABLE([XFWM],          [xfwm],          [XFWM],          [disable])
ARC_LITHIUM_ENABLE([TRANSPARENCY],  [transparency],  [transparency],  [disable])

AS_IF([test "x$ENABLE_GNOME_SHELL$ENABLE_GTK3" != xnono], [ARC_LITHIUM_GNOME])

AC_CONFIG_FILES([
    common/Makefile
    extra/Makefile
    Makefile
])

AC_OUTPUT
