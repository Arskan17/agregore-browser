
# Agregore-browser Issue#182 Report

## Introduction

This report details the work done to resolve Issue #182 on Agregore-browser,
the minimal web browser for the distributed web.

## Issue Resolution

I'm still working on it `(Issue #227)`.  
I did it by using attributes, and a function to detect when its value changes, and runs a script depending in accordance.
Events are sent to the `UI`, and depending on the event, the value of the attribute gets updated.
So far it shows the `reload-button` ond the `loading-indicator`

## Summary

- Steps to reproduce: Click on the reload button to load/reload a page
- Expected results: The loading indicator/spinner should be shown, and the reload button hidden.
- Actual results: Both the reload button and the loading indicator are shown idefinitely, no mather if clicked or not.
## Additional notes: 
- Awaiting feedback from admins.

## Ongoing Challenges: I don't really know how to correctly handle events from classes to classes. Feels a little cumbersome. 

## What I learned
- The docker instance you had open when working on a project, apparently doesn't get reloaded when you reboot your machine.
- npm is still a pain to work with.

