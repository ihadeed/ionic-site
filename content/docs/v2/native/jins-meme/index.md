---
layout: "v2_fluid/docs_base"
version: "3.4.2"
versionHref: "/docs/v2/native"
path: ""
category: native
id: "jins-meme"
title: "Jins Meme"
header_sub_title: "Class in module "
doc: "Jins Meme"
docType: "class"
---

<h1 class="api-title">Jins Meme</h1>

<a class="improve-v2-docs" href="http://github.com/driftyco/ionic-native/edit/master/src/@ionic-native/plugins/jins-meme/index.ts#L4">
  Improve this doc
</a>






<pre><code class="nohighlight">$ ionic plugin add JinsMemeSDK-Plugin-Cordova
$ npm install --save @ionic-native/jins-meme
</code></pre>
<p>Repo:
  <a href="https://github.com/jins-meme/JinsMemeSDK-Plugin-Cordova">
    https://github.com/jins-meme/JinsMemeSDK-Plugin-Cordova
  </a>
</p>


<p>Implementation of the JINS MEME SDK</p>




<h2>Supported platforms</h2>
<ul>
  <li>Android</li><li>iOS</li>
</ul>






<h2>Usage</h2>
<pre><code>import { JinsMeme } from &#39;@ionic-native/jins-meme&#39;;

constructor(private jinsMeme: JinsMeme) { }

...

this.jinsMeme.setAppClientID(appClientId: string, clientSecret: string)
  .then(this.jinsMeme.startScan())
  .catch(console.log(&#39;jinsMeme.setAppClientID authentication error!&#39;));
</code></pre>








<h2>Instance Members</h2>
<h3><a class="anchor" name="setAppClientID" href="#setAppClientID"></a><code>setAppClientID(setAppClientID,&nbsp;clientSecret)</code></h3>


Authentication and authorization of App and SDK.
Must call this method at first.

<table class="table param-table" style="margin:0;">
  <thead>
  <tr>
    <th>Param</th>
    <th>Type</th>
    <th>Details</th>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td>
      setAppClientID</td>
    <td>
      <code>string</code>
    </td>
    <td>
      </td>
  </tr>
  
  <tr>
    <td>
      clientSecret</td>
    <td>
      <code>string</code>
    </td>
    <td>
      </td>
  </tr>
  </tbody>
</table>

<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="startScan" href="#startScan"></a><code>startScan()</code></h3>




Starts scanning for JINS MEME.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> 
</div><h3><a class="anchor" name="stopScan" href="#stopScan"></a><code>stopScan()</code></h3>


Stops scanning JINS MEME.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="connect" href="#connect"></a><code>connect(target)</code></h3>




Establishes connection to JINS MEME.
<table class="table param-table" style="margin:0;">
  <thead>
  <tr>
    <th>Param</th>
    <th>Type</th>
    <th>Details</th>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td>
      target</td>
    <td>
      <code>string</code>
    </td>
    <td>
      </td>
  </tr>
  </tbody>
</table>

<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> 
</div><h3><a class="anchor" name="setAutoConnect" href="#setAutoConnect"></a><code>setAutoConnect(flag)</code></h3>


Set auto connection mode.
<table class="table param-table" style="margin:0;">
  <thead>
  <tr>
    <th>Param</th>
    <th>Type</th>
    <th>Details</th>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td>
      flag</td>
    <td>
      <code>Boolean</code>
    </td>
    <td>
      </td>
  </tr>
  </tbody>
</table>

<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="isConnected" href="#isConnected"></a><code>isConnected()</code></h3>


Returns whether a connection to JINS MEME has been established.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="disconnect" href="#disconnect"></a><code>disconnect()</code></h3>


Disconnects from JINS MEME.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="startDataReport" href="#startDataReport"></a><code>startDataReport()</code></h3>




Starts receiving realtime data.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> 
</div><h3><a class="anchor" name="stopDataReport" href="#stopDataReport"></a><code>stopDataReport()</code></h3>


Stops receiving data.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="getSDKVersion" href="#getSDKVersion"></a><code>getSDKVersion()</code></h3>


Returns SDK version.



<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="getConnectedByOthers" href="#getConnectedByOthers"></a><code>getConnectedByOthers()</code></h3>


Returns JINS MEME connected with other apps.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="isCalibrated" href="#isCalibrated"></a><code>isCalibrated()</code></h3>


Returns calibration status


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="getConnectedDeviceType" href="#getConnectedDeviceType"></a><code>getConnectedDeviceType()</code></h3>


Returns device type.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="getConnectedDeviceSubType" href="#getConnectedDeviceSubType"></a><code>getConnectedDeviceSubType()</code></h3>


Returns hardware version.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="getFWVersion" href="#getFWVersion"></a><code>getFWVersion()</code></h3>


Returns FW Version.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="getHWVersion" href="#getHWVersion"></a><code>getHWVersion()</code></h3>


Returns HW Version.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="isDataReceiving" href="#isDataReceiving"></a><code>isDataReceiving()</code></h3>


Returns response about whether data was received or not.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div>





