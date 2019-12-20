#!/bin/sh
# $Id: report-button,v 1.4 2019/12/11 01:26:19 tom Exp $
# Report button-only, no $RESULT
# vile:shmode

case ${retval:-0} in
  $DIALOG_OK)
    echo "OK";;
  $DIALOG_CANCEL)
    echo "Cancel pressed.";;
  $DIALOG_HELP)
    echo "Help pressed.";;
  $DIALOG_EXTRA)
    echo "Extra button pressed.";;
  $DIALOG_ITEM_HELP)
    echo "Item-help button pressed.";;
  $DIALOG_ERROR)
    echo "ERROR!";;
  $DIALOG_ESC)
    echo "ESC pressed.";;
esac
