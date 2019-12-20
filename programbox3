#!/bin/sh
# $Id: programbox3,v 1.1 2018/06/19 00:33:40 tom Exp $

. ./setup-vars

. ./setup-tempfile

ls -1 >$tempfile
(
while true
do
read text
test -z "$text" && break
ls -ld "$text" || break
sleep 0.1
done <$tempfile
) |

$DIALOG --title "PROGRAMBOX" "$@" --programbox -1 -1

retval=$?
. ./report-button
