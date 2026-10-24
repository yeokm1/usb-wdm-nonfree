# Notice: NUSB 3.3's Windows 98 SE USB storage files

## Why these files are kept apart

`nusb33/` sits at this repository's root, apart from `non-free/`, because
it is a special case (owner, 2026-10-22). Six of its seven files are
Microsoft's, from Windows Millennium (two of them INFs that NUSB's
author edited); the seventh is a third party's; NUSB 3.3 assembled them, and no licence to redistribute any of them has been
found. The repository's owner has accepted that risk for these files.
The xHCI98 project's base release download carries them in its own
`NUSB33\` folder, beside its installer, which installs them on Windows 98
SE; it does not carry `non-free/`, which is offered on its own.

The files are not this repository's to license, and its owner claims no
rights in them and grants no licence to them.

## The files

All in `nusb33/w98se/` (in xHCI98's download, `NUSB33\W98SE\`).

| File | Whose | Version | SHA-256 |
|---|---|---|---|
| `USBSTOR.SYS` | Microsoft Corporation (Windows Millennium) | 4.90.3000.1 | `b92a6a1582287867d4950495c0a746f0f5d8831bc311061423f8645073e42d8c` |
| `USBNTMAP.SYS` | Microsoft Corporation (Windows Millennium) | 4.90.3000 | `d1595cdbfdc22925c4e47d1720f117fe6c9beda36417ba41a1fd7398878cc6e4` |
| `USBMPHLP.PDR` | Microsoft Corporation (Windows Millennium) | 4.90.3000 | `e8e0604fddcd1772f1c5cba99de9d72d79288d0b303ed3e7bf02d36160698c1c` |
| `USBAUTH.SYS` | Microsoft Corporation (Windows Millennium) | 4.90.3000.1 | `12b09e67a5a9a8a883ab40b91c59be294f2ddc5940b9780c056176df04a463d1` |
| `USBU2A.SYS` | "USB Compliance", per its version resource (copyright 2000) | 1.42 | `1c5656dcf3dbbca97236fc0239537a34ae5a6ca1597f29cadc9c38537b2a7b78` |
| `USBSTOR.INF` | Microsoft's INF, with the edits listed in its own comment header (Maximus Decim and others) | as in NUSB 3.3 | `e78b5f2d2d30b039d74d670f09ba41c39bdfca058b72fd7c22eb7d55f81f0f6b` |
| `USBNTMAP.INF` | as `USBSTOR.INF` | as in NUSB 3.3 | `372d0a4829eab33cf5c6a1fca347a3be45da82d69a692e89b33d28dc02848657` |

They are copied unmodified, byte for byte, from Maximus Decim's Native USB
package version 3.3 for English Windows 98 SE. The same hashes are in this
repository's `SHA256.TXT` (and in the `SHA256.TXT` beside this notice in
xHCI98's download).

## Provenance

Searches recorded below were made on 2026-10-20.

- **Author:** Maximus Decim (MSFN forum user `maximus-decim`), who
  assembled the package; the files in it are Microsoft's and others', as
  in the table above.
- **Package:** Maximus Decim Native USB ver. 3.3, English, for Windows 98
  SE ("NUSB 3.3"). The newest file in it is dated 2007-11-16.
- **Original download location:** NUSB had no vendor site. It was
  distributed from the first post of its MSFN thread,
  <https://msfn.org/board/topic/43605-maximus-decim-native-usb-drivers/>
  (posted 2005-04-11 and updated per release). That post linked
  `http://rapidshare.com/files/70087438/nusb33e.exe.html`, as archived at
  <https://web.archive.org/web/20100312065424/http://www.msfn.org/board/topic/43605-maximus-decim-native-usb-drivers/>;
  Rapidshare no longer exists, and no archived copy of that file was
  found. The post now links
  `http://www.technical-assistance.co.uk/drivers/nusb33e.exe`, which as of
  2026-10-20 redirects to an unrelated site. Archived copy:
  <https://web.archive.org/web/20130415135551/http://www.technical-assistance.co.uk/drivers/nusb33e.exe>.
- **Obtained:** the date the original copy was obtained was not recorded;
  the files were added to this repository on 2026-10-20 (under
  `non-free/storage/nusb33/w98se/`, moved here on 2026-10-22). On
  2026-10-20 the archived copy above was downloaded and matched: same size
  and SHA-256 as below, and all seven files match the hashes above.
- **Archive:** `nusb33e.exe`, 774,144 bytes, SHA-256
  `f1f30a800cf6013eb6f18db775d88e777ddc3924622e6560edd2dcd7b53698d3`. It is
  a self-extracting Microsoft CAB; the files are in the CAB, which 7-Zip
  lists and unpacks without running anything.
- **Licence:** none found. The CAB's `!README.TXT` gives the package name,
  "Only for Windows 98SE English !!!", installation steps, and "Remember!
  You install it at own risk!"; it states no licence or redistribution
  terms, and neither does the MSFN post. `USBSTOR.INF` and `USBNTMAP.INF`
  carry only Maximus Decim's change logs.
- **Modification:** none.

They are offered only so that Windows 98 SE, which Microsoft no longer
supports or distributes, can use USB storage devices without the full NUSB
package.

If you hold rights in any of these files and want them removed, open an
issue on this repository and they will be taken down.

## This notice

This file is the repository owner's, released under CC0 1.0 (public domain
dedication, <https://creativecommons.org/publicdomain/zero/1.0/>). That
covers this file only, and none of the seven files above.
