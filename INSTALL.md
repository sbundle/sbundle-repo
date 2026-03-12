# Installing Xcuts

## Installing Sunbundler

Run this shortcut: https://www.icloud.com/shortcuts/598923a6577146af9d7884d9a4336b30. You will only need to run it once, to create Xcuts's ROOTFS and start the install process. Every time a shortcut pops up, click add shortcut, quickly. You can review them later.

Now, you should have 4 shortcuts in bin: Sunbundler, Sunbundler Install Helper, Uninstall Sbundle, and Sunbundler Update.

## Installing ShortTerm

If you want to install the Xcuts shell (ShortTerm), you'll need to download it at https://github.com/sbundle/sbundle-repo/raw/refs/heads/master/lib/sbundles/ShortTerm/ShortTermLatest.sbundle. Then, run Sunbundler and select the package. Keep installing shortcuts as said above. Then you can use the shell as well.
To use the shell, run ShortTermX.X.X (version info is embedded in shortcut names to avoid conflicts). Then you can type any command listed here:

 head, in2file, out2file, touch, mkdir, pwd, file, file2var, date, echo, wget, cd, qlook, set, exit, catargs, mail, tail, run, grep, rmdir, rm, ls, cp, sort, cat, mv, man.sh, help.sh, $SB

any of these commands, besides the last three, can be looked up by typing "man.sh [...]".
The last three are: man.sh -> manual page lookup, help.sh -> package README lookup, $SB -> project editor.

## Installing UICuts


If you want to install the Xcuts UI library, you can get it at https://github.com/sbundle/sbundle-repo/raw/refs/heads/master/lib/sbundles/UICuts/UICutsLatest.sbundle.
Use the install instructions outlined in the above section, but instead of installing a shell, you're installing a UI library.

Run SunbundlerUIX.X.X or HConUIX.X.X to see it in action.
