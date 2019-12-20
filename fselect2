#!/bin/sh
# $Id: fselect2,v 1.9 2019/12/10 23:37:10 tom Exp $

. ./setup-vars

exec 3>&1
RESULT=`$DIALOG --title "Please choose a file" "$@" --fselect "$HOME/" 0 0 2>&1 1>&3`
retval=$?
exec 3>&-

. ./report-string
