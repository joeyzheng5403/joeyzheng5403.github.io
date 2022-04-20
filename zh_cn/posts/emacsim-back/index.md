<!--
.. title: Emacs,I'm back!
.. slug: emacsim-back
.. date: 2022-04-15 18:54:29 UTC+08:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

I change from Emacs and vim so many times.
And use SpaceVim and SpaceEmacs.
After a little try my own config,I found it's have to use SpaceEmacs.
So I start to read SpaceEmacs' doc.

This blog will record any thing I learn how to use Emacs.

## Open emacs in terminal 
It's quite easy to open emacs in terminal
```
emacs -nw
```
but if you load a lot of plugin, it's a little slow to start.
so I aways run emacs as deamon 
```
emacs --deamon
```
and use a client in terminal
```
emacsclient -nw somefile
```

## Searching and Replacing in Multiple Files
A cool trick I learned recently is the ability to search and replace in multiple files.

1. With helm-ag you can search through all files in your projectile project with SPC / or SPC s p.
2. Enter your search query and a list of files with that occurrence will show up
3. Then hit C-c C-e and Spacemacs will create a helm-ag-edit buffer
4. Now you can use any command you’d normally be able to run on a buffer. For example, a simple Vim search and replace %s/alice/bob/g.
5. Then hit C-c C-c to save the changes.
