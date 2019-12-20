#!/bin/sh
# $Id: buildlist4,v 1.1 2019/08/08 23:20:58 tom Exp $

. ./setup-vars

. ./setup-tempfile

$DIALOG --title "BUILDLIST DEMO" --backtitle "A user-built list" \
	--separator "|" \
	--help-button \
	--item-help \
	--buildlist "hello, this is a --buildlist..." 0 0 0 \
		"1" "Item number 1" "on"  first \
		"2" "Item number 2" "off" second \
		"3" "Item number 3" "on"  third \
		"4" "Item number 4" "on"  fourth \
		"5" "Item number 5" "off" fifth \
		"6" "Item number 6" "on"  sixth 2> $tempfile

retval=$?

. ./report-tempfile
