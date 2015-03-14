This is the place where ppchugs project lives.



# Installations #
  * Download CELIB binary dll to your device under folder /windows.
  * Copy the hugs.exe to your device. Note that this binary only works for Arm/Xscale pocketpc. To make it works for your specific processor, you need to recompile the binary.
  * Copy folder /lib to your device under /unix/hugs/
  * Modify your /HK\_LocalMachine/Enviroment registry on your device. Refer this page for details. You can use ceregedt.exe (comes with EVT 3.0) to edit the registry.

# Compilation #
  * Download PPCHugs Source.
  * Download [CELIB source](http://www.google.com/url?sa=t&source=web&cd=1&ved=0CBIQFjAA&url=http%3A%2F%2Fcelib.sourceforge.net%2F&ei=XqjtTPSNEI6mugPk4PjQAQ&usg=AFQjCNEkfBV_Mpu76gk4sqC4zMVXS_h1Qw), extract it on the host PC.
  * Download [Console source](http://www.rainer-keuchel.de/wince/console.html), extract it on the host PC.
  * Download Embedded Visual Tools 3.0, install it.
  * Change path and platform settings in file Makefile.ce and plain-exe-inc.mak, then
`nmake -f makefile`

# Limitations #
  * All paths must be absolute.
  * No CPUTime support.
  * No scrolling.
  * Arrow Keys and Backspace are not functioning.