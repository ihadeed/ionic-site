---
layout: "v2_fluid/docs_base"
version: "3.4.2"
versionHref: "/docs/v2/native"
path: ""
category: native
id: "zbar"
title: "ZBar"
header_sub_title: "Class in module "
doc: "ZBar"
docType: "class"
---

<h1 class="api-title">ZBar</h1>

<a class="improve-v2-docs" href="http://github.com/driftyco/ionic-native/edit/master/src/@ionic-native/plugins/zbar/index.ts#L35">
  Improve this doc
</a>






<pre><code class="nohighlight">$ ionic plugin add cordova-plugin-cszbar
$ npm install --save @ionic-native/zbar
</code></pre>
<p>Repo:
  <a href="https://github.com/tjwoon/csZBar">
    https://github.com/tjwoon/csZBar
  </a>
</p>


<p>The ZBar Scanner Plugin allows you to scan 2d barcodes.</p>
<p>Requires Cordova plugin: <code>cordova-plugin-cszbar</code>. For more info, please see the <a href="https://github.com/tjwoon/csZBar">zBar plugin docs</a>.</p>




<h2>Supported platforms</h2>
<ul>
  <li>Android</li><li>iOS</li>
</ul>






<h2>Usage</h2>
<pre><code>import { ZBar, ZBarOptions } from &#39;@ionic-native/z-bar&#39;;

constructor(private zbar: ZBar) { }

...

let ZBarOptions = {
      flash: &quot;off&quot;,
      drawSight: false
    };

this.zbar.scan(zBarOptions)
   .then(result =&gt; {
      console.log(result); // Scanned code
   })
   .catch(error =&gt; {
      console.log(error); // Error message
   });
</code></pre>








<h2>Instance Members</h2>
<h3><a class="anchor" name="scan" href="#scan"></a><code>scan(options)</code></h3>


Open the scanner
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
      options</td>
    <td>
      <code>ZBarOptions</code>
    </td>
    <td>
      <p>Scan options</p>
</td>
  </tr>
  </tbody>
</table>

<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> Returns a Promise that resolves with the scanned string, or rejects with an error.
</div>





<h2><a class="anchor" name="ZBarOptions" href="#ZBarOptions"></a>ZBarOptions</h2>

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
      text_title
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>A string representing the title text (Android only).
Default: &quot;Scan QR Code&quot;</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      text_instructions
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>A string representing the instruction text (Android only).
Default: &quot;Please point your camera at the QR code.&quot;</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      camera
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>A string defining the active camera when opening the scanner.
Possible values: &quot;front&quot;, &quot;back&quot;
Default: &quot;back&quot;</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      flash
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>A string defining the state of the flash.
Possible values: &quot;on&quot;, &quot;off&quot;, &quot;auto&quot;
Default: &quot;auto&quot;</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      drawSight
    </td>
    <td>
      <code>boolean</code>
    </td>
    <td>
      <p>A boolean to show or hide a line in the center of the scanner.
Default: true</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  </tbody>
</table>





