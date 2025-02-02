---
layout: "v2_fluid/docs_base"
version: "3.4.2"
versionHref: "/docs/v2/native"
path: ""
category: native
id: "toast"
title: "Toast"
header_sub_title: "Class in module "
doc: "Toast"
docType: "class"
---

<h1 class="api-title">Toast</h1>

<a class="improve-v2-docs" href="http://github.com/driftyco/ionic-native/edit/master/src/@ionic-native/plugins/toast/index.ts#L36">
  Improve this doc
</a>






<pre><code class="nohighlight">$ ionic plugin add cordova-plugin-x-toast
$ npm install --save @ionic-native/toast
</code></pre>
<p>Repo:
  <a href="https://github.com/EddyVerbruggen/Toast-PhoneGap-Plugin">
    https://github.com/EddyVerbruggen/Toast-PhoneGap-Plugin
  </a>
</p>


<p>This plugin allows you to show a native Toast (a little text popup) on iOS, Android and WP8. It&#39;s great for showing a non intrusive native notification which is guaranteed always in the viewport of the browser.</p>
<p>Requires Cordova plugin: <code>cordova-plugin-x-toast</code>. For more info, please see the <a href="https://github.com/EddyVerbruggen/Toast-PhoneGap-Plugin">Toast plugin docs</a>.</p>




<h2>Supported platforms</h2>
<ul>
  <li>Android</li><li>iOS</li><li>Windows Phone 8</li>
</ul>






<h2>Usage</h2>
<pre><code class="lang-typescript">import { Toast } from &#39;@ionic-native/toast&#39;;

constructor(private toast: Toast) { }

...

this.toast.show(&quot;I&#39;m a toast&quot;, &#39;5000&#39;, &#39;center&#39;).subscribe(
  toast =&gt; {
    console.log(toast);
  }
);
</code></pre>








<h2>Instance Members</h2>
<h3><a class="anchor" name="show" href="#show"></a><code>show(message,&nbsp;duration,&nbsp;position)</code></h3>




Show a native toast for the given duration at the specified position.

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
      message</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>The message to display.</p>
</td>
  </tr>
  
  <tr>
    <td>
      duration</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Duration to show the toast, either &#39;short&#39;, &#39;long&#39; or any number of milliseconds: &#39;1500&#39;.</p>
</td>
  </tr>
  
  <tr>
    <td>
      position</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Where to position the toast, either &#39;top&#39;, &#39;center&#39;, or &#39;bottom&#39;.</p>
</td>
  </tr>
  </tbody>
</table>

<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> Returns an Observable that notifies first on success and then when tapped, rejects on error.
</div><h3><a class="anchor" name="hide" href="#hide"></a><code>hide()</code></h3>


Manually hide any currently visible toast.


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> Returns a Promise that resolves on success.
</div><h3><a class="anchor" name="showWithOptions" href="#showWithOptions"></a><code>showWithOptions(options)</code></h3>




Show a native toast with the given options.

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
      <code>Object</code>
    </td>
    <td>
      <p>Options for showing a toast. Available options:
  message  The message to display.
  duration  Duration to show the toast, either &#39;short&#39;, &#39;long&#39; or any number of milliseconds: &#39;1500&#39;.
  position  Where to position the toast, either &#39;top&#39;, &#39;center&#39;, or &#39;bottom&#39;.
  addPixelsY  Offset in pixels to move the toast up or down from its specified position.</p>
</td>
  </tr>
  </tbody>
</table>

<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> Returns an Observable that notifies first on success and then when tapped, rejects on error.
</div><h3><a class="anchor" name="showShortTop" href="#showShortTop"></a><code>showShortTop(message)</code></h3>




Shorthand for `show(message, 'short', 'top')`.
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
      message</td>
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
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> Returns an Observable that notifies first on success and then when tapped, rejects on error.
</div><h3><a class="anchor" name="showShortCenter" href="#showShortCenter"></a><code>showShortCenter(message)</code></h3>




Shorthand for `show(message, 'short', 'center')`.
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
      message</td>
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
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> Returns an Observable that notifies first on success and then when tapped, rejects on error.
</div><h3><a class="anchor" name="showShortBottom" href="#showShortBottom"></a><code>showShortBottom(message)</code></h3>




Shorthand for `show(message, 'short', 'bottom')`.
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
      message</td>
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
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> Returns an Observable that notifies first on success and then when tapped, rejects on error.
</div><h3><a class="anchor" name="showLongTop" href="#showLongTop"></a><code>showLongTop(message)</code></h3>




Shorthand for `show(message, 'long', 'top')`.
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
      message</td>
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
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> Returns an Observable that notifies first on success and then when tapped, rejects on error.
</div><h3><a class="anchor" name="showLongCenter" href="#showLongCenter"></a><code>showLongCenter(message)</code></h3>




Shorthand for `show(message, 'long', 'center')`.
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
      message</td>
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
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> Returns an Observable that notifies first on success and then when tapped, rejects on error.
</div><h3><a class="anchor" name="showLongBottom" href="#showLongBottom"></a><code>showLongBottom(message)</code></h3>




Shorthand for `show(message, 'long', 'bottom')`.
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
      message</td>
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
  <b>Returns:</b> <code>Observable&lt;any&gt;</code> Returns an Observable that notifies first on success and then when tapped, rejects on error.
</div>





<h2><a class="anchor" name="ToastOptions" href="#ToastOptions"></a>ToastOptions</h2>

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
      message
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Message to display</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      duration
    </td>
    <td>
      <code>number</code>
    </td>
    <td>
      <p>Duration in ms to show</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      position
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Position</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      addPixelsY
    </td>
    <td>
      <code>number</code>
    </td>
    <td>
      <p>Add negative value to move it up a bit</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      data
    </td>
    <td>
      <code>any</code>
    </td>
    <td>
      <p>Pass JSON object to be sent back in success callback</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      styling
    </td>
    <td>
      <code>{
    opacity?: number;
    backgroundColor?: string;
    textColor?: string;
    cornerRadius?: number;
    horizontalPadding?: number;
    verticalPadding?: number;
  }</code>
    </td>
    <td>
      <p>Styling</p>

      <em>(optional)</em>
    </td>
  </tr>
  
  </tbody>
</table>





