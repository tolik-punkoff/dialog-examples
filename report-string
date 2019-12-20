#!/bin/sh
# $Id: report-string,v 1.4 2019/12/11 01:31:26 tom Exp $
# Report result passed in a string $RESULT
# vile:shmode

case ${retval:-0} in
  $DIALOG_OK)
    echo "Result is $RESULT";;
  $DIALOG_CANCEL)
    echo "Cancel pressed.";;
  $DIALOG_HELP)
    echo "Help pressed ($RESULT).";;
  $DIALOG_EXTRA)
    echo "Extra button pressed.";;
  $DIALOG_ITEM_HELP)
    echo "Item-help button pressed.";;
  $DIALOG_ESC)
    if test -n "$RESULT" ; then
      echo "$RESULT"
    else
      echo "ESC pressed."
    fi
    ;;
esac
