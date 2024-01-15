
# Agregore-browser Issue#227 Report

## Introduction

This report details the work done to resolve Issue #227 on Agregore-browser,
the minimal web browser for the distributed web.

## Learning Phase

I began by familiarizing myself with Electron, as the browser is Electron-based.
This was a necessary step to understand the context and requirements of the
issue.

## Setup Phase

Setting up the development environment posed some challenges. Initially, I
encountered issues with `npm` and `yarn` on my local machine. Despite several
attempts, I was unable to resolve these issues. Consequently, I switched to
GitHub Spaces, which successfully set up all the dependencies. However, I was
unable to push to my branch due to a persistent `git error: failed to push
some refs to remote`. 
As a workaround, I decided to use Docker, which,
despite taking some time to set up, eventually allowed me to work smoothly.

## Issue Resolution

I was able to resolve part of the main issue (Issue #227), but the code still
needs to be formatted according to the project’s style guide. In the process, I
created some additional functions and objects that were not originally present
in the code. I am currently awaiting feedback from the Project owner regarding
these additions (since they implemented the UI, the part I’m currently working
on).

## Summary

- Steps to reproduce: Using the middle mouse click, click on the address
    bar.
- Expected results: The recently copied URL in your Clipboard should be
    pasted into the address bar, and the website should load.
- Actual results: The URL is pasted into the address bar, but the website is
    not loading automatically.
## Additional notes:

- I think the part to load the website must be in there, since the browser
does just that when the `Enter key` is pressed.

- Also, I should format the code in style with what’s already there, so it’s
easier to understand.

## Ongoing Challenges

One ongoing challenge is finding a more efficient way to test my
implementation. Currently, I have to build the entire project and go through the
process of installing & uninstalling every time I want to check if my
implementation works. I am actively seeking a workaround for this issue.

## What I learned

Electron is a really powerful tool. It allows you to easily create applications that
can be packaged for pretty much every major OS.

Docker is a lifesaver when it comes to setting up your development
environment without affecting your local machine, or your local machine
affecting your workflow.

Npm and yarn packages can be a pain to work with.

Working on an unfamiliar project can be really daunting at first, but when you
get going, you can learn a lot.

Config files are amazing at doing all the grunt work and letting you focus on
resolving your main tasks.

The most interesting was working with the package manager, and setting it up
just the way I needed.


