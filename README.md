# usb-wdm-nonfree

Drivers for USB devices on old versions of Windows (98 SE, ME, 2000, XP,
Vista and 7), collected in one place. These are the device makers' own
drivers (and, for Xbox 360 pads, a well-known independent author's),
exactly as they released them. They are not ours to license: see
[NOTICE.md](NOTICE.md) for who owns each one and where it came from.

This collection is gathered for the [xHCI98](https://github.com/yeokm1/xhci98)
project, a USB 3 host controller driver for the same systems, and its
release downloads can carry it. The drivers can also be used on their
own, under Windows' own USB drivers or another host controller driver.

## What works on which Windows

"Yes" means a driver for that system is in this repository. Find your
device's chip in Device Manager (Properties, Details, Hardware Ids) or on
the box; the brand on the dongle often differs from the chip inside.

| Device | Chip / model | 98 SE | ME | 2000 | XP | XP x64 | Vista | 7 |
|---|---|---|---|---|---|---|---|---|
| USB flash drives, card readers and USB disks | any standard USB storage device | Yes | built in | built in | built in | built in | built in | built in |
| USB 2.0 Ethernet adapter | ASIX AX88772, AX88772A | Yes | Yes | Yes | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit) |
| USB 2.0 Ethernet adapter | ASIX AX88772B, AX88772C | - | - | Yes | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit) |
| USB 2.0 Gigabit Ethernet adapter | ASIX AX88178 | Yes | Yes | Yes | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit) |
| USB 2.0 Ethernet adapter | ASIX AX88172 | Yes | Yes | Yes | Yes | - | - | - |
| USB 2.0 Ethernet adapter | ASIX AX88172A | - | - | Yes | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit) |
| USB 3.0 Gigabit Ethernet adapter | ASIX AX88179, AX88178A | - | - | - | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit) |
| USB Ethernet adapter (most USB-C dongles) | Realtek RTL8152, RTL8153 (on 7 also RTL8156) | - | - | - | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit) |
| USB 1.1 Ethernet adapter | Realtek RTL8150 | Yes | Yes | Yes | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit), Vista's driver, not listed by Realtek for 7 |
| USB 2.0 Ethernet adapter | MosChip (now ASIX) MCS7830, MCS7832, MCS7730 | Yes | Yes | Yes | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit) |
| USB 1.1 Ethernet adapter | Davicom DM9601 | Yes | Yes | Yes | Yes | - | - | - |
| USB 2.0 Ethernet adapter | Davicom DM9620, DM9621, DM9621A | Yes | Yes | Yes | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit) |
| USB Ethernet adapter | Davicom DM9622 | Yes | Yes | Yes | - | - | Yes (32/64-bit) | - |
| USB serial adapter | FTDI FT232R, FT232BM, FT245R/BM, FT8U232AM | Yes | Yes | Yes | - | - | - | - |
| USB serial adapter, dual port | FTDI FT2232D | Yes | Yes | Yes (FT2232, FT4232H) | - | - | - | - |
| USB serial adapter (cheap Arduino clones) | WCH CH340, CH341 | Yes | Yes | Yes | Yes | - | - | - |
| Xbox 360 wired controller | Microsoft and 24 Logitech, Saitek, Mad Catz and HORI pads (list below) | Yes | Yes | Yes | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit) |
| Xbox 360 Wireless Gaming Receiver | Microsoft receiver | - | - | Yes | Yes | Yes | Yes (32/64-bit) | Yes (32/64-bit) |

Not here because their licences forbid passing them on, so download them
from the maker (links below, under "Not shipped"): Silicon Labs CP210x,
Prolific PL2303 and M-Audio MidiSport. Microchip's LAN9500 and LAN7800
Ethernet drivers are not here either. Their terms could not be read.
Links to them are under "Not shipped" too.

**Not covered:** no driver for these USB Ethernet chips on the systems
named was found, here or at their makers:

- ASIX AX88772E and AX88279A, on 98 SE to 7. ASIX offers drivers for
  Windows 8 or 10 and later only.
- ASIX AX88179A, AX88772D and AX88279, on 98 SE to 7. ASIX offers
  drivers for Windows 8 and later only. The AX88179 drivers here match
  their USB ID, but whether they run these chips is not known. ASIX
  documents these chips as standard CDC-NCM devices too. The separate
  `usb-wdm-free` repository has a CDC-NCM driver, not tried with them.
- Realtek RTL8157 and RTL8159, on 98 SE to 7. Realtek offers drivers for
  Windows 10 and later only.
- Realtek RTL8156, RTL8156B, RTL8155 and RTL8153D, on 98 SE to Vista.
  The Windows 7 driver here covers them on 7.
- CoreChips SR9700 and SR9800, and WCH CH9200, on 98 SE to 7.
- Microchip LAN7500 and LAN7505, on 98 SE to 7.
- ASIX AX88772B and AX88772C, on 98 SE and ME.
- ASIX AX88172A, on 98 SE and ME.
- ASIX AX88172, on XP x64, Vista and 7.
- Davicom DM9601, on XP x64, Vista and 7.
- Davicom DM9622, on XP, XP x64 and 7.

**How to install:** plug the device in, and when Windows asks for a driver
(or in Device Manager: the device, Update Driver), point it at the folder
for your system, listed in that device's section below. Each folder is a
complete driver; keep its files together and don't rename them.

**Status:** the drivers under `non-free/` are carried exactly as their
makers released them (Davicom's `dm96xx/wxp-7/` was unpacked from its
installer, see its section) and are not tested by this project, on real or
virtual machines (the repository owner's decision, 2026-10-22). Only
NUSB 3.3's USB storage files (`nusb33/`) have been tried here, on
Windows 98 SE. One INF check was also made: Windows 98 SE reads ASIX's
AX88172 INF for 98 SE and ME (2026-10-27, see that chip's section).

**Letting Windows find them at the first plug:** [STAGE.TXT](STAGE.TXT)
lists which INF may be staged on which Windows, one line per INF, for an
installer that offers to place them where Windows looks when a device is
plugged in (xHCI98's installer, as an option that is off unless ticked).
Where two INFs here would match the same device, it names the one to
use; the format is described at its top.

Drivers this project writes itself, as free software, are in the separate
`usb-wdm-free` repository.

## Folder layout and file names

Drivers are in `non-free/<type>/<driver>/<system>/`, apart from NUSB
3.3's storage files, which are in `nusb33/w98se/` (below). The last folder
names the Windows it is for: `w98se-me` is 98 SE and ME, `w2k` is 2000,
`wxp` is XP, `wxpvis` is XP and Vista, `w7` is 7, and `64` at the end
means 64-bit. A folder named for two systems with a dash between them,
such as `w2k-xp` or `w98se-vista`, serves a range of systems. Each
driver's section below lists them exactly.

File names are kept as each vendor shipped them. Don't rename them: the
drivers' INF files refer to them by name.

Every driver here needs a USB host controller driver underneath it: the
system's own, or another the user has installed (on Windows 98 SE, NUSB's
USB 2.0 stack, for example).

## `nusb33/` - USB mass storage, Windows 98 SE only, kept apart

`nusb33/` is not under `non-free/`, and has its own notice,
[nusb33/NOTICE.md](nusb33/NOTICE.md). It is a special case (owner,
2026-10-22): six of its seven files are Microsoft's, from Windows
Millennium (two of them INFs that NUSB's author edited), the seventh
(`USBU2A.SYS`) a third party's, and no licence to redistribute any of
them has been found; the repository's owner has
accepted that risk for them. The xHCI98 project's base release download
carries these seven files on their own, in its `NUSB33\` folder, for its
installer; it does not carry `non-free/`, which is offered separately.

`nusb33/w98se/`: USB mass-storage drivers, taken unmodified from NUSB 3.3, so a Windows 98
SE machine can use USB flash drives and disks without installing the full
NUSB package. Its USB 2.0 stack is not needed; whether any of its
core-file replacements are, on a completely stock Windows 98 SE, is not yet
known (see "Not yet tested" below).

| File | What it does |
|---|---|
| `USBSTOR.INF`, `USBSTOR.SYS` | The USB mass-storage class driver (Bulk-Only, CBI and CB devices) |
| `USBNTMAP.INF`, `USBNTMAP.SYS` | Maps a USB disk into Windows 98's IOS layer, so it gets a drive letter |
| `USBMPHLP.PDR` | The IOS port driver `USBNTMAP` works with |
| `USBAUTH.SYS` | A lower filter that `USBSTOR.INF` installs for a few authenticated card readers |
| `USBU2A.SYS` | A lower filter that `USBSTOR.INF` installs for a few CBI devices |

NUSB 3.3's INFs are used rather than 3.6's: the driver binaries are
byte-identical in both, but 3.6's INFs copy no files on their own, since
NUSB 3.6's main installer does that.

If NUSB 3.3 or 3.6 is already installed, it carries the same files and
nothing more is needed.

By hand: point the Add New Hardware Wizard, or Update Driver on the device,
at `nusb33/w98se/`. On the first storage device Windows may bind the disk
to its own generic "Disk drive" before it has seen `USBNTMAP.INF`, and no
drive letter appears. In that case, in Device Manager open Disk drives, "Disk
drive", Driver, Update Driver, point it at the same folder (it installs "USB
Disk"), then unplug the device and plug it back in.

Windows ME and later ship their own storage drivers. Do not install these
files there.

**Not yet tested:** these files have been shown working without NUSB's USB
2.0 stack only on a Windows 98 SE install that still held NUSB's other
hotfix files (`IOS.VXD`, `DISKTSD.VXD`, `NTMAP.SYS`). Whether a completely
stock Windows 98 SE needs any of those is not yet known.

## `non-free/ethernet/` - USB Ethernet

ASIX's drivers for USB 2.0 Ethernet adapters built on the AX88772 family,
and for USB 3.0 Gigabit adapters built on the AX88179 and AX88178A, one
folder per system, each as ASIX released it:

| Folder | Systems | Driver | Chips |
|---|---|---|---|
| `ax88772/w98se-me/` | Windows 98 SE and ME | `AX88772.SYS` 3.0.3.12 (2004-04-08) | AX88772, AX88772A |
| `ax88772/w2k-xp/` | Windows 2000 and XP, 32-bit | `ax88772.sys` 3.4.3.38 (2010-08-04) | AX88772, AX88772A, AX88760 |
| `ax88772/wxp64/` | Windows XP x64 | `ax88772.sys` 3.6.3.18 (2007-09-21) | AX88772, AX88772A |
| `ax88772/wvista/` | Windows Vista, 32-bit | `ax88772.sys` 3.8.3.22 (2009-10-02) | AX88772, AX88772A, AX88760 |
| `ax88772/wvista64/` | Windows Vista, 64-bit | `ax88772.sys` 3.10.3.14 (2008-11-18) | AX88772, AX88772A |
| `ax88772/w7/` | Windows 7, 32-bit | `ax88772.sys` 3.12.3.2 (2009-06-10) | AX88772, AX88772A, AX88760 |
| `ax88772/w7_64/` | Windows 7, 64-bit | `ax88772.sys` 3.14.3.2 (2009-06-10) | AX88772, AX88772A, AX88760 |
| `ax88179/wxpvis/` | Windows XP and Vista, 32-bit | `ax88179_178a.sys` 1.4.2.0 (2013-05-24) | AX88179, AX88178A |
| `ax88179/wxpvis64/` | Windows XP and Vista, 64-bit | `ax88179_178a.sys` 1.6.2.0 (2013-05-24) | AX88179, AX88178A |
| `ax88179/w7/` | Windows 7, 32-bit | `AX88179_178a.sys` 1.12.11.0 (2018-01-19) | AX88179, AX88178A |
| `ax88179/w7_64/` | Windows 7, 64-bit | `AX88179_178a.sys` 1.14.11.0 (2018-01-19) | AX88179, AX88178A |

The Windows 2000 and XP AX88772 driver is a KMDF 1.7 driver: its INF installs
Microsoft's KMDF co-installer, `WdfCoInstaller01007.dll`, which ASIX ships
in the same package, so keep the folder's files together. ASIX's
`history.txt` lists that driver's changes. The XP and Vista AX88179
drivers are KMDF 1.9 drivers in the same way, with
`WdfCoInstaller01009.dll`; KMDF 1.9 does not run on Windows 2000, and
ASIX offers no AX88179 driver for 2000, 98 SE or ME.

The AX88179 INFs match these VID:PIDs. XP and Vista: `0B95:1790`
(AX88179), `0B95:178A` (AX88178A), and three adapters built on them,
Sitecom `0DF6:0072`, Lenovo `17EF:304B` and Toshiba `0930:0A13`. Windows
7 adds Samsung `04E8:A100`, Belkin `050D:0128`, MCT `0711:0179` and
Allied Telesis `07C9:000E`, `07C9:000F`, `07C9:0010` and `07C9:0011`.
These INFs match `0B95:1790` at any revision. ASIX's Windows 10 driver
(4.20.1.0) tells the chips apart by revision: `REV_0100` the AX88179,
`REV_0200` the later AX88179A, `REV_0300` the AX88772D, `REV_0400` and
`REV_0500` the AX88279; it does not name the AX88179B. So the drivers
here would be offered for an AX88179A, but ASIX lists AX88179A drivers
only for Windows 8 and later, and whether these older drivers run it is
not known. ASIX documents the AX88179A as a standard CDC-NCM device as
well.

Install by pointing the Add New Hardware Wizard, or Update Driver on the
adapter, at the folder for your system. Read the chipset, not the
packaging: most modern USB-C Ethernet dongles use a Realtek RTL8153, for
which Realtek's drivers below serve XP, Vista and 7, and which has no
driver for 98 SE, ME or 2000.

The AX88772 drivers for XP x64, Vista and 7 are older builds. ASIX's
page once listed newer ones (XP x64 3.6.3.38, Vista 3.8.3.23 and
3.10.3.23). No copy of those could be found, so the newest archived
builds are here. The Vista 32-bit driver is a KMDF 1.7 driver and the 7
drivers are KMDF 1.9 drivers. Each folder carries the co-installer its
INF needs. What the INFs match:

- XP x64: `0B95:7720` (AX88772) and `0B95:772A` (AX88772A).
- Vista 32-bit: those two, MSI `0DB0:A877`, `0421:772A` and `125E:180D`.
- Vista 64-bit: `0B95:7720`, `0B95:772A` and MSI `0DB0:A877`.
- 7: `0B95:7720`, `0B95:772A`, MSI `0DB0:A877` and `0421:772A`.

ASIX's other USB 2.0 chips, one folder per system, each as ASIX
released it:

| Folder | Systems | Driver | Chips (VID:PID) |
|---|---|---|---|
| `ax88772b/w2k-xp/` | Windows 2000 and XP, 32-bit | `ax88772b.sys` 5.4.3.0 (2010-05-21) | AX88772B (`0B95:772B`) |
| `ax88772b/wxp64/` | Windows XP x64 | `ax88772b.sys` 5.6.3.0 (2010-05-21) | AX88772B |
| `ax88772b/wvista/` | Windows Vista, 32-bit | `ax88772b.sys` 5.8.2.0 (2010-05-21) | AX88772B |
| `ax88772b/wvista64/` | Windows Vista, 64-bit | `ax88772b.sys` 5.10.2.0 (2010-05-21) | AX88772B |
| `ax88772b/w7/` | Windows 7, 32-bit | `ax88772b.sys` 5.12.12.0 (2015-05-14) | AX88772B and AX88772C (`0B95:772B` revisions `0001` and `0002`, `0B95:7E2B`), D-Link `2001:1A02` |
| `ax88772b/w7_64/` | Windows 7, 64-bit | `ax88772b.sys` 5.14.12.0 (2015-05-14) | as `w7/` |
| `ax88178/w98se-me/` | Windows 98 SE and ME | `ax88178.sys` 1.0.3.46 (2005-01-18) | AX88178 (`0B95:1780`) |
| `ax88178/w2k-xp/` | Windows 2000 and XP, 32-bit | `ax88178.sys` 1.4.3.64 (2010-11-24) | AX88178 |
| `ax88178/wxp64/` | Windows XP x64 | `ax88178.sys` 1.6.3.64 (2010-11-24) | AX88178 |
| `ax88178/wvista/` | Windows Vista, 32-bit | `ax88178.sys` 1.8.3.14 (2010-11-24) | AX88178 |
| `ax88178/wvista64/` | Windows Vista, 64-bit | `ax88178.sys` 1.10.3.14 (2010-11-24) | AX88178 |
| `ax88178/w7/` | Windows 7, 32-bit | `ax88178.sys` 1.12.6.0 (2013-07-12) | AX88178 |
| `ax88178/w7_64/` | Windows 7, 64-bit | `ax88178.sys` 1.14.6.0 (2013-07-12) | AX88178 |
| `ax88172/w98se-me/` | Windows 98 SE and ME | `ax88172.sys` 1.0.0.11 (2003-07-04) | AX88172 (`0B95:1720`) |
| `ax88172/w2k/` | Windows 2000 | `ax88172.sys` 2.3.0.2 (2003-07-02) | AX88172 |
| `ax88172/wxp/` | Windows XP, 32-bit | `AX88172.SYS` 2.0.0.5 (2003-05-22) | AX88172 |
| `ax88172a/w2k-xp/` | Windows 2000 and XP, 32-bit | `AX88172A.sys` 1.4.0.6 (2010-06-02) | AX88172A (`0B95:172A`) |
| `ax88172a/wxp64/` | Windows XP x64 | `AX88172A.sys` 1.6.0.6 (2010-06-02) | AX88172A |
| `ax88172a/wvista/` | Windows Vista, 32-bit | `AX88172A.sys` 1.8.0.5 (2010-06-02) | AX88172A |
| `ax88172a/wvista64/` | Windows Vista, 64-bit | `AX88172A.sys` 1.10.0.5 (2010-06-02) | AX88172A |
| `ax88172a/w7/` | Windows 7, 32-bit | `AX88172A.sys` 1.12.0.2 (2010-06-02) | AX88172A |
| `ax88172a/w7_64/` | Windows 7, 64-bit | `AX88172A.sys` 1.14.0.2 (2010-06-02) | AX88172A |

Where a folder has a `WdfCoInstaller` DLL, its driver needs Microsoft's
KMDF and the INF installs it from that DLL. Keep the folder's files
together. The AX88772B drivers for 2000 to Vista match `0B95:772B` at
any revision, so Windows offers them for an AX88772C too. ASIX lists the
AX88772C only for its Windows 7 driver. Whether the older drivers run it
is not known. ASIX's AX88772C driver for 7 is still on ASIX's site. The
other drivers here came from ASIX's old download server, as archived.

ASIX's AX88172 INF for 98 SE and ME begins as an NT INF does. This
project checked that Windows 98 SE reads it (2026-10-27, in a virtual
machine, with no adapter). Windows did not refuse the INF. The model
does not show in the Add New Hardware list, because ASIX's INF hides it
from manual choice, as ASIX's other 98 SE INFs do. Plug the adapter in
and point Windows at the folder when it asks for a driver. The driver
itself has not been run here.

Realtek's drivers for its USB Ethernet controllers, one folder per
system, each Realtek's whole "Auto Installation Program" as released,
with its 32-bit and 64-bit drivers together:

| Folder | Systems | Driver | INFs |
|---|---|---|---|
| `rtl815x/wxp/` | Windows XP, 32- and 64-bit | 5.23 (`DriverVer` 2018-01-23) | `WINXP\32\rtuxp.INF`, `WINXP\64\rtuxp.INF` |
| `rtl815x/wvista/` | Windows Vista, 32- and 64-bit | 6.27 (`DriverVer` 2017-12-12) | `WINVISTA\32\rtux86lh.INF`, `WINVISTA\64\rtux64lh.INF` |
| `rtl815x/w7/` | Windows 7, 32- and 64-bit | 7.61.20 (`DriverVer` 2021-11-02) | `WIN7\32\rtump62x86sta.INF`, `WIN7\64\rtump62x64sta.INF` |

Install by pointing Update Driver on the adapter at the INF's folder,
for example `rtl815x\wxp\WINXP\32\`; or run the folder's `setup.exe`,
Realtek's InstallShield setup, which has not been tried here.

What the INFs match:

- XP and Vista: Realtek's `0BDA:8152` and `0BDA:8050` (RTL8152B, Fast
  Ethernet), revisions `20xx`, and `0BDA:8153` (RTL8153 family,
  Gigabit), revisions `30xx` and `31xx`. Each of those three is also
  listed without a revision, so it matches any revision. Both list the
  same 31 adapter VID:PIDs from 12 other vendors (Lenovo, TP-Link,
  D-Link, Belkin, Samsung, LG and others), each at a fixed revision.
- 7: the same, and `0BDA:8153` at revisions `32xx`, `33xx` and `F100`,
  `0BDA:8053` (`33xx`), `0BDA:8155`, and `0BDA:8156` and `0BDA:8056`
  (RTL8156, 2.5 Gigabit), with 67 adapter VID:PIDs from 29 other
  vendors.

The INFs give every RTL8153 revision the one name, "Realtek USB GbE
Family Controller", and do not say which chip each revision is. The
RTL8153B is generally reported with revision `3100` (its USB `bcdDevice`),
which all three INFs list; that mapping is not Realtek's and has not been
checked here. The Windows 7 driver itself has code paths named for the
RTL8153B/C ("RT8153BC") and RTL8156B; the XP and Vista drivers carry no
such names. None has been tried with an adapter here.

Realtek's driver for its older USB 1.1 chip, the RTL8150, is in
`rtl8150/w98se-vista/`. It is Realtek's whole package 5.126 as released,
with one folder per system:

| INF folder | Systems | Driver |
|---|---|---|
| `WIN98\` | Windows 98 SE | `RTL8150.SYS` 5.120 (`DriverVer` 2004-03-19) |
| `WINME\` | Windows ME | `RTL8150.SYS` 5.120 (`DriverVer` 2004-03-19) |
| `WIN2000\` | Windows 2000 | `RTL8150.SYS` 5.126 (`DriverVer` 2008-04-11) |
| `WINXP\` | Windows XP, 32- and 64-bit | `RTL8150.SYS` and `rtl8150x64.sys` 5.126 |
| `WINVISTA\32\` | Windows Vista, 32-bit. Also offered here for 7, 32-bit | `RTL8150.SYS` 5.126 |
| `WINVISTA\64\` | Windows Vista, 64-bit. Also offered here for 7, 64-bit | `rtl8150x64.sys` 5.126 |

Every INF matches Realtek's `0BDA:8150` only. Adapters sold under other
makers' USB IDs are not matched. Realtek lists the package for 98 SE to
Vista and offers no driver for 7. Its Vista INFs do not exclude 7, so
this pack also offers them for 7. That use is not Realtek's and has not
been tried. Install by pointing Update Driver at the INF's folder. The
package's `SETUP.EXE` is Realtek's InstallShield setup and has not been
tried here.

### `mcs7830/` - MosChip MCS7830, MCS7832, MCS7730

The MosChip line is now ASIX's. These are the drivers ASIX offered for
it, one folder per system, each as released:

| Folder | Systems | Driver |
|---|---|---|
| `mcs7830/w98se-xp/` | Windows 98 SE, ME, 2000 and XP, 32-bit | 1.49.0.0 (2012-05-25). One INF, `netmosu.inf`. It installs `MOSMAC98.SYS` on 98 SE and ME and `mosumac.sys` on 2000 and XP |
| `mcs7830/wxp64/` | Windows XP x64 | `USBMAC64.sys` 1.49.0.0 (2012-05-25) |
| `mcs7830/wvista/` | Windows Vista, 32-bit | `mosumac.sys`, `DriverVer` 1.0.0.18 (2011-08-09), KMDF 1.9 |
| `mcs7830/wvista64/` | Windows Vista, 64-bit | `USBMAC64.sys`, `DriverVer` 1.0.0.18 (2011-08-09), KMDF 1.9 |
| `mcs7830/w7/` | Windows 7, 32-bit | `mosumac.sys`, `DriverVer` 1.0.0.17 (2010-06-01) |
| `mcs7830/w7_64/` | Windows 7, 64-bit | `USBMAC64.sys`, `DriverVer` 1.0.0.17 (2010-06-01) |

Every INF matches `9710:7830` (MCS7830), `9710:7832` (MCS7832) and
`9710:7730` (MCS7730). Install by pointing Update Driver at the folder.

### `dm96xx/` - Davicom DM9601 and DM962x

Davicom's drivers, as released, except `wxp-7/` (below):

| Folder | Systems | Driver | VID:PIDs |
|---|---|---|---|
| `dm96xx/w98se-2k/` | Windows 98 SE, ME and 2000 | `DM9USB.sys` 5.0.1.0 (2012-11-21). One INF for all three | `0A46:9601`, `9620`, `9621`, `9622`, `0269`, `1269` |
| `dm96xx/wxp/` | Windows XP, 32-bit | `DM9USB.SYS` 1.90 (2002-03-12) | `0A46:9601` only |
| `dm96xx/wxp-7/Winxp/` | Windows XP, 32-bit | `DM9USB.sys`, `DriverVer` 5.0.2.0709 (2012-07-09), KMDF 1.9 | `0A46:9620`, `9621`, `0267`, `0268`, `0269`, `1267`, `1268`, `1269` |
| `dm96xx/wxp-7/XP_x64/` | Windows XP x64 | as `Winxp/` | as `Winxp/` |
| `dm96xx/wxp-7/Vista_x86/` | Windows Vista, 32-bit | `DM9USB.sys`, `DriverVer` 5.0.2.0406 (2012-04-06), KMDF 1.9 | `0A46:9620`, `9621`, `9622`, `0267`, `0268`, `1267`, `1268`, `1269` |
| `dm96xx/wxp-7/Vista_x64/` | Windows Vista, 64-bit | as `Vista_x86/` | as `Vista_x86/` |
| `dm96xx/wxp-7/Win7_x86/` | Windows 7, 32-bit | `DM9USB.sys`, `DriverVer` 5.0.3.0703 (2012-07-03), KMDF 1.9 | as `Winxp/` |
| `dm96xx/wxp-7/Win7_x64/` | Windows 7, 64-bit | as `Win7_x86/` | as `Winxp/` |
| `dm96xx/wxp-7/Win2k/` | Windows 2000 | `DM9USB.sys`, `DriverVer` 3.0.2.0416 (2010-04-16) | `0A46:9601`, `9620`, `9621`, `9622` |

`0A46:9601` is the DM9601. The others are the DM9620, DM9621, DM9621A
and DM9622 and their variants. The INFs do not name each chip. On 2000,
use `w98se-2k/`. It is newer than `wxp-7/Win2k/` and matches more IDs.

`wxp-7/` comes from Davicom's "DM96xx Driver V1.0.4.0", which Davicom
released as one installer program. This project unpacked the installer
with 7-Zip, without running it, and keeps only its per-system driver
folders, otherwise unchanged. The installer itself, its setup programs
and its Windows 8 folders are not here. Install by pointing Update
Driver at the folder for your system.

## `non-free/serial/` - USB serial bridges

Vendors' virtual COM port drivers for their USB serial chips, each as the
vendor released it:

| Folder | Systems | Driver | Chips |
|---|---|---|---|
| `ftdi/w98se-me/` | Windows 98 SE and ME | FTDI VCP 1.09.06 (2004-11-25) | FT8U232AM, FT8U245AM, FT232BM, FT245BM, FT232R, FT245R; not FT2232 |
| `ft2232d/w98se-me/` | Windows 98 SE and ME | FTDI VCP 1.0.3 (2004-03-12) | FT2232D only |
| `ftdi/w2k/` | Windows 2000 | FTDI CDM 2.06.00 (2009-10-22), WHQL certified | FT232R and earlier single-port chips, FT2232, FT4232H; not FT232H or FT-X |
| `ch341/w98se-xp/` | Windows 98 SE, ME, 2000 and XP | WCH CH341SER 3.7 (2022-03-02) | CH340G/T/C/N/K/E/B, CH341A/F/T/B/C/U |

The chip lists are FTDI's, from its driver page of the time. The INFs
match FTDI's vendor ID `0403`: VCP 1.09.06 with product IDs `6001`,
`8372`, `6007`, `6008`, `6009` and `0232`; VCP 1.0.3 with `6010`
(interfaces `MI_00` and `MI_01`, one COM port each); CDM 2.06.00 with
`6001`, `6010` (two interfaces) and `6011` (four interfaces). CDM 2.06.00
lacks `6014` (FT232H) and `6015` (FT-X). The WCH chip list is WCH's,
from its download page; `CH341SER.INF` matches `1A86:7523`, `1A86:5523`,
`1A86:7522`, `1A86:E523` and `4348:5523`.

Install by pointing the Add New Hardware Wizard, or Update Driver on the
device, at the folder:

- VCP 1.09.06: `FTDIBUS.INF` installs the USB device, and `FTDIPORT.INF`
  then installs its COM port.
- VCP 1.0.3: `FTCUSB.INF` installs each USB interface, and `FTCSER.INF`
  then installs its COM port. The package also carries FTDI's Windows
  2000 and XP files for the same chip (`FTCSER2K.SYS` and others); this
  repository offers it for 98 SE and ME, as FTDI's page did.
- CDM 2.06.00: `ftdibus.inf` installs the USB device, and `ftdiport.inf`
  then installs its COM port. The 32-bit files are in `i386\`; FTDI's
  64-bit build in `amd64\` is shipped too, as FTDI laid the package out,
  though no system this repository covers uses it.
- CH341SER 3.7: `CH341SER.INF` installs the device as a COM port on every
  system: through `CH341S98.SYS` and `CH341SER.VXD` on 98 SE and ME, and
  `CH341SER.SYS` on 2000 and XP. WCH ships the package for Windows 98 to
  11, so it also carries 64-bit and ARM64 files, its own setup programs
  (`SETUP.EXE`, `DRVSETUP64\`), and a second set of the driver files in
  `WIN 1X\`; all are kept as WCH shipped them. Point Windows at the
  folder itself. `WIN 1X\` holds the same `CH341SER.INF` and
  `CH341SER.VXD`, byte for byte, and the same builds of the other
  drivers and DLLs (same versions and build dates, identical once their
  signatures are set aside); only their Microsoft signatures differ,
  under Microsoft's "Third Party Component CA 2014" where the folder's
  own are under its 2012 CA, presumably for Windows 10 and 11.

`FTDIBUS.INF` (VCP 1.09.06) lists `ftlang.dll` in its
`[SourceDisksFiles]`, and FTDI's package does not carry it. It is not
needed: no `CopyFiles` section of the INF names it (and `FTDIPORT.INF`
has the same line commented out), so Windows never asks for it.
Likewise `FTCSMOU.INF` (VCP 1.0.3) names a catalog, `ftcsmou.cat`, that
FTDI's package does not carry; 98 SE and ME install it without one.

On 98 SE and ME, `FTDIBUS.INF` and `FTCUSB.INF` each copy their port
and serial-mouse INFs into Windows' INF folder when they install. The
two packages' serial-mouse INFs (`FTSERMOU.INF`, `FTCSMOU.INF`) match
the same eleven `SERENUM\FTSM...` IDs, so [STAGE.TXT](STAGE.TXT) stages
neither.

## `non-free/hid/` - Xbox 360 controllers

Masahiko Morii's unofficial drivers for Xbox 360 controllers, which make
a pad a DirectInput game controller with force feedback, in his final
builds: `x360c/` for wired pads (2010-05-04) and `x360wc/` for the Xbox
360 Wireless Gaming Receiver (2010-03-21). One folder per build, each
Morii's English zip, unmodified. They come from a mirror of Morii's site
that he sanctioned in writing; NOTICE.md records why and quotes his
permission.

| Folder | Systems | Morii's file |
|---|---|---|
| `x360c/w98se-me/` | Windows 98 SE and ME | `x360c.w98.x86.en.zip` |
| `x360c/w2k/` | Windows 2000 SP4 | `x360c.w2k.x86.en.zip` |
| `x360c/wxp/` | Windows XP SP3, 32-bit | `x360c.wxp.x86.en.zip` |
| `x360c/wxp64/` | Windows XP Professional x64 Edition | `x360c.wnet.x64.en.zip` |
| `x360c/wvista/` | Windows Vista SP2, 32-bit | `x360c.wlh.x86.en.zip` |
| `x360c/wvista64/` | Windows Vista SP2, 64-bit | `x360c.wlh.x64.en.zip` |
| `x360c/w7/` | Windows 7, 32-bit | `x360c.win7.x86.en.zip` |
| `x360c/w7_64/` | Windows 7, 64-bit | `x360c.win7.x64.en.zip` |
| `x360wc/w2k/` | Windows 2000 | `x360wc.w2k.x86.en.zip` |
| `x360wc/wxp/` | Windows XP, 32-bit | `x360wc.wxp.x86.en.zip` |
| `x360wc/wxp64/` | Windows XP Professional x64 Edition | `x360wc.wnet.x64.en.zip` |
| `x360wc/wvista/` | Windows Vista, 32-bit | `x360wc.wlh.x86.en.zip` |
| `x360wc/wvista64/` | Windows Vista, 64-bit | `x360wc.wlh.x64.en.zip` |
| `x360wc/w7/` | Windows 7, 32-bit | `x360wc.win7.x86.en.zip` |
| `x360wc/w7_64/` | Windows 7, 64-bit | `x360wc.win7.x64.en.zip` |

Every `x360c` build matches the same 25 pads, as its INFs name them
(on 98 SE and ME across three INFs: `x360c.inf` for the Microsoft,
Logitech and Saitek pads, `x360c_hori.inf` for HORI's, `x360c_mdcz.inf`
for Mad Catz's):

| VID:PID | Pad |
|---|---|
| `045E:028E` | Microsoft Xbox 360 Controller |
| `046D:C242` | Logitech ChillStream |
| `0738:4716` | Mad Catz Xbox 360 Game Pad |
| `0738:4718` | Mad Catz Street Fighter IV Arcade FightStick |
| `0738:4726` | Mad Catz Xbox 360 Game Pad Pro |
| `0738:4728` | Mad Catz Street Fighter IV FightPad |
| `0738:4736` | Mad Catz Xbox 360 MicroCon Game Pad Pro |
| `0738:4738` | Mad Catz Street Fighter IV Arcade FightStick Tournament Edition |
| `0738:A728` | Mad Catz FightPad |
| `0738:CB02` | Saitek Cyborg Rumble Pad |
| `0F0D:000A` | HORI DEAD OR ALIVE 4 STICK |
| `0F0D:000B` | HORI STEERING CONTROLLER EX |
| `0F0D:000C` | HORI HORIPAD EX TURBO |
| `0F0D:000D` | HORI FIGHTING STICK EX2 |
| `0F0D:000F` | HORI FLIGHT STICK EX |
| `0F0D:0016` | HORI REAL ARCADE PRO. EX |
| `0F0D:0031` | HORI HYPER STICK PRO |
| `1BAD:F028` | Mad Catz FightPad |
| `1BAD:F029` | Mad Catz FightPad |
| `1BAD:F039` | Mad Catz Arcade FightStick Tournament Edition |
| `1BAD:F500` | HORI TWIN STICK EX |
| `1BAD:F501` | HORI HORIPAD EX2 TURBO |
| `1BAD:F502` | HORI REAL ARCADE PRO. VX-SA |
| `1BAD:F504` | HORI REAL ARCADE PRO. EX |
| `1BAD:F506` | HORI REAL ARCADE PRO. EX Premium VLX |

`x360wc` matches the receiver, `045E:0719` ("Microsoft Xbox 360 Wireless
Controller"), in every build, and from XP on also `045E:028F`
("Microsoft Xbox 360 Play & Charge Kit"), the wireless pad's charging
cable. Morii's page says the receiver driver does not show battery state
and gives the wireless racing wheel no force feedback.

The readmes are in Japanese; the `.en` builds have an English control
panel. Install by pointing the Add New Hardware Wizard, or Update Driver
on the pad or receiver, at the folder for your system (on Vista and 7,
through "Have Disk"). Morii's readme lists these known problems: on some
NVIDIA nForce 400-series chipsets the pad can stop responding after
sleep or hibernation; friction, damper, inertia, spring, custom-force and
effect-direction force feedback are not supported; XInput and the Xbox
360 headset are not supported. Morii's page adds that if a direction
stays pressed after replacing Microsoft's driver, the DirectInput
calibration needs resetting in Game Controllers.

## Where each package comes from

Each driver was taken unmodified from its maker's official download (or,
where that no longer exists, an archived or author-approved copy). [NOTICE.md](NOTICE.md)
gives the exact source, version, date and file hashes for every one.

## Not shipped: download these from the vendor

These drivers exist at their vendors' official URLs, as archived by the
Internet Archive and found on 2026-10-20, but their licences rule out
shipping them here. Download each from the archived URL yourself, check
it against the size and SHA-256 given, and read its licence before using
it. Microchip's Ethernet drivers (the last section) are left out for
another reason: their terms could not be read.

### Silicon Labs CP210x, Windows 98 SE

CP210x VCP driver 4.28a, "Silicon Laboratories CP210x VCP Drivers for
Windows 98 SE", an InstallShield installer:

- `CP210x_VCP_Win98SE.exe`, 2,521,644 bytes, SHA-256
  `665be3f6c2e54609e21b437437499ad949a8468e952cb8c03e58b5a7b7d798d9`:
  <https://web.archive.org/web/20070104000157/http://www.silabs.com/public/documents/software_doc/drivers/Microcontrollers/Interface/en/CP210x_VCP_Win98SE.exe>
  (linked from Silicon Labs' VCP page,
  <https://web.archive.org/web/20060810152808/http://www.silabs.com/tgwWebApp/public/web_content/products/Microcontrollers/USB/en/mcu_vcp.htm>).

Why not shipped: its `License_Agreement_DLL.txt` (read from the
installer's cabinets with unshield 1.6.2, without running the installer)
allows you to "Distribute copies of the Software, provided the Software
is incorporated into Licensee's product and is not distributed as a stand
alone product."

### Prolific PL2303, Windows 98, ME, 2000 and XP

PL-2303 driver 2.0.0.19 for 98 and ME, with 2.0.2.1 for 2000 and XP, in
"PL-2303 Driver Installer", an InstallShield installer in a zip:

- `wd_pl2303h-hx-x_v20019v2021.zip`, 1,506,495 bytes, SHA-256
  `18ac0f6dcb3e9c437a13bc6c130bd299e0c013ae3bd85981261088eb88eeea8c`:
  <https://web.archive.org/web/20051126015256/http://www.prolific.com.tw/support/files/%5CIO%20Cable%5CPL-2303%5CDrivers%20-%20Generic%5CWindows%5Cwd_pl2303h-hx-x_v20019v2021.zip>.

Why not shipped: Prolific's EULA
(<https://web.archive.org/web/20091229213202/http://www.prolific.com.tw/support/files/%5CIO%20Cable%5CPL-2303%5CDrivers%20-%20Generic%5CEULA.pdf>)
grants only "a non-exclusive right to install PL-2303 Drivers ... on any
computer" and says "You may not rent, lease, sublicense, modify, alter,
reverse engineer, disassemble, decompile, or create any derivative work of
the SOFTWARE".

### M-Audio MidiSport, Windows 98, ME, 2000 and XP

The USB MidiSport interfaces need firmware loaded at each plug-in. M-Audio
(then Midiman) shipped the loader, with its firmware, and the MIDI driver
in one self-extracting ZIP per model; each one's `#INSTALL.TXT` covers
Windows XP, 2000, ME, 98 SE and 98. The newest of each found on M-Audio's
server:

| Model | File | Size (bytes) | SHA-256 | Archived URL |
|---|---|---|---|---|
| MidiSport 1x1 | `Midisport1x1_1.08.EXE` | 135,178 | `67be18f1650f386fcf4cd2cf0c1d08b15cb6f196bd032a01afc5ec359d6e34e5` | <https://web.archive.org/web/20040629172913/http://www.m-audio.com/images/global/drivers/Midisport1x1_1.08.EXE> |
| MidiSport 2x2 | `Midisport 2x2_4.1.09.EXE` | 251,163 | `29b06f28b7a7d38547eb50906e081b881caaf2554f2cbd192b95259044de7059` | <https://web.archive.org/web/20040629165751/http://www.m-audio.com/images/global/drivers/Midisport%202x2_4.1.09.EXE> |
| MidiSport 4x4 | `Midisport 4x4_4.1.09.EXE` | 252,671 | `d852b402be7eede5a0dc2c5a6cde5137bb892af705fb75c9f56c7af4141cb3b2` | <https://web.archive.org/web/20040629173544/http://www.m-audio.com/images/global/drivers/Midisport%204x4_4.1.09.EXE> |
| MidiSport 8x8 | `MS8x8_4115.EXE` | 254,459 | `f1a55a45e4e78b16e2a7b5a16d68e588b0c6fac2724cdde2c201e5ccd619943b` | <https://web.archive.org/web/20040114214631/http://www.m-audio.com/images/global/drivers/MS8x8_4115.EXE> |

`Midisport 1x1_4.1.09.EXE` on the same server is mislabelled: it holds
the driver for the MidiSport 8x8/S serial interface (`MIDSPRT8.SYS`,
`OEMSETUP.INF`), not the USB 1x1. Its archived copy is
<https://web.archive.org/web/20040212225723/http://www.m-audio.com/images/global/drivers/Midisport%201x1_4.1.09.EXE>
(68,567 bytes, SHA-256
`84c3668fade78acf78eaa381cf0475c3ad1de9715a4514c56108519af7eb3880`).
M-Audio's later driver pages link "web" installers (`MS2x2_1010_web.exe`
and others) instead; those are Setup Factory installers and were not
examined.

Why not shipped: M-Audio's driver licence
(<https://web.archive.org/web/20041227061225/http://m-audio.com/index.php?do=support.driverlicense&ID=202>)
says "You may NOT publish, display, disclose, rent, lease, modify, loan,
distribute, or create derivative works based on the Software or any part
thereof."

### Microchip LAN9500 and LAN7800 families, Windows XP to 7

Microchip's (formerly SMSC's) Windows driver packages for its USB
Ethernet chips. Each zip holds drivers for several systems, including 8
and 10:

- LAN9500 family (`0424:9500`, `9505`, `9530`, `9535`, `9730`, `9735`,
  `9900` to `9906`, `9E00`, `9E01`, `9E08`, `9E09`, `EC00`): XP 32- and
  64-bit 2.6.5.0, Vista 2.11.0.0, 7 2.17.0.0.
  `lan9500-wdf-v18.12.18.0.zip`, 13,380,608 bytes, SHA-256
  `a2728876845a4476a51004119d193faa21cf86206d5ad35ccefc5af684404ee5`:
  <https://web.archive.org/web/20200816184737/http://ww1.microchip.com/downloads/en//softwarelibrary/obj-lan95xx-windows/lan9500-wdf-v18.12.18.0.zip>
- LAN7800 family (`0424:7800`, `7801`, `780A`, `7850`): Vista 3.5.2.0,
  7 3.8.4.0. No XP driver.
  `lan7800-wdf-v18.12.14.0.zip`, 10,380,378 bytes, SHA-256
  `01b50282c8a129cdee586b9c59f0999e9a217b4fe8059a97b4bd1f0a0b59234e`:
  <https://web.archive.org/web/20200816184807/http://ww1.microchip.com/downloads/en//softwarelibrary/obj-lan78xx-windows/lan7800-wdf-v18.12.14.0.zip>

Why not shipped: no licence file is in either zip. Microchip's download
pages refused this project's requests (2026-10-27), so any terms they
show were not read (the repository owner's decision, 2026-10-27).

## Checking the files

```sh
sha256sum -c SHA256.TXT
```

`.gitattributes` keeps every file byte for byte, so a checkout matches the
hashes whatever the local line-ending setting.

## Releases

Each release is a zip of the repository's files at its tag, made with
`git archive --format=zip -o usb-wdm-nonfree-<version>.zip <tag>`, so the
same command at the same tag gives the same bytes. Its hash is recorded
here, in the commit after the tag (a zip cannot hold its own hash):

| Version | Tag | File | Size (bytes) | SHA-256 |
|---|---|---|---|---|
| 1.0.0 | `v1.0.0` (commit `128106f`) | `usb-wdm-nonfree-v1.0.0.zip` | 40,860,928 | `31756d03326ea003c10c4b17f52f38883c8f4675aa629f03e93e46eb9b07ece9` |
