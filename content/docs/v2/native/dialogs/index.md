---
layout: "v2_fluid/docs_base"
version: "3.4.2"
versionHref: "/docs/v2/native"
path: ""
category: native
id: "dialogs"
title: "Dialogs"
header_sub_title: "Class in module "
doc: "Dialogs"
docType: "class"
---

<h1 class="api-title">Dialogs</h1>

<a class="improve-v2-docs" href="http://github.com/driftyco/ionic-native/edit/master/src/@ionic-native/plugins/dialogs/index.ts#L16">
  Improve this doc
</a>






<pre><code class="nohighlight">$ ionic plugin add cordova-plugin-dialogs
$ npm install --save @ionic-native/dialogs
</code></pre>
<p>Repo:
  <a href="https://github.com/apache/cordova-plugin-dialogs.git">
    https://github.com/apache/cordova-plugin-dialogs.git
  </a>
</p>


<p>This plugin gives you ability to access and customize the device native dialogs.</p>
<p>Requires Cordova plugin: <code>cordova-plugin-dialogs</code>. For more info, please see the <a href="https://github.com/apache/cordova-plugin-dialogs">Dialogs plugin docs</a>.</p>




<h2>Supported platforms</h2>
<ul>
  <li>Android</li><li>BlackBerry 10</li><li>Firefox OS</li><li>iOS</li><li>Ubuntu</li><li>Windows</li><li>Windows Phone</li>
</ul>






<h2>Usage</h2>
<pre><code class="lang-typescript">import { Dialogs } from &#39;@ionic-native/dialogs&#39;;

constructor(private dialogs: Dialogs) { }

...

this.dialogs.alert(&#39;Hello world&#39;)
  .then(() =&gt; console.log(&#39;Dialog dismissed&#39;))
  .catch(e =&gt; console.log(&#39;Error displaying dialog&#39;, e));
</code></pre>








<h2>Instance Members</h2>
<h3><a class="anchor" name="alert" href="#alert"></a><code>alert(message,&nbsp;title,&nbsp;buttonName)</code></h3>




Shows a custom alert or dialog box.
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
      <p>Dialog message.</p>
</td>
  </tr>
  
  <tr>
    <td>
      title</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Dialog title. (Optional, defaults to Alert)</p>
</td>
  </tr>
  
  <tr>
    <td>
      buttonName</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Button name. (Optional, defaults to OK)</p>
</td>
  </tr>
  </tbody>
</table>

<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> Returns a blank promise once the user has dismissed the alert.
</div><h3><a class="anchor" name="confirm" href="#confirm"></a><code>confirm(message,&nbsp;title,&nbsp;buttonLabels)</code></h3>




Displays a customizable confirmation dialog box.
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
      <p>Dialog message.</p>
</td>
  </tr>
  
  <tr>
    <td>
      title</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Dialog title. (Optional, defaults to Confirm)</p>
</td>
  </tr>
  
  <tr>
    <td>
      buttonLabels</td>
    <td>
      <code>Array&lt;string&gt;</code>
    </td>
    <td>
      <p>Array of strings specifying button labels. (Optional, defaults to [OK,Cancel])</p>
</td>
  </tr>
  </tbody>
</table>

<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;number&gt;</code> Returns a promise that resolves the button index that was clicked. Note that the index use one-based indexing.
</div><h3><a class="anchor" name="prompt" href="#prompt"></a><code>prompt(message,&nbsp;title,&nbsp;buttonLabels,&nbsp;defaultText)</code></h3>




Displays a native dialog box that is more customizable than the browser's prompt function.
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
      <p>Dialog message.</p>
</td>
  </tr>
  
  <tr>
    <td>
      title</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Dialog title. (Optional, defaults to Prompt)</p>
</td>
  </tr>
  
  <tr>
    <td>
      buttonLabels</td>
    <td>
      <code>Array&lt;string&gt;</code>
    </td>
    <td>
      <p>Array of strings specifying button labels. (Optional, defaults to [&quot;OK&quot;,&quot;Cancel&quot;])</p>
</td>
  </tr>
  
  <tr>
    <td>
      defaultText</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Default textbox input value.  (Optional, Default: empty string)</p>
</td>
  </tr>
  </tbody>
</table>

<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;DialogsPromptCallback&gt;</code> Returns a promise that resolves an object with the button index clicked and the text entered
</div><h3><a class="anchor" name="beep" href="#beep"></a><code>beep(times)</code></h3>




The device plays a beep sound.
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
      times</td>
    <td>
      <code>numbers</code>
    </td>
    <td>
      <p>The number of times to repeat the beep.</p>
</td>
  </tr>
  </tbody>
</table>







<h2><a class="anchor" name="DialogsPromptCallback" href="#DialogsPromptCallback"></a>DialogsPromptCallback</h2>

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
      buttonIndex
    </td>
    <td>
      <code>number</code>
    </td>
    <td>
      <p>The index of the pressed button. (Number) Note that the index uses one-based indexing, so the value is 1, 2, 3, etc.</p>

      
    </td>
  </tr>
  
  <tr>
    <td>
      input1
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>The text entered in the prompt dialog box. (String)</p>

      
    </td>
  </tr>
  
  </tbody>
</table>





