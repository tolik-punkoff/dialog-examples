#!/bin/sh
# $Id: fselect,v 1.12 2019/12/10 23:36:16 tom Exp $

. ./setup-vars

exec 3>&1
RESULT=`$DIALOG --title "Please choose a file" "$@" --fselect "$HOME/" 14 48 2>&1 1>&3`
retval=$?
exec 3>&-

. ./report-string
