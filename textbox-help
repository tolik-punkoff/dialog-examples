#!/bin/sh
# $Id: textbox-help,v 1.2 2019/12/11 00:06:26 tom Exp $

. ./setup-vars

. ./setup-tempfile

TEXT=/usr/share/common-licenses/GPL
test -f $TEXT || TEXT=../COPYING

expand < textbox.txt > $tempfile
expand < $TEXT >> $tempfile

$DIALOG --clear --title "TEXT BOX" \
	--help-button "$@" \
	--textbox "$tempfile" 22 77

retval=$?

. ./report-button
