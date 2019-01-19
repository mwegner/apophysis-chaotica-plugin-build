INTRO:
------

There are a few different templates for Apophysis plugin compilation out there, but I hadn't seen one that automates
compilation.

This takes the [plugin development template by DarkBeam and bezo97](https://bezo97.tk/plugins/development),

And automates compilation with a batch file.  It expects to find Visual Studio 2017 Build Tools, [which are free to download](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=15).

On the build tools install, I just used default C/C++ selection, and it worked out. You should be able to update the
batch file to use other VS environments.


BUILD AUTOMATION:
-----------------

Run **build.cmd** with no arguments to compile all variations in the "sources" folder.  It drops 64-bit/32-bit versions into
x64/x86 folders.  Logs with warnings/errors go into x64/x86.

You can also invoke build.cmd with the name of a variation, without extension, like:  "build.cmd twoface"


ME:
---

-Matthew (@mwegner on gmail/twitter/etc)
