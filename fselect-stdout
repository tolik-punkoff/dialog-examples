#!/bin/sh
# $Id: fselect-stdout,v 1.7 2019/12/10 23:36:22 tom Exp $

. ./setup-vars

RESULT=`$DIALOG --stdout --title "Please choose a file" "$@" --fselect "$HOME/" 14 48`
retval=$?

. ./report-string
