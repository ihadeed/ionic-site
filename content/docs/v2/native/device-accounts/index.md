---
layout: "v2_fluid/docs_base"
version: "3.4.2"
versionHref: "/docs/v2/native"
path: ""
category: native
id: "device-accounts"
title: "Device Accounts"
header_sub_title: "Class in module "
doc: "Device Accounts"
docType: "class"
---

<h1 class="api-title">Device Accounts</h1>

<a class="improve-v2-docs" href="http://github.com/driftyco/ionic-native/edit/master/src/@ionic-native/plugins/device-accounts/index.ts#L1">
  Improve this doc
</a>






<pre><code class="nohighlight">$ ionic plugin add https://github.com/loicknuchel/cordova-device-accounts.git
$ npm install --save @ionic-native/device-accounts
</code></pre>
<p>Repo:
  <a href="https://github.com/loicknuchel/cordova-device-accounts">
    https://github.com/loicknuchel/cordova-device-accounts
  </a>
</p>


<p>Gets the Google accounts associated with the Android device</p>




<h2>Supported platforms</h2>
<ul>
  <li>Android</li>
</ul>






<h2>Usage</h2>
<pre><code class="lang-typescript">import { DeviceAccounts } from &#39;@ionic-native/device-accounts&#39;;

constructor(private deviceAccounts: DeviceAccounts) { }

...

this.deviceAccounts.get()
  .then(accounts =&gt; console.log(accounts))
  .catch(error =&gt; console.error(error));
</code></pre>








<h2>Instance Members</h2>
<h3><a class="anchor" name="get" href="#get"></a><code>get()</code></h3>


Gets all accounts registered on the Android Device


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="getByType" href="#getByType"></a><code>getByType()</code></h3>


Get all accounts registered on Android device for requested type


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="getEmails" href="#getEmails"></a><code>getEmails()</code></h3>


Get all emails registered on Android device (accounts with 'com.google' type)


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div><h3><a class="anchor" name="getEmail" href="#getEmail"></a><code>getEmail()</code></h3>


Get the first email registered on Android device


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> 
</div>





