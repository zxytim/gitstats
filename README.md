gitstats
========

git history statistics generator

what's different from the original one
======================================

+ BUG FIX: If gitstats is soft-linked to directory which is in PATH 
  environment variable (such as $HOME/bin), it can not locate static
  assets property. 
  Fixed by change os.path.abspath to os.path.realpath
