# adobe-ip-blocker

A hosts file for Windows OS to avoid excessive communication for Adobe apps. 

## USAGE

### Delete the extension
Delete the **.csv** extension.

### Overwrite hosts file
Access the following directory in Windows Explorer.

```
C:\Windows\System32\drivers\etc
```

Overwrite the hosts file.

## Use without overwriting the hosts file
The hosts file can be additioned to rather than overwritten.

open the file `C:\Windows\system32\drivers\etc\hosts` with a code editor such as [VSCode]([URL](https://azure.microsoft.com/ja-jp/products/visual-studio-code/)).

```
# Copyright (c) 1993-2009 Microsoft Corp.
#
# This is a sample HOSTS file used by Microsoft TCP/IP for Windows.
#
# This file contains the mappings of IP addresses to host names. Each
# entry should be kept on an individual line. The IP address should
# be placed in the first column followed by the corresponding host name.
# The IP address and the host name should be separated by at least one
# space.
#
# Additionally, comments (such as these) may be inserted on individual
# lines or following the machine name denoted by a '#' symbol.
#
# For example:
#
#　　　102.54.94.97　　 rhino.acme.com　　 　 # source server
#　　　38.25.63.10　　　x.acme.com　　　　　　# x client host
# localhost name resolution is handled within DNS itself.
#　127.0.0.1　　　　　　localhost
#　::1　　　　　　　　　localhost
```

Add to the last line.

```
# Copyright (c) 1993-2009 Microsoft Corp.
#
# This is a sample HOSTS file used by Microsoft TCP/IP for Windows.
#
# This file contains the mappings of IP addresses to host names. Each
# entry should be kept on an individual line. The IP address should
# be placed in the first column followed by the corresponding host name.
# The IP address and the host name should be separated by at least one
# space.
#
# Additionally, comments (such as these) may be inserted on individual
# lines or following the machine name denoted by a '#' symbol.
#
# For example:
#
#　　　102.54.94.97　　 rhino.acme.com　　 　 # source server
#　　　38.25.63.10　　　x.acme.com　　　　　　# x client host
# localhost name resolution is handled within DNS itself.
#　127.0.0.1　　　　　　localhost
#　::1　　　　　　　　　localhost

127.0.0.1 adobe.com
127.0.0.1 www.adobe.com
:
```

## CAUTION
Back up your hosts file before using it. Updating the hosts file may result in incorrect activation of your Adobe license.
