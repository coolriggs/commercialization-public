---
author: joshbax-msft
title: DMR playback performance (PERF-01 PERF-05)
description: DMR playback performance (PERF-01 PERF-05)
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 4abe6871-73f9-4b24-8593-ba78d9eea2e1
---

# DMR playback performance (PERF-01 PERF-05)


This test verifies that the DMR complies with performance specifications (PERF-01) and displays a visual indicator during delays longer than 3 seconds (PERF-05), as specified below.

**PERF-01** (Applies to A/V DMR and Audio DMR)

A DMR device must comply with the performance specifications indicated in the “Table PERF: Expected performance values for DMR devices” in the Device.Media.DMR.Base.PlaybackPerformance requirement. The test content for this requirement has the following characteristics:

-   A/V: AVC and AAC using an MP4 file. The video resolution is 1280 x 720 at 30 fps. Maximum system bitrate of 5 Mbps

-   Audio: LPCM content, Maximum bitrate of 1.5 Mbps

-   Image: 1920x1080, Maximum size of 500 KB

All tests require ideal network conditions.

**PERF-05** (Applies to A/V DMR and Audio DMR)

A DMR that needs more than 3 seconds to play audio, A/V, or images for any of the cases described in Table PERF must display a visual indicator to indicate that data is being processed and that it will start playing content soon.

## Test details


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Associated requirements</strong></p></td>
<td><p>Device.Media.DMR.Base.PlaybackPerformance</p>
<p>[See the device hardware requirements.](http://go.microsoft.com/fwlink/p/?linkid=254483)</p></td>
</tr>
<tr class="even">
<td><p><strong>Platforms</strong></p></td>
<td><p>Windows 7 (x64) Windows 7 (x86) Windows 8 (x64) Windows 8 (x86) Windows 8.1 x64 Windows 8.1 x86</p></td>
</tr>
<tr class="odd">
<td><p><strong>Expected run time</strong></p></td>
<td><p>~5 minutes</p></td>
</tr>
<tr class="even">
<td><p><strong>Categories</strong></p></td>
<td><p>Certification</p></td>
</tr>
<tr class="odd">
<td><p><strong>Type</strong></p></td>
<td><p>Manual</p></td>
</tr>
</tbody>
</table>

 

## Running the test


Before you run the test, complete the test setup as described in the test requirements: [Digital Media Renderer Testing Prerequisites](digital-media-renderer-testing-prerequisites.md).

A dialog box will appears that says **PlayTo a media to the DMR**. From the Windows client, right click on media file from File Explorer or Windows Media Player, and then click **PlayTo** to the DMR.

After the media starts rendering in the DMR, click **OK** in the dialog box.

## Troubleshooting


For troubleshooting information, see [Troubleshooting Device.Media Testing](troubleshooting-devicemedia-testing.md).

## More information


### Parameters

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parameter</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>WDKData_DeviceUUID</p></td>
<td><p>The Device ID</p></td>
</tr>
</tbody>
</table>

 

### Command syntax

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Command option</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>NetMediaLogoTests.exe NETMEDIA_0132 /dmrID=[Query WDKData_DeviceUUID]</strong></p></td>
<td><p>Runs the test.</p></td>
</tr>
</tbody>
</table>

 

### File list

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>File</th>
<th>Location</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>NetMediaLogoTests.exe</p></td>
<td><p><em>&lt;testbinroot&gt;</em>\nttest\multimediatest\sharing\netmedialogotests</p></td>
</tr>
</tbody>
</table>

 

 

 





