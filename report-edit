#!/bin/sh
# $Id: report-edit,v 1.5 2019/12/11 01:23:08 tom Exp $
# Report results from editing.
# vile:shmode

case ${retval:-0} in
  $DIALOG_OK)
    diff -c "${input:-input}" "${output:-output}"
    echo "OK"
    ;;
  $DIALOG_CANCEL)
    echo "Cancel pressed";;
  $DIALOG_HELP)
    echo "Help pressed";;
  $DIALOG_EXTRA)
    echo "Extra pressed";;
  $DIALOG_ITEM_HELP)
    echo "Item-help button pressed.";;
  $DIALOG_ERROR)
    echo "ERROR!";;
  $DIALOG_ESC)
    echo "ESC pressed.";;
esac
