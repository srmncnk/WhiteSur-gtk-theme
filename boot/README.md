# Change Ubuntu Boot & Login Logo

Login logo is stored under /usr/share/plymouth as ubuntu-logo.png
Replace with logo.png

Location of the boot logo can be retrieved like this:
update-alternatives --list default.plymouth
... which should give the following output:
/usr/share/plymouth/themes/bgrt/bgrt.plymouth
Location of the logo:
grep -i imagedir /usr/share/plymouth/themes/bgrt/bgrt.plymouth
Search for:
/usr/share/plymouth/themes/spinner/watermark.png
And replace with logo.png