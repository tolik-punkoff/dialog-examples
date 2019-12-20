#!/bin/sh
# $Id: report-tempfile,v 1.6 2019/12/11 00:18:08 tom Exp $
# Report results in a temporary-file.
# vile:shmode

case "${retval:-0}" in
  $DIALOG_OK)
    echo "Result: `cat "$tempfile"`";;
  $DIALOG_CANCEL)
    echo "Cancel pressed.";;
  $DIALOG_HELP)
    echo "Help pressed: `cat "$tempfile"`";;
  $DIALOG_EXTRA)
    echo "Extra button pressed.";;
  $DIALOG_ITEM_HELP)
    echo "Item-help button pressed: `cat "$tempfile"`";;
  $DIALOG_ESC)
    if test -s "$tempfile" ; then
      cat "$tempfile"
    else
      echo "ESC pressed."
    fi
    ;;
esac
