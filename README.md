PuTTY-CAC
=========
secure shell client with support for US Gov't Smartcards and other X.509 certificates.

This is a fork of PuTTY.  It breaks much of the delictious goodness of
the original PuTTY, in that it only builds for Windows, and is only
known to build correctly with Microsoft Visual C, at this time.

But it supports the DoD Common Access Card (CAC) and a number of other smartcards.  

PuTTY-CAC is now updated to 0.66 and is in sync with the latest PuTTY
Suite 0.66.  This is my version with the modified pageant.
PuTTY 0.66 fixes a security hole in 0.65 and before:
vuln-ech-overflow. It also contains a few other small bug fixes and
minor features.

Source:
http://www.chiark.greenend.org.uk/~sgtatham/putty/ (Original PuTTY as
developed by Simon Tatham.)
Source: http://www.risacher.org/putty-cac/
(PuTTY-CAC was developed by Dan Risacher.)

WARNING: The PKCS11 API
originally from PuTTY-SC has been removed from all applications in this
PuTTY-CAC Suite due to complications I was having with the code.
However, CAPI support is still functional which is the main premise
behind PuTTY-CAC anyways. If you need to use PKCS11 then DO NOT DOWNLOAD
ANY OF THESE VERSIONS. Download an older release of 0.62 which has
support for PKCS11. If you do not know what I am talking about then this
release should be fine for your needs. Also, none of these releases will
include the PuTTYtel application.

I have included compiled versions of
the PuTTY-CAC suite that can be found in the EXECUTABLES folder for each
type listed above for those that do not want to compile the code.
However, these compiled applications may only work on Windows 7/8. They
have not been tested on older OS’s such as Vista/XP or newer OS's such
as 10.

If you choose to compile the source code yourself you will need
to use the MakeFile.vc as I did not update nor do I support the other
MakeFile.* files.