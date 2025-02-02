---
layout: "v2_fluid/docs_base"
version: "3.4.2"
versionHref: "/docs/v2/native"
path: ""
category: native
id: "twitter-connect"
title: "Twitter Connect"
header_sub_title: "Class in module "
doc: "Twitter Connect"
docType: "class"
---

<h1 class="api-title">Twitter Connect</h1>

<a class="improve-v2-docs" href="http://github.com/driftyco/ionic-native/edit/master/src/@ionic-native/plugins/twitter-connect/index.ts#L20">
  Improve this doc
</a>






<pre><code class="nohighlight">$ ionic plugin add twitter-connect-plugin --variable FABRIC_KEY=fabric_API_key
$ npm install --save @ionic-native/twitter-connect
</code></pre>
<p>Repo:
  <a href="https://github.com/ManifestWebDesign/twitter-connect-plugin">
    https://github.com/ManifestWebDesign/twitter-connect-plugin
  </a>
</p>


<p>Plugin to use Twitter Single Sign On
Uses Twitter&#39;s Fabric SDK</p>
<pre><code class="lang-typescript">import { TwitterConnect } from &#39;@ionic-native/twitter-connect&#39;;

constructor(private twitter: TwitterConnect) { }

...

function onSuccess(response) {
  console.log(response);

  // Will console log something like:
  // {
  //   userName: &#39;myuser&#39;,
  //   userId: &#39;12358102&#39;,
  //   secret: &#39;tokenSecret&#39;
  //   token: &#39;accessTokenHere&#39;
  // }
}

this.twitter.login().then(onSuccess, onError);

this.twitter.logout().then(onLogoutSuccess, onLogoutError);
</code></pre>















<h2>Instance Members</h2>
<h3><a class="anchor" name="login" href="#login"></a><code>login()</code></h3>


Logs in


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;TwitterConnectResponse&gt;</code> returns a promise that resolves if logged in and rejects if failed to login
</div><h3><a class="anchor" name="logout" href="#logout"></a><code>logout()</code></h3>


Logs out


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> returns a promise that resolves if logged out and rejects if failed to logout
</div><h3><a class="anchor" name="showUser" href="#showUser"></a><code>showUser()</code></h3>


Returns user's profile information


<div class="return-value" markdown="1">
  <i class="icon ion-arrow-return-left"></i>
  <b>Returns:</b> <code>Promise&lt;any&gt;</code> returns a promise that resolves if user profile is successfully retrieved and rejects if request fails
</div>





<h2><a class="anchor" name="TwitterConnectResponse" href="#TwitterConnectResponse"></a>TwitterConnectResponse</h2>

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
      userName
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Twitter Username</p>

      
    </td>
  </tr>
  
  <tr>
    <td>
      userId
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Twitter User ID</p>

      
    </td>
  </tr>
  
  <tr>
    <td>
      secret
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Twitter OAuth Secret</p>

      
    </td>
  </tr>
  
  <tr>
    <td>
      token
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>Twitter OAuth Token</p>

      
    </td>
  </tr>
  
  </tbody>
</table>





