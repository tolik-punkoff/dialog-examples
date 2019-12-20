#!/bin/sh
# $Id: inputbox6-8bit,v 1.7 2019/12/11 01:14:49 tom Exp $

. ./setup-vars

. ./setup-tempfile

. ./testdata-8bit

$DIALOG \
--title    "`printf '%s' "$SAMPLE"`" "$@" \
--inputbox "`printf '%s' "$SAMPLE"`" \
10 40      "`printf '%s' "$SAMPLE"`" 2>$tempfile

retval=$?

. ./report-tempfile
