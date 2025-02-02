---
layout: "v2_fluid/docs_base"
version: "3.4.2"
versionHref: "/docs/v2/native"
path: ""
category: native
id: "browser-tab"
title: "Browser Tab"
header_sub_title: "Class in module "
doc: "Browser Tab"
docType: "class"
---

<h1 class="api-title">Browser Tab</h1>

<a class="improve-v2-docs" href="http://github.com/driftyco/ionic-native/edit/master/src/@ionic-native/plugins/browser-tab/index.ts#L1">
  Improve this doc
</a>






<pre><code class="nohighlight">$ ionic plugin add cordova-plugin-browsertab
$ npm install --save @ionic-native/browser-tab
</code></pre>
<p>Repo:
  <a href="https://github.com/google/cordova-plugin-browsertab">
    https://github.com/google/cordova-plugin-browsertab
  </a>
</p>


<p>This plugin provides an interface to in-app browser tabs that exist on some mobile platforms, specifically <a href="http://developer.android.com/tools/support-library/features.html#custom-tabs">Custom Tabs</a> on Android (including the <a href="https://developer.chrome.com/multidevice/android/customtabs">Chrome Custom Tabs</a> implementation), and <a href="https://developer.apple.com/library/ios/documentation/SafariServices/Reference/SFSafariViewController_Ref/">SFSafariViewController</a> on iOS.</p>




<h2>Supported platforms</h2>
<ul>
  <li>Android</li><li>iOS</li>
</ul>






<h2>Usage</h2>
<pre><code>import { BrowserTab } from &#39;@ionic-native/browser-tab&#39;;

constructor(private browserTab: BrowserTab) {

  browserTab.isAvailable()
    .then((isAvailable: boolean) =&gt; {

      if (isAvailable) {

        browserTab.openUrl(&#39;https://ionic.io&#39;);

      } else {

        // open URL with InAppBrowser instead or SafariViewController

      }

    });


}
</code></pre>








<h2>Instance Members</h2>
<h3><a class="anchor" name="isAvailable" href="#isAvailable"></a><code>isAvailable()</code></h3>


Check if BrowserTab option is available


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> Returns a promise that resolves when check is successful and returns true or false
</div><h3><a class="anchor" name="openUrl" href="#openUrl"></a><code>openUrl(url)</code></h3>


Opens the provided URL using a browser tab
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
      url</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>The URL you want to open</p>
</td>
  </tr>
  </tbody>
</table>

<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> Returns a promise that resolves when check open was successful
</div><h3><a class="anchor" name="close" href="#close"></a><code>close()</code></h3>


Closes browser tab


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> Returns a promise that resolves when close was finished
</div>





