# TinyHugoTest
This is a tiny repository with a hugo project designed to not work right.


This is a happy little hugo project created to demonstrate the issues as discussed in

https://discourse.gohugo.io/t/hugo-does-not-see-or-build-content-unless-i-save-a-change-to-disk/14819/11

It does not behave as I expect it to:

Expected behaviour:
Run hugo server
Click on buttons, go to pages A,B,C.

Observed behavior.
Run Hugo Server
Click on buttons, page not found
Edit source of pages. Hugo updates... the page that was edited now exists, but other pages don't.


Note that this broken behavior occurs ONLY if there exists an index.md file. If we have no index.md, then all is well.

I am running Hugo version 0.56.0, on ubunutu.

I can get the site to load by getting rid of index page... but it seems sad that having index.md causes things to break.
