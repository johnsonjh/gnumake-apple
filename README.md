# gnumake-apple

## Overview

* A portable version of Apple's **GNU Make 3.81**, as shipped with Apple macOS.

## Support

* Tested on **GNU/Linux**, **AIX** 7.3, **NetBSD** 9.3, **FreeBSD** 13.1, **OpenBSD** 7.2, and **macOS** 13.1.

## Notes

### Building on OpenBSD

1. Install `autoconf`, `automake`, `gmake`, and `gettext-utils` via ports or packages.
2. Configure and build:
   ```bash
   env MAKE=gmake AUTOCONF_VERSION=2.71 AUTOMAKE_VERSION=1.16 \
     autoreconf -vfi
   ./configure --disable-dependency-tracking
   gmake
   ```
