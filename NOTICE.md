# Notice

## The driver files are not this repository's to license

Every file under `non-free/` belongs to its authors, not to the owner of this
repository, and so does every file in `nusb33/w98se/` (below). Each
folder under `non-free/` has its table below, and each package its
provenance record (README.md, "Where each package comes from"); a package
added later adds both. Searches recorded below were made on 2026-10-20.

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

They are ASIX's driver packages as released, unmodified. `SHA256.TXT`
lists each file's hash.

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
