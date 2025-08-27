# Installing Xcuts

## Installing Sunbundler

Installing Sunbundler is a simple 3-step process.

1. Run this shortcut: https://www.icloud.com/shortcuts/f445b8eb86c242ceb1b3788d15d4e735. You will only need to run it once, to create Xcuts's ROOTFS.
2. Get these shortcuts: https://www.icloud.com/shortcuts/b482c424e11440638991fb1c7d662c71 and https://www.icloud.com/shortcuts/f128cd7e0d69424fa18407d4d22fd979. These let you install packages. Move them to the bin folder in shortcuts created in step 1, and then you're ready to install packages.
3. Install the rest of Sunbundler by downloading https://github.com/sbundle/sbundle-repo/raw/refs/heads/main/lib/sbundles/Sunbundler/SunbundlerLatest.sbundle. To install it, run Sunbundler and select the downloaded file. Once Sunbundler finishes, run Sunbundler Install Helper again and again until it says that the package is installed.

Now, you should have 4 shortcuts in bin: Sunbundler, Sunbundler Install Helper, Uninstall Sbundle, and Sunbundler Update.

## Installing ShortTerm

If you want to install the Xcuts shell (ShortTerm), you'll need to download it at https://github.com/sbundle/sbundle-repo/raw/refs/heads/main/lib/sbundles/ShortTerm/ShortTermLatest.sbundle. Then, run Sunbundler and select the package. After Sunbundler finishes, run Sunbundler Install Helper over and over again as with Sunbundler. Then you can use the shell as well.
To use the shell, run ShortTermX.X.X (version info is embedded in shortcut names to avoid conflicts). Then you can type any command listed here:

 head, in2file, out2file, touch, mkdir, pwd, file, file2var, date, echo, wget, cd, qlook, set, exit, catargs, mail, tail, run, grep, rmdir, rm, ls, cp, sort, cat, mv, man.sh, help.sh, $SB

any of these commands, besides the last three, can be looked up by typing "man.sh [...]".
The last three are: man.sh -> manual page lookup, help.sh -> package README lookup, $SB -> project editor.

## Installing UICuts


If you want to install the Xcuts UI library, you can get it at https://github.com/sbundle/sbundle-repo/raw/refs/heads/main/lib/sbundles/UICuts/UICutsLatest.sbundle.
Use the install instructions outlined in the above section, but instead of installing a shell, you're installing a UI library.

Run SunbundlerUIX.X.X or HConUIX.X.X to see it in action.
