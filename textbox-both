#!/bin/sh
# $Id: textbox-both,v 1.2 2019/12/11 00:06:46 tom Exp $

. ./setup-vars

. ./setup-tempfile

TEXT=/usr/share/common-licenses/GPL
test -f $TEXT || TEXT=../COPYING

expand < textbox.txt > $tempfile
expand < $TEXT >> $tempfile

$DIALOG --clear --title "TEXT BOX" \
	--help-button \
	--extra-button "$@" \
	--textbox "$tempfile" 22 77

retval=$?

. ./report-button
