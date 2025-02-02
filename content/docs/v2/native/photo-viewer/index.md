---
layout: "v2_fluid/docs_base"
version: "3.4.2"
versionHref: "/docs/v2/native"
path: ""
category: native
id: "photo-viewer"
title: "Photo Viewer"
header_sub_title: "Class in module "
doc: "Photo Viewer"
docType: "class"
---

<h1 class="api-title">Photo Viewer</h1>

<a class="improve-v2-docs" href="http://github.com/driftyco/ionic-native/edit/master/src/@ionic-native/plugins/photo-viewer/index.ts#L1">
  Improve this doc
</a>






<pre><code class="nohighlight">$ ionic plugin add com-sarriaroman-photoviewer
$ npm install --save @ionic-native/photo-viewer
</code></pre>
<p>Repo:
  <a href="https://github.com/sarriaroman/photoviewer">
    https://github.com/sarriaroman/photoviewer
  </a>
</p>


<p>This plugin can display your image in full screen with the ability to pan, zoom, and share the image.</p>




<h2>Supported platforms</h2>
<ul>
  <li>Android</li><li>iOS</li>
</ul>






<h2>Usage</h2>
<pre><code class="lang-typescript">import { PhotoViewer } from &#39;@ionic-native/photo-viewer&#39;;

constructor(private photoViewer: PhotoViewer) { }

...

this.photoViewer.show(&#39;https://mysite.com/path/to/image.jpg&#39;);

this.photoViewer.show(&#39;https://mysite.com/path/to/image.jpg&#39;, &#39;My image title&#39;, {share: false});
</code></pre>








<h2>Instance Members</h2>
<h3><a class="anchor" name="show" href="#show"></a><code>show(url,&nbsp;title,&nbsp;options)</code></h3>




Shows an image in full screen
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
      <p>URL or path to image</p>
</td>
  </tr>
  
  <tr>
    <td>
      title</td>
    <td>
      <code>string</code>
    </td>
    <td>
      </td>
  </tr>
  
  <tr>
    <td>
      options</td>
    <td>
      <code>any</code>
    </td>
    <td>
      </td>
  </tr>
  </tbody>
</table>







