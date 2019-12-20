#!/bin/sh
# $Id: fselect1-stdout,v 1.7 2019/12/10 23:37:10 tom Exp $

. ./setup-vars

FILE=$HOME
for n in .cshrc .profile .bashrc
do
	if test -f "$HOME/$n" ; then
		FILE=$HOME/$n
		break
	fi
done

RESULT=`$DIALOG --stdout --title "Please choose a file" "$@" --fselect "$FILE" 14 48`
retval=$?

. ./report-string
