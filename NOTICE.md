# Notice

## The driver files are not this repository's to license

Every file under `non-free/` belongs to its authors, not to the owner of this
repository, and so does every file in `nusb33/w98se/` (below). Each
folder under `non-free/` has its table below, and each package its
provenance record (README.md, "Where each package comes from"); a package
added later adds both. Searches recorded below were made on 2026-10-20,
except where a package says otherwise.

### `nusb33/`, kept apart

NUSB 3.3's seven Windows 98 SE USB storage files are not under
`non-free/`: they sit at the repository's root in `nusb33/w98se/`, with
their own notice and provenance in [nusb33/NOTICE.md](nusb33/NOTICE.md)
(moved there from this file on 2026-10-22). They are a special case: six
are Microsoft's, from Windows Millennium (two of them INFs that NUSB's
author edited), the seventh a third party's, no licence to redistribute any of them has been found, the repository's
owner has accepted that risk for them, and the xHCI98 project's base
release download carries them on their own, while `non-free/` is offered
separately (owner, 2026-10-22).

### `non-free/ethernet/`

| File | Whose | Version |
|---|---|---|
| `ax88772/w98se-me/AX88772.SYS`, `Ax88772.inf` | ASIX Electronics Corporation | 3.0.3.12 |
| `ax88772/w2k-xp/ax88772.sys`, `Ax88772.inf`, `ax88772.cat`, `history.txt` | ASIX Electronics Corporation | 3.4.3.38 |
| `ax88772/w2k-xp/WdfCoInstaller01007.dll` | Microsoft Corporation, the KMDF 1.7 co-installer, as ASIX ships it with that driver | 1.7.6001.0 |
| `ax88179/wxpvis/` and `ax88179/wxpvis64/`: `ax88179_178a.sys`, `Ax88179_178a.inf`, `ax88179_178a.cat`, `history.txt`, `Readme.txt` | ASIX Electronics Corporation | 1.4.2.0 (32-bit), 1.6.2.0 (64-bit) |
| `ax88179/wxpvis/WdfCoInstaller01009.dll`, `ax88179/wxpvis64/WdfCoInstaller01009.dll` | Microsoft Corporation, the KMDF 1.9 co-installer, as ASIX ships it with that driver | 1.9.7600.16385 |
| All 4 files in `ax88179/w7/` and in `ax88179/w7_64/` | ASIX Electronics Corporation | 1.12.11.0 (32-bit), 1.14.11.0 (64-bit) |
| All 73 files in `rtl815x/wxp/` | Realtek Semiconductor Corp.; its setup engine (`setup.exe`, `ISSetup.dll`, `data1.cab` and the files with them) is Flexera's InstallShield, as Realtek ships it | 5.23 (`rtuxp.INF` `DriverVer` 01/23/2018,5.23.0123.2018) |
| All 73 files in `rtl815x/wvista/` | as `rtl815x/wxp/` | 6.27 (`rtux86lh.INF` `DriverVer` 12/12/2017,6.27.1212.2017) |
| All 92 files in `rtl815x/w7/` | as `rtl815x/wxp/` | 7.61.20 (`rtump62x86sta.INF` `DriverVer` 11/02/2021,7.61.20.1102) |
| All 3 files in `ax88772/wxp64/`, all 4 in `ax88772/wvista64/`; in `ax88772/wvista/`, `w7/` and `w7_64/` all files but the co-installer | ASIX Electronics Corporation | 3.6.3.18 (XP x64), 3.8.3.22 (Vista), 3.10.3.14 (Vista x64), 3.12.3.2 (7), 3.14.3.2 (7 x64) |
| `ax88772/wvista/WdfCoInstaller01007.dll` | Microsoft Corporation, the KMDF 1.7 co-installer, as ASIX ships it with that driver | 1.7.6001.0 |
| `ax88772/w7/WdfCoInstaller01009.dll`, `ax88772/w7_64/WdfCoInstaller01009.dll` | Microsoft Corporation, the KMDF 1.9 co-installer, as ASIX ships it with that driver | 1.9.7100.0 |
| All 6 files in each of `ax88772b/w2k-xp/`, `wxp64/`, `wvista/`, `wvista64/`, all 4 in each of `ax88772b/w7/`, `w7_64/` | ASIX Electronics Corporation (`WdfCoInstaller01007.dll`, 1.7.6001.0: Microsoft Corporation, as ASIX ships it) | 5.4.3.0, 5.6.3.0, 5.8.2.0, 5.10.2.0, 5.12.12.0, 5.14.12.0 |
| Both files in `ax88178/w98se-me/`, all 4 in each of `w2k-xp/`, `wxp64/`, all 5 in each of `wvista/`, `wvista64/`, `w7/`, `w7_64/` | ASIX Electronics Corporation (`WdfCoInstaller01007.dll`, 1.7.6001.0, and `WdfCoInstaller01009.dll`, 1.9.7600.16385: Microsoft Corporation, as ASIX ships them) | 1.0.3.46, 1.4.3.64, 1.6.3.64, 1.8.3.14, 1.10.3.14, 1.12.6.0, 1.14.6.0 |
| Both files in `ax88172/w98se-me/`, all 3 in each of `w2k/`, `wxp/` | ASIX Electronics Corporation | 1.0.0.11, 2.3.0.2, 2.0.0.5 |
| All 4 files in each of `ax88172a/w2k-xp/`, `wxp64/`, all 5 in each of `wvista/`, `wvista64/`, `w7/`, `w7_64/` | ASIX Electronics Corporation (`WdfCoInstaller01007.dll`, 1.7.6001.0, and `WdfCoInstaller01009.dll`, 1.9.7600.16385: Microsoft Corporation, as ASIX ships them) | 1.4.0.6, 1.6.0.6, 1.8.0.5, 1.10.0.5, 1.12.0.2, 1.14.0.2 |
| All 5 files in `mcs7830/w98se-xp/`, all 4 in each of `wxp64/`, `wvista/`, `wvista64/`, all 3 in each of `w7/`, `w7_64/` | ASIX Electronics Corporation, for MosChip Semiconductor's line (`WdfCoInstaller01009.dll`, 1.9.7600.16385: Microsoft Corporation, as shipped) | 1.49.0.0, 1.49.0.0, 1.0.0.18, 1.0.0.18, 1.0.0.17, 1.0.0.17 (`DriverVer`) |
| All 35 files in `rtl8150/w98se-vista/` | Realtek Semiconductor Corp.; its setup engine (`SETUP.EXE`, `ISSetup.dll`, `_Setup.dll`, `DATA1.CAB` and the files with them) is Flexera's InstallShield, as Realtek ships it | 5.126 (`WINXP\NET8150.INF` `DriverVer` 04/11/2008,5.126.0411.2008; `WIN98` and `WINME` 03/19/2004,5.1191.0319.2004) |
| All 3 files in `dm96xx/w98se-2k/`, all 4 in `dm96xx/wxp/` | DAVICOM Semiconductor, Inc. | 5.0.1.0; 1.90 (`DriverVer` 03/12/2002,1.90.0312.2002) |
| All 32 files in `dm96xx/wxp-7/` | DAVICOM Semiconductor, Inc. (`WdfCoInstaller01009.dll` in every folder but `Win2k/`, 1.9.7600.16385: Microsoft Corporation, as Davicom ships it) | V1.0.4.0 (`DriverVer` 5.0.2.0709 XP, 5.0.2.0406 Vista, 5.0.3.0703 7, 3.0.2.0416 2000) |

They are their makers' driver packages as released, unmodified, apart
from `dm96xx/wxp-7/` (unpacked from Davicom's installer, below).
`SHA256.TXT` lists each file's hash.

Provenance of `ax88772/w98se-me/`:

- **Vendor:** ASIX Electronics Corporation.
- **Package:** "Windows ME/98SE" driver v3.0.3.12, listed by ASIX with the
  date 2005-09-09 and size 10.6 KB (`AX88772.SYS` 3.0.3.12; the INF's
  `DriverVer` is 04/08/2004).
- **Original download location:** ASIX's official URL
  `http://www.asix.com.tw/FrootAttach/driver/AX88772_772A_WinME98SE_v3.0.3.12.zip`,
  linked from ASIX's AX88772A and AX88772 driver pages, archived at
  <https://web.archive.org/web/20130325165523/http://www.asix.com.tw/download.php?sub=driverdetail&PItemID=97>
  and
  <https://web.archive.org/web/20151208134557/http://www.asix.com.tw/download.php?sub=driverdetail&PItemID=86>.
  As of 2026-10-20 the URL redirects to ASIX's home page, ASIX's current
  site lists no Windows 98 or ME driver, and no archived copy of the zip
  itself was found.
- **Obtained:** date not recorded; the files were added here on
  2026-10-20.
- **Archive:** not kept, and no copy found to check against as of
  2026-10-20.
- **Licence:** none found. The only legal text in the files is
  `Ax88772.inf`'s "Copyright 2003-2005, ASIX Electronics Corporation".
- **Modification:** none.

Provenance of `ax88772/w2k-xp/`:

- **Vendor:** ASIX Electronics Corporation (`WdfCoInstaller01007.dll`:
  Microsoft Corporation, shipped by ASIX in the package).
- **Package:** "Windows XP/2K 32-bit Driver" v3.4.3.38, 2010-08-04, WHQL
  certified.
- **Original download location:** ASIX's official URL
  `http://www.asix.com.tw/FrootAttach/driver/AX88772A_760_772_XP2K_32bit_Driver_v3.4.3.38_WHQL.zip`,
  linked from ASIX's AX88772A driver page, archived at
  <https://web.archive.org/web/20130325165523/http://www.asix.com.tw/download.php?sub=driverdetail&PItemID=97>.
  As of 2026-10-20 the URL redirects to ASIX's home page and ASIX's
  current site lists no Windows 2000 or XP driver for this chip. Archived
  copy of the zip:
  <https://web.archive.org/web/20200303095656/https://www.asix.com.tw/FrootAttach/driver/AX88772A_760_772_XP2K_32bit_Driver_v3.4.3.38_WHQL.zip>.
- **Obtained:** the date the original copy was obtained was not recorded;
  the files were added here on 2026-10-20. On 2026-10-20 the archived copy
  above was downloaded: it holds exactly the five files in
  `ax88772/w2k-xp/`, in a folder `AX88772A_760_772_XP2K_32bit_Driver_v3.4.3.38_WHQL/`,
  and all five match `SHA256.TXT`.
- **Archive:** `AX88772A_760_772_XP2K_32bit_Driver_v3.4.3.38_WHQL.zip`
  (the archived copy; the original download was not kept), 1,103,090
  bytes, SHA-256
  `93cb4d7bce6a2ea3d4aaa00ebbdc3ff269468190a462af6b97871ecd7200defb`.
- **Licence:** none found. The zip holds no licence or EULA file;
  `history.txt` is ASIX's change log.
- **Modification:** none.

Provenance of `ax88179/` (`wxpvis/`, `wxpvis64/`, `w7/`, `w7_64/`):

- **Vendor:** ASIX Electronics Corporation (`WdfCoInstaller01009.dll`:
  Microsoft Corporation, shipped by ASIX in the XP and Vista packages).
- **Packages:** the four AX88179 drivers ASIX lists for these systems,
  each the latest for its system on ASIX's AX88179 download page on
  2026-10-20:
  - "Windows XP & Vista 32-bit Driver", "For x86 CPU platform", 1.4.2.0,
    2013-05-24 (`wxpvis/`);
  - "Windows XP & Vista 64-bit Driver", "For x64 CPU platform", 1.6.2.0,
    2013-05-24 (`wxpvis64/`);
  - "Windows 7 32-bit Driver", "For x86 CPU platform WHCK certified",
    1.12.11.0, 2018-01-19 (`w7/`);
  - "Windows 7 64-bit Driver", "For x64 CPU platform, WHCK certified",
    1.14.11.0, 2018-01-19 (`w7_64/`).

  The page also lists drivers setup programs for XP and Vista (1.0.4.0)
  and for 7 (3.0.6.0); those are not used.
- **Original download location:** ASIX's AX88179 download page,
  <https://www.asix.com.tw/en/support/download/step2/11/2/3>, and its
  official URLs, live on 2026-10-20, each served with the zip's name in
  `Content-Disposition`:
  - `https://www.asix.com.tw/en/support/download/file/1134` (XP and
    Vista 32-bit), archived at
    <https://web.archive.org/web/20240330043303/https://www.asix.com.tw/en/support/download/file/1134>;
  - `https://www.asix.com.tw/en/support/download/file/1135` (XP and
    Vista 64-bit), archived at
    <https://web.archive.org/web/20240330043322/https://www.asix.com.tw/en/support/download/file/1135>;
  - `https://www.asix.com.tw/en/support/download/file/127` (7 32-bit),
    archived at
    <https://web.archive.org/web/20210227091523/https://www.asix.com.tw/en/support/download/file/127>;
  - `https://www.asix.com.tw/en/support/download/file/128` (7 64-bit),
    archived at
    <https://web.archive.org/web/20210227094043/https://www.asix.com.tw/en/support/download/file/128>.
- **Obtained:** 2026-10-20, from ASIX's live URLs. The archived copies
  above were downloaded the same day and are byte-identical to them.
- **Archives:** each zip holds its files in one folder named after the
  zip; they are copied without that folder.
  - `AX88179_178A_WinXP_Vista_32bit_Driver_v1.4.2.0_WHQL.zip`, 1,455,013
    bytes, SHA-256
    `86272f515eefb147b60fc032e09ad261d43f2d19215e74c90b41aeef6d49e567`
  - `AX88179_178A_WinXP_Vista_64bit_Driver_v1.6.2.0_WHQL.zip`, 1,715,732
    bytes, SHA-256
    `1b4553504b898ba645a643426887cfa11c0b255ecfa309db6979cffc8ed8964d`
  - `AX88179_178A_Win7_32bit_Driver_v1.12.11.0_WHCK_20180119.zip`,
    43,942 bytes, SHA-256
    `cfcbf35f825b91cf84e45d6602065b5cbadcd7ca92961133e463a7f17522d56b`
  - `AX88179_178A_Win7_64bit_Driver_v1.14.11.0_WHCK_20180119.zip`,
    48,796 bytes, SHA-256
    `8458bf955d7be2df6df7abfb137d2848b30ae6a05ffae4c7b6ab5124162063a5`
- **Licence:** none found. The zips hold no licence or EULA file; the
  INFs carry "Copyright 2012-2013, ASIX Electronics Corporation" (XP
  and Vista) and "Copyright 2012-2017, ASIX Electronics Corporation"
  (7); `Readme.txt` describes the driver's settings and `history.txt` is
  ASIX's change log. ASIX's download page states no terms.
- **Name:** these keep ASIX's names, which are not 8.3:
  `Ax88179_178a.inf` or `AX88179_178a.inf`, `ax88179_178a.sys` or
  `AX88179_178a.sys`, `ax88179_178a.cat` and `WdfCoInstaller01009.dll`.
  The INF names each.
- **Modification:** none.

Provenance of `rtl815x/` (`wxp/`, `wvista/`, `w7/`):

- **Vendor:** Realtek Semiconductor Corp. The setup engine in each
  package is InstallShield's, as Realtek ships it.
- **Packages:** the three Windows packages Realtek lists for XP, Vista
  and 7 on its "Realtek USB FE / GBE / 2.5G / Gaming Ethernet Family
  Controller Software" page:
  - "WinXP Auto Installation Program for FE/GBE", 5.23;
  - "Vista and Server 2008 Auto Installation Program", 6.27;
  - "Win7 and Server 2008 R2 Auto Installation Program", 7.61.20.

  Each is the latest for its system: the live page
  (`https://www.realtek.com/Download/List?cate_id=585`) on 2026-10-20
  lists 5.23 dated 2021/07/27, 6.27 dated 2018/08/02 and 7.61.20 dated
  2021/12/28; as archived on 2021-10-17
  (<https://web.archive.org/web/20211017103908/https://www.realtek.com/en/component/zoo/category/network-interface-controllers-10-100-1000m-gigabit-ethernet-usb-3-0-software>)
  it listed 5.23 and 6.27 both dated 2018/03/06, and 7.59.20.
- **Original download location:** Realtek's download page hands out each
  file only after a captcha, so the link it leads to could not be
  followed on 2026-10-20. The packages used are the Internet Archive's
  copies of them on Realtek's own file server, `rtitwww.realtek.com`,
  which did not answer the host that searched on 2026-10-20:
  - <https://web.archive.org/web/20211124094743/https://rtitwww.realtek.com/rtdrivers/cn/nic/0004-Install_USB_XP_5023_01262018.zip>
  - <https://web.archive.org/web/20211124092227/https://rtitwww.realtek.com/rtdrivers/cn/nic/0006-Install_USB_Vista_6027_01102018.zip>
  - <https://web.archive.org/web/20220824051244/https://rtitwww.realtek.com/rtdrivers/cn/nic1/Install_USB_Win7_7061.20_12232021.zip>

  These are the only XP and Vista USB packages the Internet Archive holds
  from that server. Whether the files the live page now serves (dated
  2021/07/27 for XP and 2018/08/02 for Vista) are byte-identical to them
  is not known.
- **Obtained:** 2026-10-20, from the archived copies above.
- **Archives:**
  - `0004-Install_USB_XP_5023_01262018.zip`, 9,640,984 bytes, SHA-256
    `8d1a1953ae4ac069f43b120a0ef72b0656c75484702d6fa13a649b42cff3464d`.
    It holds the files in a folder `Install_USB_XP_5023_01262018/`; they
    are copied without that folder.
  - `0006-Install_USB_Vista_6027_01102018.zip`, 9,742,431 bytes, SHA-256
    `2265c11b15816833ffd8fc42bc67964fd91b8048c4bba5d29bd4a9405c1aa731`.
    It holds the files in a folder `Install_USB_Vista_6027_01102018/`;
    they are copied without that folder.
  - `Install_USB_Win7_7061.20_12232021.zip`, 5,462,174 bytes, SHA-256
    `eafaa407464ce00bcb7122580b2d01caedc89f5b229027c7731f4b794cd1bdcc`.
    It holds one file, `Install_USB_Win7_7061.20_12232021.exe`
    (5,654,368 bytes, SHA-256
    `f3da41eb53fe4ed52f03fc17ea77db6cf8938bbb7105329c4bc2500f517ea872`),
    a 7-Zip self-extracting archive. Its 92 files were unpacked with
    7-Zip, without running it, and are copied as they are.

  Each package also holds an empty folder `PATCH/`, which git does not
  keep.
- **Licence:** none found. The licence text inside each package's
  `data1.cab` (`license.rtf`, read with unshield 1.6.2 without running
  the setup) is InstallShield's placeholder: "To add your own license
  text to this dialog, specify your license agreement file in the
  Support Files/Billboards view." The INFs carry "COPYRIGHT (C)
  2007-2018 Realtek CORPORATION" (2007-2017 and 2007-2021 in the Vista
  and 7 INFs) and a list of patents covering the product. Realtek's
  download page offers these files as "direct" downloads, which show
  "The file is ready. The file will start download after click." and a
  captcha, and no terms; its other kind of download, which asks the user
  to accept the terms above it, is not used for them.
- **Name:** the long names listed in README.md keep Realtek's names, as
  its INFs and setup name them.
- **Modification:** none.

Common to the packages added on 2026-10-27 (`ax88772/` XP x64 to 7,
`ax88772b/`, `ax88178/`, `ax88172/`, `ax88172a/`, `mcs7830/`,
`rtl8150/`, `dm96xx/`): the archives were found and fetched on
2026-10-27 for the xHCI98 project's USB Ethernet survey, from the URLs
given, into a scratch folder. They were unpacked with 7-Zip, and no
installer or program in them was run. Each archive's SHA-256 below is
of the file as fetched. Where a zip holds one folder named after itself
(or a version folder), its files are copied without that folder. None of
these archives holds a licence or EULA file, except Realtek's RTL8150
package (below). The repository owner decided on 2026-10-27 that
packages which carry only their maker's copyright, and no licence text,
are added on the same basis as the ASIX and Realtek packages above.

Provenance of `ax88772/wxp64/`, `wvista/`, `wvista64/`, `w7/`, `w7_64/`:

- **Vendor:** ASIX Electronics Corporation (`WdfCoInstaller01007.dll`
  and `WdfCoInstaller01009.dll`: Microsoft Corporation, shipped by ASIX
  in the packages).
- **Packages:** ASIX's AX88772/AX88772A drivers for XP x64 (3.6.3.18,
  `DriverVer` 2007-09-21), Vista 32-bit (3.8.3.22, 2009-10-02), Vista
  64-bit (3.10.3.14, 2008-11-18), 7 32-bit (3.12.3.2, 2009-06-10) and 7
  64-bit (3.14.3.2, 2009-06-10), all marked WHQL in their names. ASIX's
  archived AX88760/AX88772A driver page (2010) listed newer builds, XP
  x64 3.6.3.38 and Vista 3.8.3.23 and 3.10.3.23. No copy of those files
  could be found, so these older builds are carried (owner, 2026-10-27).
- **Original download location:** ASIX's official URLs under
  `http://www.asix.com.tw/FrootAttach/driver/`, which no longer serve
  them. Archived copies, the ones used:
  - <https://web.archive.org/web/20110802222733/http://www.asix.com.tw/FrootAttach/driver/AX88772_772A_WinXP2K3_64bit_Driver_v3.6.3.18_WHQL.zip>
  - <https://web.archive.org/web/20111127002545/http://www.asix.com.tw/FrootAttach/driver/AX88772_772A_760_Vista_32bit_Driver_v3.8.3.22_WHQL.zip>
  - <https://web.archive.org/web/20140703183417/http://www.asix.com.tw/FrootAttach/driver/AX88772_772A_Vista_64bit_Driver_v3.10.3.14_WHQL.zip>
  - <https://web.archive.org/web/20111127002136/http://www.asix.com.tw/FrootAttach/driver/AX88772_772A_760_Win7_32bit_Driver_v3.12.3.2_WHQL.zip>
  - <https://web.archive.org/web/20111214235701/http://www.asix.com.tw/FrootAttach/driver/AX88772_772A_760_Win7_64bit_Driver_v3.14.3.2_WHQL.zip>
- **Obtained:** 2026-10-27, from the archived copies above.
- **Archives:**
  - `AX88772_772A_WinXP2K3_64bit_Driver_v3.6.3.18_WHQL.zip`, 26,708
    bytes, SHA-256
    `ce31fc3a8119d9d7df38edd8b40bb828da41498f3f6bc3bd791cee7cfffa06a7`
  - `AX88772_772A_760_Vista_32bit_Driver_v3.8.3.22_WHQL.zip`, 1,105,293
    bytes, SHA-256
    `b49f0fb05a8ccf5a33d843bbbb38bfeafb530ed861a6c18a4f570cf376b7a364`
  - `AX88772_772A_Vista_64bit_Driver_v3.10.3.14_WHQL.zip`, 33,026 bytes,
    SHA-256
    `c1b167f1b6f9dea416355e938aa1abcf4f4dac00ecc43df700fd47fe29804ba5`
  - `AX88772_772A_760_Win7_32bit_Driver_v3.12.3.2_WHQL.zip`, 1,166,729
    bytes, SHA-256
    `16e4309bfa3bb04ad182de1a600b03ce0b065e94efc5f3e010195e0cf6c64ee0`
  - `AX88772_772A_760_Win7_64bit_Driver_v3.14.3.2_WHQL.zip`, 1,428,346
    bytes, SHA-256
    `b512266a949ec00177dd0972c941f9dc156869935b1069e16055c0105882ba2c`
- **Licence:** none found. The INFs carry "Copyright 2003-2007" (XP
  x64), "Copyright 2003-2008" (Vista x64) and "Copyright 2003-2009" (the
  others), "ASIX Electronics Corporation".
- **Name:** these keep ASIX's names: `ax88772ex.cat`,
  `history_Vista64.txt` and the co-installers are not 8.3.
- **Modification:** none.

Provenance of `ax88772b/`:

- **Vendor:** ASIX Electronics Corporation (`WdfCoInstaller01007.dll`:
  Microsoft Corporation, shipped by ASIX in the packages).
- **Packages:** ASIX's AX88772B drivers for 2000 and XP 32-bit (5.4.3.0),
  XP x64 (5.6.3.0), Vista 32-bit (5.8.2.0) and Vista 64-bit (5.10.2.0),
  all `DriverVer` 2010-05-21 and marked WHQL; and ASIX's AX88772C/AX88772B
  drivers for 7 32-bit (5.12.12.0) and 64-bit (5.14.12.0), `DriverVer`
  2015-05-14, marked WHCK, the ones ASIX's AX88772C page lists today.
- **Original download location:** for 2000 to Vista, ASIX's official URLs
  under `http://www.asix.com.tw/FrootAttach/driver/`, which no longer
  serve them. Archived copies, the ones used:
  - <https://web.archive.org/web/20111106121911/http://www.asix.com.tw/FrootAttach/driver/AX88772B_XP2K_32bit_Driver_v5.4.3.0_WHQL.zip>
  - <https://web.archive.org/web/20111106122513/http://www.asix.com.tw/FrootAttach/driver/AX88772B_XP2K3_64bit_Driver_v5.6.3.0_WHQL.zip>
  - <https://web.archive.org/web/20111106121035/http://www.asix.com.tw/FrootAttach/driver/AX88772B_Vista_32bit_Driver_v5.8.2.0_WHQL.zip>
  - <https://web.archive.org/web/20111106121442/http://www.asix.com.tw/FrootAttach/driver/AX88772B_Vista_64bit_Driver_v5.10.2.0_WHQL.zip>

  For 7, ASIX's live official URLs, each served with the zip's name in
  `Content-Disposition`: `https://www.asix.com.tw/en/support/download/file/241`
  (32-bit) and `https://www.asix.com.tw/en/support/download/file/242`
  (64-bit), from ASIX's AX88772C product page.
- **Obtained:** 2026-10-27: 2000 to Vista from the archived copies, 7
  from ASIX's live URLs.
- **Archives:**
  - `AX88772B_XP2K_32bit_Driver_v5.4.3.0_WHQL.zip`, 1,108,220 bytes,
    SHA-256
    `3ee77b145333e671614519ba81789c1467b6772c3a6e6e7103c00167b2f6f367`
  - `AX88772B_XP2K3_64bit_Driver_v5.6.3.0_WHQL.zip`, 1,488,097 bytes,
    SHA-256
    `f120b772fce256fb0bfbe91da7396767b17f44954663a986cc319766a5095645`
  - `AX88772B_Vista_32bit_Driver_v5.8.2.0_WHQL.zip`, 1,113,184 bytes,
    SHA-256
    `e3b2ceb8f1cf689af666bb7099f2b48d318a0baa6c0e176d2febff3319f924b4`
  - `AX88772B_Vista_64bit_Driver_v5.10.2.0_WHQL.zip`, 1,493,165 bytes,
    SHA-256
    `19cdc77be51490383d90625048a96ff7513f76234713b8547ec99dcd944762eb`
  - `AX88772C_772B_Win7_32bit_Driver_v5.12.12.0_WHCK.zip`, 51,395 bytes,
    SHA-256
    `959f783ebe0d160b5b2693fd99b2c146de41ad0f82a1daeb24c414f75f05b370`
  - `AX88772C_772B_Win7_64bit_Driver_v5.14.12.0_WHCK.zip`, 59,790 bytes,
    SHA-256
    `79aa9496bffb0cb409c2f57539e077b47c142f12888c1358c2e53793f36f2fea`
- **Licence:** none found. The INFs carry "Copyright 2010, ASIX
  Electronics Corporation" (2010-2015 for 7); `readme.txt` or
  `Readme.txt` describes the driver's settings and `history.txt` is
  ASIX's change log. ASIX's download page states no terms.
- **Name:** these keep ASIX's names: `ax88772bex.cat` and the
  co-installer are not 8.3.
- **Modification:** none.

Provenance of `ax88178/`:

- **Vendor:** ASIX Electronics Corporation (the KMDF co-installers:
  Microsoft Corporation, shipped by ASIX in the packages).
- **Packages:** ASIX's AX88178 drivers for 98 SE and ME (1.0.3.46,
  `DriverVer` 2005-01-18), 2000 and XP 32-bit (1.4.3.64), XP x64
  (1.6.3.64), Vista 32-bit (1.8.3.14) and 64-bit (1.10.3.14), all
  2010-11-24 and marked WHQL, and 7 32-bit (1.12.6.0) and 64-bit
  (1.14.6.0), 2013-07-12, marked WHCK.
- **Original download location:** ASIX's official URLs under
  `http://www.asix.com.tw/FrootAttach/driver/` (98 SE and ME) and
  `http://asix.com.tw/FrootAttach/driver/` (the others), which no longer
  serve them. Archived copies, the ones used:
  - <https://web.archive.org/web/20060507062610/http://www.asix.com.tw:80/FrootAttach/driver/AX88178_WinME98_v1.0.3.46.zip>
  - <https://web.archive.org/web/20171108160114/http://asix.com.tw/FrootAttach/driver/AX88178_XP2K_32bit_Driver_v1.4.3.64_WHQL.zip>
  - <https://web.archive.org/web/20171108200702/http://asix.com.tw/FrootAttach/driver/AX88178_XP2K3_64bit_Driver_v1.6.3.64_WHQL.zip>
  - <https://web.archive.org/web/20171108213820/http://asix.com.tw/FrootAttach/driver/AX88178_Vista_32bit_Driver_v1.8.3.14_WHQL.zip>
  - <https://web.archive.org/web/20171108183405/http://asix.com.tw/FrootAttach/driver/AX88178_Vista_64bit_Driver_v1.10.3.14_WHQL.zip>
  - <https://web.archive.org/web/20171108154804/http://asix.com.tw/FrootAttach/driver/AX88178_Win7_Win8.x_32bit_Driver_v1.12.6.0_WHCK.zip>
  - <https://web.archive.org/web/20171108231631/http://asix.com.tw/FrootAttach/driver/AX88178_Win7_Win8.x_64bit_Driver_v1.14.6.0_WHCK.zip>
- **Obtained:** 2026-10-27, from the archived copies above.
- **Archives:** the 98 SE and ME zip holds its two files at its root.
  - `AX88178_WinME98_v1.0.3.46.zip`, 13,974 bytes, SHA-256
    `ad44af1ac38a60c0769bf63a63592699b04c5dde29192be1b69de1f6a1b20666`
  - `AX88178_XP2K_32bit_Driver_v1.4.3.64_WHQL.zip`, 28,087 bytes,
    SHA-256
    `f957ae8c8e3f72c973fe5b76fa7a710b54d1f91458cc38276c735f69b7dc790c`
  - `AX88178_XP2K3_64bit_Driver_v1.6.3.64_WHQL.zip`, 35,037 bytes,
    SHA-256
    `e4b72e43bca21894a97051469c0441f24539250db78d362c95e9bb84ac7298f6`
  - `AX88178_Vista_32bit_Driver_v1.8.3.14_WHQL.zip`, 1,100,080 bytes,
    SHA-256
    `796de3d5e29cd2c9e6e485e9b717dada8597eb62fea7f4cc8d5775afa394290e`
  - `AX88178_Vista_64bit_Driver_v1.10.3.14_WHQL.zip`, 1,477,896 bytes,
    SHA-256
    `891b94d5a4bdbf8fdeb29cfe88b750977ca284a80450611d978a87b109e9e95b`
  - `AX88178_Win7_Win8.x_32bit_Driver_v1.12.6.0_WHCK.zip`, 1,454,326
    bytes, SHA-256
    `6a3dde95aa1d2f5bccd63ca69167e00cd0b523689b40049a7259681333f5a6f2`
  - `AX88178_Win7_Win8.x_64bit_Driver_v1.14.6.0_WHCK.zip`, 1,714,600
    bytes, SHA-256
    `6220bb36412d6cef7b772e74ef907b3a90f166fdb3a77da159a21f0012ba1583`
- **Licence:** none found. The INFs carry "Copyright 2004-2005" (98 SE
  and ME), "Copyright 2004-2010" (2000 to XP x64), "Copyright 2003-2010"
  (Vista) and "Copyright 2003-2013" (7), "ASIX Electronics Corporation".
- **Name:** these keep ASIX's names: `ax88178ex.cat` and the
  co-installers are not 8.3.
- **Modification:** none.

Provenance of `ax88172/`:

- **Vendor:** ASIX Electronics Corporation.
- **Packages:** ASIX's AX88172 drivers for 98 and ME (1.0.0.11,
  `DriverVer` 2003-07-04), 2000 (2.3.0.2, 2003-07-02, WHQL) and XP
  (2.0.0.5, 2003-05-22, WHQL). The 98 and ME INF's `Signature` reads
  `"$Windows NT$"`. This project checked on 2026-10-27, in a Windows 98
  SE virtual machine with no adapter, that 98 SE reads the INF (README.md,
  the AX88172 paragraph); the driver itself has not been run.
- **Original download location:** ASIX's official URLs under
  `http://www.asix.com.tw/FrootAttach/driver/`, which no longer serve
  them. Archived copies, the ones used:
  - <https://web.archive.org/web/20060523201836/http://www.asix.com.tw:80/FrootAttach/driver/AX88172_WinME98_v1.0.0.11.zip>
  - <https://web.archive.org/web/20060523201824/http://www.asix.com.tw:80/FrootAttach/driver/AX88172_Win2K_v2.3.0.2_WHQL.zip>
  - <https://web.archive.org/web/20060523201904/http://www.asix.com.tw:80/FrootAttach/driver/AX88172_WinXP_v2.0.0.5_WHQL.zip>
- **Obtained:** 2026-10-27, from the archived copies above.
- **Archives:** each zip holds its files in a version folder
  (`v1.0.0.11/`, `v2.3.0.2_WHQL/`, `v2.0.0.5_WHQL/`), copied without it.
  - `AX88172_WinME98_v1.0.0.11.zip`, 8,811 bytes, SHA-256
    `943c46dcb0a1cec68563222962a65d49f5b072df2ae806c2edf85069d22b329b`
  - `AX88172_Win2K_v2.3.0.2_WHQL.zip`, 13,045 bytes, SHA-256
    `0df00da45898719691167faa08ccdeaeffb0b68496c2967ddd13c9c2d779af86`
  - `AX88172_WinXP_v2.0.0.5_WHQL.zip`, 12,951 bytes, SHA-256
    `eb03c248f8ea7dbc4933cd6efaa3c2426f4fabfacca76e584dde6acb473458f5`
- **Licence:** none found. The INFs carry "Copyright 2001-2003, ASIX
  Electronics Corporation".
- **Name:** these keep ASIX's names: `ax881722k.cat` and
  `ax88172xp.cat` are not 8.3.
- **Modification:** none.

Provenance of `ax88172a/`:

- **Vendor:** ASIX Electronics Corporation (the KMDF co-installers:
  Microsoft Corporation, shipped by ASIX in the packages).
- **Packages:** ASIX's AX88172A drivers for 2000 and XP 32-bit
  (1.4.0.6), XP x64 (1.6.0.6), Vista 32-bit (1.8.0.5) and 64-bit
  (1.10.0.5), and 7 32-bit (1.12.0.2) and 64-bit (1.14.0.2), all
  `DriverVer` 2010-06-02 and marked WHQL. ASIX's AX88172A product page is
  live and lists no Windows driver.
- **Original download location:** ASIX's official URLs under
  `http://asix.com.tw/FrootAttach/driver/`, which no longer serve them.
  Archived copies, the ones used:
  - <https://web.archive.org/web/20171109030053/http://asix.com.tw/FrootAttach/driver/AX88172A_XP2K_32bit_Driver_v1.4.0.6_WHQL.zip>
  - <https://web.archive.org/web/20171109040410/http://asix.com.tw/FrootAttach/driver/AX88172A_XP2K3_64bit_Driver_v1.6.0.6_WHQL.zip>
  - <https://web.archive.org/web/20171109005925/http://asix.com.tw/FrootAttach/driver/AX88172A_Vista_32bit_Driver_v1.8.0.5_WHQL.zip>
  - <https://web.archive.org/web/20171109052754/http://asix.com.tw/FrootAttach/driver/AX88172A_Vista_64bit_Driver_v1.10.0.5_WHQL.zip>
  - <https://web.archive.org/web/20171109070729/http://asix.com.tw/FrootAttach/driver/AX88172A_Win7_32bit_Driver_v1.12.0.2_WHQL.zip>
  - <https://web.archive.org/web/20171109015339/http://asix.com.tw/FrootAttach/driver/AX88172A_Win7_64bit_Driver_v1.14.0.2_WHQL.zip>
- **Obtained:** 2026-10-27, from the archived copies above.
- **Archives:**
  - `AX88172A_XP2K_32bit_Driver_v1.4.0.6_WHQL.zip`, 33,119 bytes,
    SHA-256
    `180a608be8ea7a1c3946a1fcc4eaf5ae5d50d5a1ba15f7da8e5c42b9afec13e5`
  - `AX88172A_XP2K3_64bit_Driver_v1.6.0.6_WHQL.zip`, 41,548 bytes,
    SHA-256
    `bf9164547e6ef05c2afd311fb8c26dfbf864ff01f03d433d25dbdc755370e817`
  - `AX88172A_Vista_32bit_Driver_v1.8.0.5_WHQL.zip`, 1,106,187 bytes,
    SHA-256
    `a729958ecaea1edd7634b5662305b64ffddc86bb05b898e06974520394e809c9`
  - `AX88172A_Vista_64bit_Driver_v1.10.0.5_WHQL.zip`, 1,484,548 bytes,
    SHA-256
    `898bde6066be1d53334cc4fbf97a0ba945a9260622a3e4652d71d744d71c4d40`
  - `AX88172A_Win7_32bit_Driver_v1.12.0.2_WHQL.zip`, 1,458,056 bytes,
    SHA-256
    `ca1c4a8d804c4c4071f46b58e7a297d0a76e6c2416ce62e6707fc387fcba34c9`
  - `AX88172A_Win7_64bit_Driver_v1.14.0.2_WHQL.zip`, 1,718,450 bytes,
    SHA-256
    `c17f856a8768ac0f73568b3694213c8c3477cf5825e74f9e91d151a8a31af98a`
- **Licence:** none found. The INFs carry "Copyright 2007-2010, ASIX
  Electronics Corporation".
- **Name:** these keep ASIX's names: `ax88172aex.cat` and the
  co-installers are not 8.3.
- **Modification:** none.

Provenance of `mcs7830/`:

- **Vendor:** ASIX Electronics Corporation, which took over MosChip
  Semiconductor's USB Ethernet line (`WdfCoInstaller01009.dll`:
  Microsoft Corporation, shipped in the Vista packages).
- **Packages:** the MCS7830/7832/7730 drivers on ASIX's old download
  server: "Windows XP/2000 32-bit Driver v1.49.0.0" (one INF that also
  serves 98 SE and ME, with `mosmac98.sys`) and "Windows XP/2003 64-bit
  Driver v1.49.0.0", both 2012-05-25, Vista 32- and 64-bit 1.0.0.18
  (2011-08-09) and 7 32- and 64-bit 1.0.0.17 (2010-06-01), as ASIX's
  archived MCS7830 driver page (2014) lists them.
- **Original download location:** ASIX's official URLs under
  `http://asix.com.tw/FrootAttach/driver/`, which no longer serve them.
  Archived copies, the ones used:
  - <https://web.archive.org/web/20171031193523/http://asix.com.tw/FrootAttach/driver/MCS783x_Windows_XP_32bit_Driver_v1.49.0.0_WHQL.zip>
  - <https://web.archive.org/web/20171031185302/http://asix.com.tw/FrootAttach/driver/MCS783x_Windows_XP_64bit_Driver_v1.49.0.0_WHQL.zip>
  - <https://web.archive.org/web/20171101010524/http://asix.com.tw/FrootAttach/driver/MCS783x_Vista_32bit_driver_v1.0.0.18_WHQL_20110902.zip>
  - <https://web.archive.org/web/20171101021713/http://asix.com.tw/FrootAttach/driver/MCS783x_Vista_64bit_driver_v1.0.0.18_WHQL_20110902.zip>
  - <https://web.archive.org/web/20171031191755/http://asix.com.tw/FrootAttach/driver/MCS783x_Win7_32bit_driver_v1.0.0.17_WHQL_20110902.zip>
  - <https://web.archive.org/web/20171031164337/http://asix.com.tw/FrootAttach/driver/MCS783x_Win7_64bit_driver_v1.0.0.17_WHQL_20110902.zip>
- **Obtained:** 2026-10-27, from the archived copies above.
- **Archives:**
  - `MCS783x_Windows_XP_32bit_Driver_v1.49.0.0_WHQL.zip`, 47,610 bytes,
    SHA-256
    `f8632cac2c506c34dfb7299c88c6a66f0545d2c8ec957c0b9e63a8787f7e1d8f`
  - `MCS783x_Windows_XP_64bit_Driver_v1.49.0.0_WHQL.zip`, 34,040 bytes,
    SHA-256
    `dfcbd8258abb0f526ecae49399c15b3b18b80de20054d711103b861a491ea226`
  - `MCS783x_Vista_32bit_driver_v1.0.0.18_WHQL_20110902.zip`, 1,451,221
    bytes, SHA-256
    `5747144fc5f2886dcf2710b79bd5f61adf7ea12fdf807ea799281501c7e7f333`
  - `MCS783x_Vista_64bit_driver_v1.0.0.18_WHQL_20110902.zip`, 1,711,105
    bytes, SHA-256
    `4e5355b3f5ef3aac513aed5d19f506c8bd3861f6f723acf49ab86eaa6fcf19df`
  - `MCS783x_Win7_32bit_driver_v1.0.0.17_WHQL_20110902.zip`, 32,275
    bytes, SHA-256
    `0f31509b36580d37bcbd435a67c29220a08f65b87a8eb291b7aee91b14483710`
  - `MCS783x_Win7_64bit_driver_v1.0.0.17_WHQL_20110902.zip`, 36,370
    bytes, SHA-256
    `cd179d486b2d1c5bf8201db4a15bb5ef1f1e795c7bb8d3b57f8786ab88a4cebd`
- **Licence:** none found. The INFs carry "(c) Copyright 2002 - 2012",
  "2002-2012", "2002" or "2004", with no holder named; they name
  "MosChip" as provider (XP x64: "ASIX Electronics Corporation").
- **Name:** these keep the vendor's names: `usbmac_64.cat` and the
  co-installer are not 8.3.
- **Modification:** none.

Provenance of `rtl8150/w98se-vista/`:

- **Vendor:** Realtek Semiconductor Corp. The setup engine in the package
  is InstallShield's, as Realtek ships it.
- **Package:** "Windows Driver (Support Win98SE/WinME/Win2K/WinXP/Vista)",
  listed on Realtek's RTL8150 software page with version 1.26 and the date
  2008/04/28 (archived at
  <https://web.archive.org/web/20210126192000/https://www.realtek.com/en/component/zoo/category/rtl8150l-m-software>);
  the INFs' `DriverVer` is 5.126 (2008-04-11) for 2000 to Vista and
  5.1191 (2004-03-19) for 98 SE and ME. Realtek lists no driver for 7.
  This pack also offers the Vista INFs for 7 (owner, 2026-10-27; README.md).
- **Original download location:** Realtek's own file server,
  `https://www.realtek.com/rtdrivers/cn/nic/0001-8150_INST_5_126.zip`.
  Archived copy, the one used:
  <https://web.archive.org/web/20240219063703/https://www.realtek.com/rtdrivers/cn/nic/0001-8150_INST_5_126.zip>.
- **Obtained:** 2026-10-27, from the archived copy above.
- **Archive:** `0001-8150_INST_5_126.zip`, 4,215,806 bytes, SHA-256
  `b8d07d77df1593484c7ebe2d45de6a75a0b937f083769ef4cef674ea4ffaa4ff`. It
  holds the 35 files in a folder `8150_INST_5_126/`; they are copied
  without that folder.
- **Licence:** none found. `LICENSE/LICENSE.RTF` is InstallShield's
  placeholder: "Please edit this file to add license message". The INFs
  carry "Copyright 1996-2008, Realtek Semiconductor Corporation"
  (1996-2003 for 98 SE and ME). `RELEASE_NOTE/RELEASE.TXT` is Realtek's
  change log.
- **Name:** these keep Realtek's names: `rtl8150x64.sys`, `ISSetup.dll`,
  `_Setup.dll`, `InstCtrl.txt`, `Lanset2.dat`, `LANSETV6.DAT` and the
  others named by its setup are carried as they are.
- **Modification:** none.

Provenance of `dm96xx/`:

- **Vendor:** DAVICOM Semiconductor, Inc. (`WdfCoInstaller01009.dll`:
  Microsoft Corporation, shipped by Davicom in the installer).
- **Packages:**
  - `w98se-2k/`: "DM9621A_Win982KV5.0.1.0", one INF for 98, ME and 2000,
    5.0.1.0 (2012-11-21), with Davicom's `history.txt`.
  - `wxp/`: Davicom's DM9601 "XP Logo" driver 1.90 (`DriverVer`
    2002-03-12), with its catalog and Microsoft's logo submission file
    `riverLanguageMap.xml` (the name as Davicom's zip has it).
  - `wxp-7/`: "DM96xx Driver V1.0.4.0", which Davicom released as a
    single installer program (2013). XP and XP x64 5.0.2.0709, Vista
    5.0.2.0406, 7 5.0.3.0703, 2000 3.0.2.0416.
- **Original download location:** Davicom's official URLs under
  `http://www.davicom.com.tw/userfile/24247/`, which no longer serve
  them. Archived copies, the ones used:
  - <https://web.archive.org/web/20130528124624/http://www.davicom.com.tw/userfile/24247/DM9621A_Win982KV5.0.1.0.rar>
  - <https://web.archive.org/web/20130528120714/http://www.davicom.com.tw/userfile/24247/DM9601_XP_Logo_Driver_587532_1.zip>
  - <https://web.archive.org/web/20130528120023/http://www.davicom.com.tw/userfile/24247/DM96xx_Driver_V1.0.4.0.zip>
- **Obtained:** 2026-10-27, from the archived copies above.
- **Archives:** the RAR and the XP zip hold their files at their root.
  - `DM9621A_Win982KV5.0.1.0.rar`, 20,219 bytes, SHA-256
    `3b10033f48da265123c49b7cbb7b55d4057d70078947b3a3a7294ca69969f31e`
  - `DM9601_XP_Logo_Driver_587532_1.zip`, 19,303 bytes, SHA-256
    `2b81dfe45d027baa6007277951ecb2de2338acf6a49eae53c268c575c460efc4`
  - `DM96xx_Driver_V1.0.4.0.zip`, 16,475,943 bytes, SHA-256
    `dcc2552409ef13e92225e49818c01595c6d5897df92a40a9ee8e2ea01854d497`.
    It holds one file, `DM96xx_Driver V1.0.4.0.exe` (16,667,819 bytes,
    SHA-256
    `22e2dcd3304c1b888f999f44940ca95532a718f54c107ea6822019133af7dc9e`),
    an installer with a zip archive inside.
- **Licence:** none found. The INFs carry no copyright line; they name
  "DAVICOM Semiconductor, Inc." as provider.
- **Name:** these keep Davicom's names: `riverLanguageMap.xml`, the
  folders `Vista_x86/`, `Vista_x64/` and the co-installer are not 8.3.
- **Modification:** `w98se-2k/` and `wxp/`: none. `wxp-7/`: the folders
  were unpacked from Davicom's installer by this project, with 7-Zip,
  without running it, and are otherwise unchanged (owner, 2026-10-27).
  Of the installer's `Application Folder`, only the seven per-system
  driver folders `Win2k`, `Winxp`, `XP_x64`, `Vista_x86`, `Vista_x64`,
  `Win7_x86` and `Win7_x64` are carried, each with all its files
  (including Davicom's `.pdb` symbol files). Left out: the installer
  itself, its `DPInst*.exe` setup programs, the `Install_*.bat` and
  `Uninstall_*.bat` files, the `WdfCoInstaller01009.dll` at its top, the
  `Win8_x86` and `Win8_x64` folders (Windows 8 is outside this pack), its
  empty folders (`Win98` and others) and its `SimpleInstaller.si`.

### `non-free/serial/`

| File | Whose | Version |
|---|---|---|
| All 16 files in `ftdi/w98se-me/` | Future Technology Devices International Ltd. (FTDI) | VCP 1.09.06 (`FTDIPORT.INF` `DriverVer` 11/25/2004,1.09.06) |
| All 18 files in `ft2232d/w98se-me/` | FTDI | VCP 1.0.3 (the INFs' `DriverVer` 03/12/2004,1.00.00) |
| All 23 files in `ftdi/w2k/` | FTDI | CDM 2.06.00 (`ftdibus.inf` `DriverVer` 10/22/2009,2.06.00) |
| All 24 files in `ch341/w98se-xp/` | Nanjing Qinheng Microelectronics Co., Ltd. (WCH) | CH341SER 3.7 (`CH341SER.INF` `DriverVer` 01/18/2022, 3.7.2022.01) |

Each is its vendor's driver package as released, unmodified. `SHA256.TXT`
lists each file's hash.

Provenance of `ftdi/w98se-me/`:

- **Vendor:** Future Technology Devices International Ltd. (FTDI).
- **Package:** FTDI's VCP driver for Windows 98 and ME, version 1.09.06,
  listed by FTDI with the date 25th November 2004, the chips FT232R,
  FT245R, FT232B, FT245B, FT8U232AM and FT8U245AM, and the comment "FT2232
  not supported".
- **Original download location:** FTDI's official URL
  `http://www.ftdichip.com/Drivers/VCP/Win98/R10906.zip`, linked from
  FTDI's VCP driver page, archived at
  <https://web.archive.org/web/20070610120922/http://www.ftdichip.com/Drivers/VCP.htm>.
  As of 2026-10-20 the URL, with or without `www.`, returns HTTP 403 to
  the host that searched. Archived copy:
  <https://web.archive.org/web/20070610121533/http://www.ftdichip.com/Drivers/VCP/Win98/R10906.zip>.
- **Obtained:** 2026-10-20, from the archived copy above.
- **Archive:** `R10906.zip`, 323,481 bytes, SHA-256
  `fa41bcfb2cfe2635ee59a7b33be591fa6b361360a6c95517ebf3e4c78fa57d30`. It
  holds the 16 files in a folder `R10906/`; they are copied without that
  folder.
- **Licence:** none in the archive. `FTDIBUS.INF` and `FTDIPORT.INF` carry
  "Copyright (c) 2000-2004 FTDI Ltd."; `906 Release Info.DOC` (an RTF file)
  is FTDI's revision history. FTDI's VCP driver page states no terms in
  the 2007 copy above. As archived on 2015-12-31
  (<https://web.archive.org/web/20151231095819/http://www.ftdichip.com/Drivers/VCP.htm>),
  it reads: "FTDI drivers may be used only in conjunction with products
  based on FTDI parts. FTDI drivers may be distributed in any form as long
  as license information is not modified."
- **Name:** `906 Release Info.DOC` keeps FTDI's name, which is not 8.3. It
  is an exception to the 8.3 rule, by the owner's decision of 2026-10-20.
  No INF names it.
- **Modification:** none.

Provenance of `ft2232d/w98se-me/`:

- **Vendor:** Future Technology Devices International Ltd. (FTDI).
- **Package:** FTDI's VCP driver for the FT2232D on Windows 98 and ME,
  version 1.0.3, listed by FTDI with the date 12th March 2004 and the
  comment "Only for use with Windows 98/ME. Not Microsoft WHQL certified."
  (2007), later "Only supports FT2232D devices" (2011). The package also
  holds FTDI's Windows 2000 and XP files for the chip; its
  `ReleaseNotes.doc` gives 1.00.00 (98 and ME) and 1.00.03 (2000 and XP).
- **Original download location:** FTDI's official URL
  `http://www.ftdichip.com/Drivers/VCP/Win98/FTC100103.zip`, linked from
  FTDI's VCP driver page, archived at
  <https://web.archive.org/web/20070610120922/http://www.ftdichip.com/Drivers/VCP.htm>
  and
  <https://web.archive.org/web/20111020130746/http://www.ftdichip.com/Drivers/VCP.htm>.
  As of 2026-10-20 the URL returns HTTP 403 to the host that searched.
  Archived copy:
  <https://web.archive.org/web/20060210135857/http://www.ftdichip.com/Drivers/VCP/Win98/FTC100103.zip>.
- **Obtained:** 2026-10-20, from the archived copy above.
- **Archive:** `FTC100103.zip`, 403,298 bytes, SHA-256
  `2dfb71ce39ec305708d577e846d05fb34eea80e1d0248d533fbab9736e9fd898`. Its
  18 files sit at the zip's root and are copied as they are.
- **Licence:** none in the archive. `FTCUSB.INF` and `FTCSER.INF` carry
  "Copyright (c) 2004 FTDI Ltd."; `ReleaseNotes.doc` gives contents,
  contacts and revision history. FTDI's VCP driver page, as archived on
  2011-10-20 (above), reads: "FTDI drivers may be used only in conjunction
  with products based on FTDI parts. FTDI drivers may be distributed in any
  form as long as license information is not modified."
- **Name:** `ReleaseNotes.doc` keeps FTDI's name, which is not 8.3, by the
  owner's decision of 2026-10-20. No INF names it.
- **Modification:** none.

Provenance of `ftdi/w2k/`:

- **Vendor:** Future Technology Devices International Ltd. (FTDI).
- **Package:** FTDI's CDM driver for Windows 2000, version 2.06.00,
  WHQL certified, listed by FTDI under "No Longer Supported" as "Windows
  2000 2009-10-22 2.06.00 ... WHQL Certified".
- **Original download location:** FTDI's official URL
  `http://www.ftdichip.com/Drivers/CDM/Win2k/CDM%202.06.00%20WHQL%20Certified.zip`,
  linked from FTDI's VCP driver page, archived at
  <https://web.archive.org/web/20111020130746/http://www.ftdichip.com/Drivers/VCP.htm>.
  As of 2026-10-20 the URL returns HTTP 403 to the host that searched.
  Archived copy:
  <https://web.archive.org/web/20111019224829/http://www.ftdichip.com/Drivers/CDM/Win2k/CDM%202.06.00%20WHQL%20Certified.zip>.
- **Obtained:** 2026-10-20, from the archived copy above.
- **Archive:** `CDM 2.06.00 WHQL Certified.zip`, 897,812 bytes, SHA-256
  `a6920cac51bf1cf2df6649c789e9fcd604269ab1e73fa74d5f631d4493f847eb`. It
  holds the 23 files in a folder `CDM 2.06.00 WHQL Certified/`, with
  subfolders `i386/` and `amd64/`; they are copied without the top
  folder, the subfolders kept.
- **Licence:** no licence file in the archive. `ftdibus.inf` and
  `ftdiport.inf` carry "Copyright (c) 2000-2009 FTDI Ltd." and "The
  driver may be distributed in any form as long as our license information
  is not modified." `ftd2xx.h` carries "Copyright (c) 2001-2007 Future
  Technology Devices International Ltd." FTDI's VCP driver page, as
  archived on 2011-10-20 (above), reads: "FTDI drivers may be used only in
  conjunction with products based on FTDI parts. FTDI drivers may be
  distributed in any form as long as license information is not
  modified."
- **Name:** `CDM 2 06 00 Release Info.rtf` and
  `LogoVerificationReport.pdf` keep FTDI's names, which are not 8.3, by
  the owner's decision of 2026-10-20. No INF names them.
- **Modification:** none.

Provenance of `ch341/w98se-xp/`:

- **Vendor:** Nanjing Qinheng Microelectronics Co., Ltd. (WCH,
  "南京沁恒微电子股份有限公司").
- **Package:** `CH341SER.ZIP`, CH341SER version 3.7, uploaded
  2022-03-02, listed by WCH as 545KB and described as
  "CH340/CH341 USB转串口WINDOWS驱动程序，内含DLL动态库及非标准波特率的设置等使用说明，支持32/64位Windows 11/10/8.1/8/7/VISTA/XP，SERVER 2022/2019/2016/2012/2008/2003，2000/ME/98，通过微软数字签名认证，支持USB转UART/3线和9线SERIAL串口。"
  (CH340/CH341 USB-to-serial Windows driver, with a DLL and notes on
  non-standard baud rates; supports 32/64-bit Windows 11 to XP, Server
  2022 to 2003, and 2000/ME/98; signed by Microsoft). `CH341SER.INF`
  reads "Driver for CH340/CH341 (USB=>SERIAL chip) V3.7" and "WDM&VXD
  for Windows 98/Me/2000/XP/Vista/7/8/8.1/10/11/SERVER
  2003/2008/2012/2016/2019/2022".
- **Original download location:** WCH's download page
  `http://www.wch.cn/downloads/CH341SER_ZIP.html`, archived at
  <https://web.archive.org/web/20220407194124/http://www.wch.cn/downloads/CH341SER_ZIP.html>,
  whose download link is WCH's `http://www.wch.cn/downloads/file/5.html`
  with a per-visit `time` and `code` query. As of 2026-10-20 the live page
  is built by script and gave no download link to the host that searched.
  Archived copy, served by WCH with
  `Content-Disposition: attachment; filename="CH341SER.ZIP"`:
  <https://web.archive.org/web/20220606101141/http://www.wch.cn/downloads/file/5.html?time=2022-06-06+18%3A01%3A53&code=OY1yrm7HiwKmZRF9eCaTcVK9njKAsYXQbJXLFtQT>.
- **Obtained:** 2026-10-20, from the archived copy above.
- **Archive:** `CH341SER.ZIP`, 558,470 bytes, SHA-256
  `0b1da457085bdf981ca24de2ab72a24b6460b52375ac886abff0dbec79d360ec`. It
  holds the 24 files in a folder `CH341SER/`, with subfolders
  `DRVSETUP64/` and `WIN 1X/`; they are copied without the top folder,
  the subfolders kept.
- **Licence:** none found. The archive holds no licence or EULA file;
  `CH341SER.INF` carries "Copyright (C) W.ch 2001-2022". WCH's download
  page (the 2022-04-07 copy above) gives the description quoted above and
  no licence terms.
- **Name:** these keep WCH's names, which are not 8.3, by the owner's
  decision of 2026-10-20: `CH341PORTS.DLL` (which `CH341SER.INF` copies
  on every system), `CH341PORTSA64.DLL`, `CH341PTA64.DLL`, the folder
  `DRVSETUP64/` and its `DRVSETUP64.exe`, and the folder `WIN 1X/` (its
  name has a space) with its own `CH341PORTS.DLL`, `CH341PORTSA64.DLL` and
  `CH341PTA64.DLL`.
- **Modification:** none.

### `non-free/hid/`

| File | Whose | Version |
|---|---|---|
| All 8 files in `x360c/w98se-me/` | Masahiko Morii | `x360c.w98.x86.en.zip`, 2010-05-04 |
| All 6 files in `x360c/w2k/` | Masahiko Morii | `x360c.w2k.x86.en.zip`, 2010-05-04 |
| All 6 files in `x360c/wxp/` | Masahiko Morii | `x360c.wxp.x86.en.zip`, 2010-05-04 |
| All 7 files in `x360c/wxp64/` | Masahiko Morii | `x360c.wnet.x64.en.zip`, 2010-05-04 |
| All 7 files in `x360c/wvista/` | Masahiko Morii | `x360c.wlh.x86.en.zip`, 2010-05-04 |
| All 8 files in `x360c/wvista64/` | Masahiko Morii | `x360c.wlh.x64.en.zip`, 2010-05-04 |
| All 7 files in `x360c/w7/` | Masahiko Morii | `x360c.win7.x86.en.zip`, 2010-05-04 |
| All 8 files in `x360c/w7_64/` | Masahiko Morii | `x360c.win7.x64.en.zip`, 2010-05-04 |
| All 7 files in `x360wc/w2k/` | Masahiko Morii | `x360wc.w2k.x86.en.zip`, 2010-03-21 |
| All 6 files in `x360wc/wxp/` | Masahiko Morii | `x360wc.wxp.x86.en.zip`, 2010-03-21 |
| All 7 files in `x360wc/wxp64/` | Masahiko Morii | `x360wc.wnet.x64.en.zip`, 2010-03-21 |
| All 7 files in `x360wc/wvista/` | Masahiko Morii | `x360wc.wlh.x86.en.zip`, 2010-03-21 |
| All 8 files in `x360wc/wvista64/` | Masahiko Morii | `x360wc.wlh.x64.en.zip`, 2010-03-21 |
| All 7 files in `x360wc/w7/` | Masahiko Morii | `x360wc.win7.x86.en.zip`, 2010-03-21 |
| All 8 files in `x360wc/w7_64/` | Masahiko Morii | `x360wc.win7.x64.en.zip`, 2010-03-21 |

The dates are those of the folders Morii served each build from. Each
folder is one of his builds, unmodified. `SHA256.TXT` lists each file's
hash.

Provenance of `x360c/` and `x360wc/`:

- **Author:** Masahiko Morii, who published both drivers, with their
  source, on his own site at `http://www.katch.ne.jp/~morii/` (titled
  "Not digitally signed" by 2011). The pages and readmes call them
  unofficial ("非公式") and say to use them at one's own risk
  ("本ソフトウェアの使用は各自の責任で行ってください").
- **Packages:** Morii's final builds, the English (`.en`) zip for each
  system. His last x360c page, as archived on 2011-09-03
  (<https://web.archive.org/web/20110903042003/http://www.katch.ne.jp:80/%7Emorii/driver/x360c/index.html>),
  lists them under `files/20100504/` for Windows 7, Vista, XP, XP
  Professional x64, 2000, and Me / 98SE, each marked "開発終了"
  (development ended); his x360wc page, as archived on 2011-09-27
  (<https://web.archive.org/web/20110927232228/http://www.katch.ne.jp/~morii/driver/x360wc/index.html>),
  lists the receiver driver's under `files/20100321/` for Windows 7,
  Vista, XP, XP Professional x64 and 2000. The size of every zip used
  here agrees with the size his page gives for it, and every file in the
  zips is dated 2010-05-04 (x360c) or 2010-03-21 (x360wc).
- **Original download location:** Morii's own URLs,
  `http://www.katch.ne.jp/~morii/driver/x360c/files/20100504/<file>` and
  `http://www.katch.ne.jp/~morii/driver/x360wc/files/20100321/<file>`.
  The Internet Archive never captured a copy of them: every capture of
  those URLs is an HTTP 403 or 404 from Morii's server, and the site
  returned HTTP 404 on 2026-10-20. They were therefore taken from the
  mirror of his site that he sanctioned in writing:
  - **Morii's permission.** His home page, as archived on 2011-11-23
    (<https://web.archive.org/web/20111123183605/http://www.katch.ne.jp/~morii/index.html>),
    announcing the site's closure, reads:
    "諸事情により、2011年11月30日を以って、当サイトを閉鎖致します。デバイス ドライバなどが必要な方は適宜、ダウンロードをお願いします。なお、転載が必要でしたら、各自の責任で自由に行っていただいて構いません。"
    (For various reasons this site will close on 30 November 2011.
    Anyone who needs the device drivers or other files, please download
    them as needed. If you need to repost them, you are free to do so, on
    your own responsibility.)
  - **The mirror.** `https://lavendy.net/special/driver/`, put up on
    2011-12-01 by the operator of lavendy.net, whose post of that date
    (<https://web.archive.org/web/20120510074336/http://lavendy.net/psu/2011/12/xbox360_unofficial_driver.html>)
    says it holds Morii's site as taken in the early hours of the day it
    closed, that all rights stay with Morii, and that the pages are
    reproduced as they were, with only the access counter and Morii's
    mail address removed. Its index page carries Morii's closure notice
    and permission word for word. Archived pages:
    <https://web.archive.org/web/20120426090645/http://lavendy.net/special/driver/index.html>,
    <https://web.archive.org/web/20120426225851/http://lavendy.net:80/special/driver/x360c/index.html>
    and
    <https://web.archive.org/web/20120426225935/http://lavendy.net:80/special/driver/x360wc/index.html>.
- **Obtained:** 2026-10-20, from the live mirror. Each zip matches the
  SHA-1 the Internet Archive records for its captures of the mirror's
  URL (the earliest is given below; the captures run from 2015 to 2026,
  all with the same content).
- **Archives:** the files sit at each zip's root (with a folder `Omake/`
  in `x360c.w98.x86.en.zip` and `x360wc.w2k.x86.en.zip`) and are copied
  as they are. With the archived copy of each:
  - `x360c.w98.x86.en.zip`, 71,016 bytes, SHA-256
    `32c9ea96d43b5c94287402b258a7a977b8f60e68a9d24587d7ed13b122591657`:
    <https://web.archive.org/web/20160407092644/http://lavendy.net/special/driver/x360c/x360c.w98.x86.en.zip>
  - `x360c.w2k.x86.en.zip`, 88,992 bytes, SHA-256
    `deee17e328a9f314f9ddf056d5cb20c96b38b8a89a0e4febb7eece35fbe60334`:
    <https://web.archive.org/web/20250627163321/https://lavendy.net/special/driver/x360c/x360c.w2k.x86.en.zip>
  - `x360c.wxp.x86.en.zip`, 97,959 bytes, SHA-256
    `839a0603cb2c3844a6a07c5e38c2b911f165df15dd4a87b670ccac0e46b3d7ad`:
    <https://web.archive.org/web/20160323012400/http://lavendy.net/special/driver/x360c/x360c.wxp.x86.en.zip>
  - `x360c.wnet.x64.en.zip`, 112,919 bytes, SHA-256
    `022ff38ed4f091c68676736d6cdb56b0135bd7c63e1d6e4319979989a5b8082e`:
    <https://web.archive.org/web/20161204215459/http://lavendy.net/special/driver/x360c/x360c.wnet.x64.en.zip>
  - `x360c.wlh.x86.en.zip`, 320,959 bytes, SHA-256
    `9e2abbe18b0e74ea057434d74316c56aab0302534e4873dd881fed39a1ebd953`:
    <https://web.archive.org/web/20161204215416/http://lavendy.net/special/driver/x360c/x360c.wlh.x86.en.zip>
  - `x360c.wlh.x64.en.zip`, 335,636 bytes, SHA-256
    `8d46cd4534d7992ebda8e2c8897cc1e1edd70a3cb406813ad92bb32e92d0b806`:
    <https://web.archive.org/web/20160407090312/http://lavendy.net/special/driver/x360c/x360c.wlh.x64.en.zip>
  - `x360c.win7.x86.en.zip`, 320,894 bytes, SHA-256
    `5f682ac74f2f51b94b88b5c832bb9ed7bb06ae571ff198d4d8bda2b70095c6ad`:
    <https://web.archive.org/web/20161204215427/http://lavendy.net/special/driver/x360c/x360c.win7.x86.en.zip>
  - `x360c.win7.x64.en.zip`, 335,571 bytes, SHA-256
    `d8aa78ca91a77be948ea41241c36b50e3e6fd02f07de1f05bea62a77c099042b`:
    <https://web.archive.org/web/20160323012332/http://lavendy.net/special/driver/x360c/x360c.win7.x64.en.zip>
  - `x360wc.w2k.x86.en.zip`, 83,784 bytes, SHA-256
    `00bbf2feee7573c117b14364b1dd93480e1d56695259b2acf069d51d58fd2cf3`:
    <https://web.archive.org/web/20151030131800/http://lavendy.net/special/driver/x360wc/x360wc.w2k.x86.en.zip>
  - `x360wc.wxp.x86.en.zip`, 92,134 bytes, SHA-256
    `24efb94c1b96d4a1932acdb4229fd7f06a151edaf60979b6b7372bc09ed7aee1`:
    <https://web.archive.org/web/20151030132503/http://lavendy.net/special/driver/x360wc/x360wc.wxp.x86.en.zip>
  - `x360wc.wnet.x64.en.zip`, 107,194 bytes, SHA-256
    `255bf8b8269e485ba82a7866c9d738baeaf3a8c6c5c57b2a753f0df599c31050`:
    <https://web.archive.org/web/20151030132752/http://lavendy.net/special/driver/x360wc/x360wc.wnet.x64.en.zip>
  - `x360wc.wlh.x86.en.zip`, 314,631 bytes, SHA-256
    `b866d27d9ae2379bb73c285382ca017bbc1b39e838715196ab6a5d0246b20050`:
    <https://web.archive.org/web/20151030132120/http://lavendy.net/special/driver/x360wc/x360wc.wlh.x86.en.zip>
  - `x360wc.wlh.x64.en.zip`, 329,634 bytes, SHA-256
    `c3d4d863e46d1a3ee0cc10d78587b8a1d61eef1d7b081fd1b84e0492c0d61ccd`:
    <https://web.archive.org/web/20151030132846/http://lavendy.net/special/driver/x360wc/x360wc.wlh.x64.en.zip>
  - `x360wc.win7.x86.en.zip`, 314,581 bytes, SHA-256
    `b75d8da6f14bb9541f6781aeefb25f77ee238e7b0edb0209eb7baef9935af80d`:
    <https://web.archive.org/web/20151030132347/http://lavendy.net/special/driver/x360wc/x360wc.win7.x86.en.zip>
  - `x360wc.win7.x64.en.zip`, 329,569 bytes, SHA-256
    `87f1eb8cc84128bff914631183870570cef487d4b44e351a4c76791e832057cc`:
    <https://web.archive.org/web/20151030132615/http://lavendy.net/special/driver/x360wc/x360wc.win7.x64.en.zip>
- **Cross-checks** (2026-10-20; nothing shipped from them):
  - `x360c.w98.x86.en.zip`: the archive.org item
    `win98-xbox-360-controller-driver` (uploaded 2024-08-06), in its
    `Win98, 2000, XP Xbox 360 Controller Driver.zip`, holds a copy with
    the same SHA-256. Its "Newer Drivers" folder holds a repacked set
    whose `X360C.INF` differs; its `X360C.SYS`, `X360CCP.DLL`,
    `X360CFF.DLL` and `X360CSA.EXE` are byte-identical to Morii's.
  - MDGx's `X360C.EXE`, as archived on 2015-06-02
    (<https://web.archive.org/web/20150602065842/http://www.mdgx.com/files/X360C.EXE>,
    154,112 bytes, SHA-256
    `64c5354969932680f069f7ef8d39cb853b223b977620935f42d5061ae25899c3`),
    a self-extracting CAB of a 98 SE/ME repack: its `X360C.SYS`,
    `X360CCP.DLL`, `X360CFF.DLL` and `X360CSA.EXE` are byte-identical to
    those in `x360c.w98.x86.en.zip`; its `X360C.INF` is MDGx's own.
  - The Unofficial Windows 98 SE Service Pack 3 was not checked.
  - No copy of the 2000 to 7 builds, or of x360wc, was found outside the
    mirror.
- **Licence:** no licence file in the archives, and none on Morii's
  pages beyond the own-risk sentence above. His permission to repost is
  quoted above. His home page also says that freeware and personal
  non-commercial shareware may use his source code without restriction.
- **Name:** the long names listed in README.md keep Morii's names.
- **Modification:** none.

### `non-free/wifi/`

| File | Whose | Version |
|---|---|---|
| All 16 files in `rtl8187/w98se-vista/` | Realtek Semiconductor Corp. | 5.1313.0613.2008 (`Win98\Netrtuw.inf` `DriverVer` 06/13/2008. XP x64 5.1312.0416.2008. Vista 6.1313.0613.2008) |
| All 6 files in `rtl8187/w7/` | Realtek Semiconductor Corp. | 6.1316.1209.2009 |
| All 18 files in `rtl8187b/wxp-7/` | Realtek Semiconductor Corp. | XP 5.1162.0610.2009, XP x64 5.1160.0415.2009, Vista 6.1162.0610.2009, 7 62.1181.1105.2009 |
| All 20 files in `rtl8192cu/wxp-7/` | Realtek Semiconductor Corp. | 1021.3.0912.2012 (`RTLBt.inf` 1.0.0.0) |
| All 38 files in `rtwlanu/wxp-7/` | Realtek Semiconductor Corp. | 1030.25.0701.2017 (`DriverVer` 12/25/2017) |
| All 18 files in `rtwlanu17/wxp-7/` | Realtek Semiconductor Corp. | 1030.17.1101.2016 (`DriverVer` 04/06/2017) |
| All 21 files in `rtl8192su/w2k-7/` | Realtek Semiconductor Corp. | 1084.53.0809.2011 (2000 to Vista), 1086.48.0809.2011 (7) |
| All 19 files in `ar9271/wxp-7/` | Atheros Communications (now Qualcomm Atheros), as TP-LINK Technologies Co., Ltd. ships it for the TL-WN721N (the INFs name "TP-LINK" as provider) | 7.7.0.102 (XP), 8.0.0.84 (Vista), 2.0.0.62 (7) |
| All 25 files in `ar9170/w2k-7/` | Atheros Communications, as TP-LINK Technologies Co., Ltd. ships it for the TL-WN821N and TL-WN822N (the INFs for 7 carry TP-LINK's copyright). `Setup.exe` and `QSS.exe`: TP-LINK, built with Macrovision's InstallShield 14 (their version resources), as TP-LINK ships them. The two user guides: TP-LINK | 3.0.0.165 (2000, XP), 3.1.0.131 (Vista), 3.5.0.12 (7) |
| All 9 files in `ae2500/wxp/`, all 15 in each of `wvista/`, `w7/` | Broadcom Corporation, as Cisco-Linksys ships it for the AE1200 and AE2500 (`WdfCoInstaller01005.dll` and `WdfCoInstaller0100564.dll`, 1.5.6000.0, and `WdfCoInstaller01009.dll` and `WdfCoInstaller0100964.dll`, 1.9.7600.16385: Microsoft Corporation, as Linksys ships them) | 5.100.68.46, 5.100.243.6, 5.100.68.46 |

The Realtek folders hold only the per-system driver folders, taken from
Realtek's packages by this project and otherwise unchanged (below).
`ar9271/wxp-7/` is TP-LINK's package without its Windows 8 and 8.1
folders. The others are their packages as released, unmodified.
`SHA256.TXT` lists each file's hash. None of these drivers has been tested
by this project.

Provenance of `rtl8187/` (`w98se-vista/`, `w7/`):

- **Vendor:** Realtek Semiconductor Corp.
- **Packages:** Realtek's RTL8187L "Auto Installation Program" packages:
  `8187_1313.0613_UI_1.00.0023` for 98 SE to Vista (`w98se-vista/`) and
  `RTL8187L_WindowsDriver_Win7_6.1316.1209.2009_UI_1.00.0145.L` for 7
  (`w7/`). Both are linked from Realtek's old RTL8187L download list
  (`realtek.com.tw/downloads/RedirectFTPSite.aspx`, entry `DownID=437`,
  archived 2015).
- **Original download location:** Realtek's own file server,
  `https://www.realtek.com/rtdrivers/cn/wlan/`. Archived copies, the ones
  used:
  - <https://web.archive.org/web/20240219095753/https://www.realtek.com/rtdrivers/cn/wlan/0001-8187_1313.0613_UI_1.00.0023.zip>
  - <https://web.archive.org/web/20240219102145/https://www.realtek.com/rtdrivers/cn/wlan/0001-RTL8187L_Win7_6.1316.1209.2009.L.zip>
- **Obtained:** 2026-10-27, from the archived copies above.
- **Archives:**
  - `0001-8187_1313.0613_UI_1.00.0023.zip`, 10,459,616 bytes, SHA-256
    `761c9f420c0f2636b429ddbc1905f45f38727cdfbca6b84f5cb39139c74d7898`
  - `0001-RTL8187L_Win7_6.1316.1209.2009.L.zip`, 18,383,978 bytes,
    SHA-256
    `063c2a3193b454b8a43e80a55122aa758aeba287a99b0a33d62d5812b161a9f3`
- **Licence:** none found. Neither zip holds a licence or EULA file. The
  INFs carry "Copyright (C) 2008 Realtek Semiconductor Corp." (2009 for
  7).
- **Name:** these keep Realtek's names: `Netrtuw_x64.inf` and the
  folders `VistaX86/`, `VistaX64/`, `WinXP2K/`, `Win7X86/` and
  `Win7X64/` are not 8.3.
- **Modification:** the folders were taken from the packages by this
  project and are otherwise unchanged (owner, 2026-10-27). Only the
  per-system folders of each package's `RTL8187\` folder are carried:
  `Win98`, `WinME`, `WinXP2K`, `WinX64`, `VistaX86` and `VistaX64` (from
  `87-USB\RTL8187\`), and `Win7X86` and `Win7X64`. Left out: the rest of
  each package, that is Realtek's InstallShield setup and its files, the
  install batch files (7 package), `DATA\`, `EAP\` (7 package) and the
  release notes.

Provenance of `rtl8187b/wxp-7/`:

- **Vendor:** Realtek Semiconductor Corp.
- **Package:** `RTL8187B_Drv_XP_5.1162.0610.2009_Win7_62.1181.1105.2009_UI_1.00.0145.ALL.L`,
  Realtek's RTL8187B "Auto Install Program" (Realtek's download list
  entry `DownID=880`).
- **Original download location:** Realtek's own file server. Archived
  copy, the one used:
  <https://web.archive.org/web/20240219101632/https://www.realtek.com/rtdrivers/cn/wlan/0001-RTL8187B_Auto_Install_Program.zip>.
- **Obtained:** 2026-10-27, from the archived copy above.
- **Archive:** `0001-RTL8187B_Auto_Install_Program.zip`, 17,212,818
  bytes, SHA-256
  `aa503063bfad2e6987161388b0736bcf0f3e00ac6fc7b72a8451bf0fdd55b82a`.
- **Licence:** none found. The INFs carry "Copyright (C) 2008 Realtek
  Semiconductor Corp." (2009 for 7).
- **Modification:** the folders were taken from the package by this
  project and are otherwise unchanged (owner, 2026-10-27). Only the six
  per-system folders of its `RTL8187B\` folder are carried (`WinXP`,
  `WinX64`, `VistaX86`, `VistaX64`, `Win7X86`, `Win7X64`). Left out: the
  rest of the package, that is the InstallShield setup and its files, the
  install batch files, `DATA\`, `EAP\` and the release notes.

Provenance of `rtl8192cu/wxp-7/`:

- **Vendor:** Realtek Semiconductor Corp.
- **Package:** `(BV5)RTLWlanU_1021.3.0912.2012_UI_1.00.0199.SupportALL.L`,
  Realtek's RTL8188CU/RTL8192CU "Auto Install Package", 1021.3.0912.2012,
  for XP to 8.
- **Original download location:** Realtek's own file server. Archived
  copy, the one used:
  <https://web.archive.org/web/20240219104028/https://www.realtek.com/rtdrivers/cn/wlan/0001-RTL819xCU_AutoInstallPackage.zip>.
- **Obtained:** 2026-10-27, from the archived copy above.
- **Archive:** `0001-RTL819xCU_AutoInstallPackage.zip`, 35,282,265 bytes,
  SHA-256
  `ad686d0e08c390f074e989950b70b4b94c03a5114c79f3cf265a912b20f4f1ef`.
- **Licence:** none found. The INFs carry "Copyright (C) 2012 Realtek
  Semiconductor Corp."
- **Modification:** the folders were taken from the package by this
  project and are otherwise unchanged (owner, 2026-10-27). Only six
  per-system folders of its `RTWLANU_Driver\` folder are carried
  (`WinXP`, `WinX64`, `VistaX86`, `VistaX64`, `Win7X86`, `Win7X64`).
  Left out: the rest of the package, that is the InstallShield setup and
  its files, the install batch files, `DATA\`, `EAP\`, the `IM\`
  intermediate driver, the release notes and the `Win8X86` and `Win8X64`
  folders (Windows 8 is outside this pack).

Provenance of `rtwlanu/wxp-7/`:

- **Vendor:** Realtek Semiconductor Corp.
- **Package:** `RTLWlanU_WindowsDriver_1030.25.0701.2017_DUA_Drv_3.00.0019.L`,
  listed on Realtek's RTL8192EU, RTL8811AU, RTL8811CU, RTL8812AU,
  RTL8812BU and RTL8814AU pages (archived 2023) as "32bit/64bit Windows7,
  Windows8.1, Windows10 WLAN USB driver (Install Package)
  1030.25.0701.2017, 2018/09/07". The package itself holds XP and Vista
  builds too, and its release note reads "support WinXP ~ Win10 OS". This
  pack offers it on XP and Vista as well as 7 (owner, 2026-10-27).
- **Original download location:** Realtek's own file server. Realtek's
  pages link it through an `agree-to-download` page (archived 2020, an
  e-mail field and an audio-driver note, no terms for this file).
  Archived copy, the one used:
  <https://web.archive.org/web/20240218131614/https://www.realtek.com/rtdrivers/cn/wlan/0002-Realtek_WindowsDriver_1030.25.0701.2017.zip>.
- **Obtained:** 2026-10-27, from the archived copy above.
- **Archive:** `0002-Realtek_WindowsDriver_1030.25.0701.2017.zip`,
  52,899,174 bytes, SHA-256
  `dac755a0cecbdbe2818313f2049dfb140c98667ca08fe71b0478759c85d46c3a`.
- **Licence:** none found. The INFs carry "Copyright (C) 2012 Realtek
  Semiconductor Corp."
- **Modification:** the folders were taken from the package by this
  project and are otherwise unchanged (owner, 2026-10-27). Only six
  per-system folders of its `RTWLANU_Driver\` folder are carried
  (`WinXP`, `WinX64`, `VistaX86`, `VistaX64`, `Win7X86`, `Win7X64`).
  Left out: `Setup.exe` and the InstallShield files with it,
  `Install.bat`, `UnInstall.bat`, `Autorun.inf`, `EAP\`, `IHV\`, the
  release notes and the Windows 8, 8.1 and 10 folders.

Provenance of `rtwlanu17/wxp-7/`:

- **Vendor:** Realtek Semiconductor Corp.
- **Package:** `Realtek_USB_Windows_WHQL_Driver_1030.17.1101.2016`, a
  drivers-only package for XP to 10 (Realtek's download list entry
  `DownID=1120&PFid=64`, archived 2019).
- **Original download location:** Realtek's own file server. Archived
  copy, the one used:
  <https://web.archive.org/web/20240218044047/https://www.realtek.com/rtdrivers/cn/wlan/0001-Realtek_USB_Windows_Driver_1030.17.1101.2016.zip>.
- **Obtained:** 2026-10-27, from the archived copy above.
- **Archive:** `0001-Realtek_USB_Windows_Driver_1030.17.1101.2016.zip`,
  25,710,952 bytes, SHA-256
  `a3ce0028313a8ca9058969170cc66966cc0488766a7ea7c4f66bf536885af45a`.
- **Licence:** none found. The INFs carry "Copyright (C) 2012 Realtek
  Semiconductor Corp."
- **Modification:** the folders were taken from the package by this
  project and are otherwise unchanged (owner, 2026-10-27). Its six XP to
  7 folders are carried (`WinXP`, `WinX64`, `VistaX86`, `VistaX64`,
  `Win7X86`, `Win7X64`). Left out: the Windows 8, 8.1 and 10 folders.

Provenance of `rtl8192su/w2k-7/`:

- **Vendor:** Realtek Semiconductor Corp.
- **Package:** `RTL8188_8191_8192_SU_WindowsDriver_1086.48.0809.2011.F0049_12.P0406_UI_1.00.0187.L`,
  Realtek's RTL8188SU/RTL8191SU/RTL8192SU "Auto Install Package"
  (Realtek's download list entry `DownID=858`).
- **Original download location:** Realtek's own file server. Archived
  copy, the one used:
  <https://web.archive.org/web/20240219103357/https://www.realtek.com/rtdrivers/cn/wlan/0001-RTL8192SU_AutoInstallPackage.zip>.
- **Obtained:** 2026-10-27, from the archived copy above.
- **Archive:** `0001-RTL8192SU_AutoInstallPackage.zip`, 29,820,529 bytes,
  SHA-256
  `535ffcf7822c827d2bdaa1358ba57b7a1b7cc6245839054407b334fcebdad331`.
- **Licence:** none found. The INFs carry "Copyright (C) 2008 Realtek
  Semiconductor Corp."
- **Modification:** the folders were taken from the package by this
  project and are otherwise unchanged (owner, 2026-10-27). Only the seven
  per-system folders of its `88_91_92_SU_Driver\` folder are carried
  (`Win2K`, `WinXP`, `WinX64`, `VistaX86`, `VistaX64`, `Win7X86`,
  `Win7X64`). Left out: the rest of the package, that is the
  InstallShield setup and its files, the install batch files, `DATA\`,
  `EAP\` and the release notes.

Provenance of `ar9271/wxp-7/`:

- **Vendor:** Atheros Communications (now Qualcomm Atheros), shipped by
  TP-LINK Technologies Co., Ltd. The INFs name "TP-LINK" as provider.
- **Package:** TP-LINK's TL-WN721N v1 driver, `TL-WN721N_V1_140915`,
  listed on TP-LINK's page with "Published Date: 2014-09-15" and
  "Vista/XP/7/8/8.1". TP-LINK's utility for the same adapter is a
  separate download and is not carried (owner, 2026-10-27).
- **Original download location:** TP-LINK's official URL, live on
  2026-10-27:
  `https://static.tp-link.com/resources/software/TL-WN721N_V1_140915.zip`,
  from <https://www.tp-link.com/us/support/download/tl-wn721n/v1/>.
- **Obtained:** 2026-10-27, from TP-LINK's URL above.
- **Archive:** `TL-WN721N_V1_140915.zip`, 7,368,965 bytes, SHA-256
  `5217cb84427bee80754e9ab6718acde854bd1eb0507580dd19d00803f27f345d`. It
  holds its files in a folder `TL-WN721N_V1_140915/`. They are copied
  without that folder.
- **Licence:** none found. The XP to 7 INFs carry no copyright line. The
  Windows 8 and 8.1 INFs (not carried) carry "Copyright 2009 Atheros
  Communications Inc., all rights reserved." and "Copyright (c) 2011
  Qualcomm Atheros, Inc.".
- **Name:** these keep TP-LINK's names: the folders (`Windows XP 32bit/`
  and the others) and `Release Note.txt` hold spaces.
- **Modification:** the `Windows 8 32bit`, `Windows 8 64bit`, `Windows
  8.1 32bit` and `Windows 8.1 64bit` folders are left out (Windows 8 is
  outside this pack). The rest is as released.

Provenance of `ar9170/w2k-7/`:

- **Vendor:** Atheros Communications, shipped by TP-LINK Technologies
  Co., Ltd. The INFs name "TP-LINK" as provider.
- **Package:** TP-LINK's driver for the TL-WN821N v2 and TL-WN822N v1,
  listed on TP-LINK's TL-WN822N v1 page as "TL-WN822N_100629",
  "Published Date: 2010-06-29", "Windows 2000/XP/Vista/7",
  "WHQL-Certified".
- **Original download location:** TP-LINK's official URL, live on
  2026-10-27:
  `https://static.tp-link.com/resources/software/TL-WN821N_WN822N_100629.zip`,
  from <https://www.tp-link.com/us/support/download/tl-wn822n/v1/>.
- **Obtained:** 2026-10-27, from TP-LINK's URL above.
- **Archive:** `TL-WN821N_WN822N_100629.zip`, 30,190,672 bytes, SHA-256
  `3d4d5d7d49f61e5b4e17e0ea4d5d415770599d7b238f31eb019c1a7b5aaa7d44`. It
  holds its files in a folder `TL-WN821N_WN822N/`. They are copied without
  that folder.
- **Licence:** none found. The INFs for 7 carry "Copyright (c) 2009,
  TP-LINK TECHNOLOGIES CO., LTD.All Rights Reserved." The others carry
  no copyright line.
- **Name:** these keep TP-LINK's names: `Driver Files/`, its folders and
  the user guides hold spaces.
- **Modification:** none. `Setup.exe` and `QSS.exe` are TP-LINK's setup
  and its QSS (Quick Secure Setup) program. They are copied, never
  run.

Provenance of `ae2500/` (`wxp/`, `wvista/`, `w7/`):

- **Vendor:** Broadcom Corporation, shipped by Cisco-Linksys (the INFs:
  "Cisco Consumer Products LLC"). The KMDF co-installers: Microsoft
  Corporation, shipped by Linksys in the Vista and 7 packages.
- **Packages:** Linksys's AE2500 drivers for XP (5.100.68.46,
  2011-03-28), Vista (5.100.243.6, 2011-03-30) and 7 (5.100.68.46),
  marked WHQL. Their INFs serve the Linksys AE1200 too.
- **Original download location:** Linksys's official URLs under
  `downloads.linksys.com/downloads/driver/`. Archived copies, the ones
  used:
  - <https://web.archive.org/web/20210922091040/https://downloads.linksys.com/downloads/driver/AE2500_xpdriver_5.100.68.46_WHQL,0.zip>
  - <https://web.archive.org/web/20210922091037/https://downloads.linksys.com/downloads/driver/AE2500_vistadriver_5.100.243.6_WHQL,0.zip>
  - <https://web.archive.org/web/20150809163702/http://downloads.linksys.com/downloads/driver/AE2500Win7_WHQL.zip>
- **Obtained:** 2026-10-27, from the archived copies above.
- **Archives:** each zip holds its files in one folder (`xp/`, `vista/`,
  `win7/`), copied without it.
  - `AE2500_xpdriver_5.100.68.46_WHQL,0.zip`, 3,117,121 bytes, SHA-256
    `ee9bdf47246e37bc2d1150e0504bd18dcedfbf0a2b8c67c561a25fdcff592250`
  - `AE2500_vistadriver_5.100.243.6_WHQL,0.zip`, 10,695,279 bytes,
    SHA-256
    `217b3287fdc27fe2e652b9538329edc1f0db42b516749382eb109bfdfc0d2463`
  - `AE2500Win7_WHQL.zip`, 10,580,152 bytes, SHA-256
    `fbcba9646b1eb2c9f0fa0135c12d5e3748c7a7152f3c32fed5228880de7ab3e2`
- **Licence:** none found. The INFs carry "Copyright 1998-2011, Broadcom
  Corporation." and "(c) 2011 Cisco and/or its affiliates. All rights
  reserved."
- **Name:** these keep Linksys's names: `bcmwlhigh5.inf`,
  `bcmwlhigh6.inf`, the `.sys`, `.cat` and `.dll` files with long names
  are not 8.3.
- **Modification:** none.

## Every file under `non-free/`

The owner of this repository claims no rights in these files and grants no
licence to them. Apart from the vendors' and authors' own statements
quoted above, no licence permitting their redistribution has been found
for any of them.

If you hold rights in any of these files and want them removed, open an issue
on this repository and they will be taken down.

## This repository's own files

`README.md`, `NOTICE.md`, `nusb33/NOTICE.md`, `SHA256.TXT` and
`.gitattributes` are the repository owner's, released under CC0 1.0
(public domain dedication,
<https://creativecommons.org/publicdomain/zero/1.0/>). That covers those
files only: nothing under `non-free/`, and none of the files in
`nusb33/w98se/`.
