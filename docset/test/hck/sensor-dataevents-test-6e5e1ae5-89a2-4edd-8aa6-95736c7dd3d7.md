---
author: joshbax-msft
title: Sensor DataEvents Test
description: Sensor DataEvents Test
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 5911d2e6-3718-4d2f-8166-4c5c9b422e06
---

# Sensor DataEvents Test


If a client sets the change sensitivity to 0, data events will fire at the rate of the current report interval to within 20%, both for short (&lt; 1 sec) and long (&gt; 1 minute) values of the current report interval.

Data events should not be fired if the current report interval and change sensitivity (when applicable) are not met.

Sensors should not delay data reports more than 100% of the current report interval.

Data events should not be fired at a rate less than the minimum report interval.

## Test details


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Associated requirements</strong></p></td>
<td><p>Device.Input.Sensor.ALS.Discretional Device.Input.Sensor.Base.Discretional</p>
<p>[See the device hardware requirements.](http://go.microsoft.com/fwlink/p/?linkid=254483)</p></td>
</tr>
<tr class="even">
<td><p><strong>Platforms</strong></p></td>
<td><p>Windows 8.1 x64 Windows 8.1 x86</p></td>
</tr>
<tr class="odd">
<td><p><strong>Expected run time</strong></p></td>
<td><p>~2 minutes</p></td>
</tr>
<tr class="even">
<td><p><strong>Categories</strong></p></td>
<td><p>Basic</p></td>
</tr>
<tr class="odd">
<td><p><strong>Type</strong></p></td>
<td><p>Automated</p></td>
</tr>
</tbody>
</table>

 

## Running the test


Before you run the test, complete the test setup as described in the test requirements: [Sensor Device Testing Prerequisites](sensor-device-testing-prerequisites.md).

If this test is being run against a GPS sensor device node, make sure that you are running the test in an environment in which you can receive a GPS signal.

## Troubleshooting


For troubleshooting information, see [Troubleshooting Device.Input Testing](troubleshooting-deviceinput-testing.md).

Ensure that the location permissions are enabled.

Ensure that the GPS sensor has a signal.

 

 





