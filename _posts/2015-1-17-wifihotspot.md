---
layout: post
title: Use command line in windows 8/8.1 to create a wifi hotspot.
---

<div dir="ltr" style="text-align: left;" trbidi="on">
Hey Guys.<br />
<br />
This post is dedicated to the girls in my hostel who asked me how to go about it. So while I was staying at the hostel I found this simple hack very useful to connect all my devices to the Internet, by creating a hotspot on my laptop. This article will save you from installing connectify and other unnecessary software on your PC.<br />
<br />
Steps to be followed:<br />
<ol style="text-align: left;">
<li>Click windows button. Type cmd. Command Prompt will open up as a search result. Right Click on Command Prompt and select Run as administrator option.</li>
<li>&nbsp;A dialog box asking permission to make changes to the computer appears. Click Yes.</li>
<li>To check if your computer supports hotspot feature or not type :</li>
<ul>
<li><b>netsh wlan show drivers&nbsp;</b> </li>
</ul>
<li><b>&nbsp;</b>If you see <b>Hosted Network Supported : Yes </b>then your PC supports&nbsp;&nbsp;&nbsp;&nbsp; hotspot and you can continue. </li>
<li>Now type&nbsp;</li>
<ul>
<li><b>netsh wlan set hostednetwork mode=allow ssid=wifiname key=typepasswordhere&nbsp;</b></li>
<li><b>&nbsp;</b>ssid is the name of your hotspot and key is the password for your hotspot </li>
</ul>
<li>Click Enter.</li>
<li>&nbsp;If you will get a message saying "<i> The hosted network mode has been set to allow. The SSID of the&nbsp; hosted network has been successfully changed. The user key passphrase of the hosted network has been successfully changed", </i>you are good to go.</li>
<li>To turn on the hotspot anytime later, all you have to do is enter</li>
<ul>
<li><b>netsh wlan start hostednetwork</b></li>
<li>you will get a message saying "The Hosted network started" </li>
</ul>
</ol>
<div style="text-align: center;">
</div>
<div style="text-align: center;">
</div>
<div style="text-align: left;">
Thats how easy it is!<b>&nbsp;</b><b> </b></div>
<div style="text-align: justify;">
<br /></div>
<br />
<div>
<br />
<br />
<br />
<br /></div>
</div>

