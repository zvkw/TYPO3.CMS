==========================================================================
Feature: #34922 - Allow .ts file extension for static TypoScript templates
==========================================================================

Description
===========

Only these TypoScript file names were allowed:

- constants.txt
- setup.txt
- include_static.txt
- include_static_files.txt

The ts file extension has been allowed for constants and setup and is prioritised over txt.


Impact
======

There is a little performance impact when loading the TypoScript from scratch like in the backend and frontend without
cache as the new extension is always tested.
