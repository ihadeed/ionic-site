---
layout: "v2_fluid/docs_base"
version: "3.4.2"
versionHref: "/docs/v2/native"
path: ""
category: native
id: "streaming-media"
title: "Streaming Media"
header_sub_title: "Class in module "
doc: "Streaming Media"
docType: "class"
---

<h1 class="api-title">Streaming Media</h1>

<a class="improve-v2-docs" href="http://github.com/driftyco/ionic-native/edit/master/src/@ionic-native/plugins/streaming-media/index.ts#L16">
  Improve this doc
</a>






<pre><code class="nohighlight">$ ionic plugin add cordova-plugin-streaming-media
$ npm install --save @ionic-native/streaming-media
</code></pre>
<p>Repo:
  <a href="https://github.com/nchutchind/cordova-plugin-streaming-media">
    https://github.com/nchutchind/cordova-plugin-streaming-media
  </a>
</p>


<p>This plugin allows you to stream audio and video in a fullscreen, native player on iOS and Android.</p>




<h2>Supported platforms</h2>
<ul>
  <li>Android</li><li>iOS</li>
</ul>






<h2>Usage</h2>
<pre><code>import { StreamingMedia, StreamingVideoOptions } from &#39;@ionic-native/streaming-media&#39;;

constructor(private streamingMedia: StreamingMedia) { }

let options: StreamingVideoOptions = {
  successCallback: () =&gt; { console.log(&#39;Video played&#39;) },
  errorCallback: (e) =&gt; { console.log(&#39;Error streaming&#39;) },
  orientation: &#39;landscape&#39;
};

this.streamingMedia.playVideo(&#39;https://path/to/video/stream&#39;, options);
</code></pre>








<h2>Instance Members</h2>
<h3><a class="anchor" name="playVideo" href="#playVideo"></a><code>playVideo(videoUrl,&nbsp;options)</code></h3>




Streams a video
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
      videoUrl</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>The URL of the video</p>
</td>
  </tr>
  
  <tr>
    <td>
      options</td>
    <td>
      <code>StreamingVideoOptions</code>
    </td>
    <td>
      <p>Options</p>
</td>
  </tr>
  </tbody>
</table>

<h3><a class="anchor" name="playAudio" href="#playAudio"></a><code>playAudio(audioUrl,&nbsp;options)</code></h3>




Streams an audio
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
      audioUrl</td>
    <td>
      <code>string</code>
    </td>
    <td>
      <p>The URL of the audio stream</p>
</td>
  </tr>
  
  <tr>
    <td>
      options</td>
    <td>
      <code>StreamingAudioOptions</code>
    </td>
    <td>
      <p>Options</p>
</td>
  </tr>
  </tbody>
</table>

<h3><a class="anchor" name="stopAudio" href="#stopAudio"></a><code>stopAudio()</code></h3>




Stops streaming audio



<h3><a class="anchor" name="pauseAudio" href="#pauseAudio"></a><code>pauseAudio()</code></h3>



<p>
  <strong>Platforms:</strong><strong class="tag">iOS</strong>&nbsp;</p>


Pauses streaming audio



<h3><a class="anchor" name="resumeAudio" href="#resumeAudio"></a><code>resumeAudio()</code></h3>



<p>
  <strong>Platforms:</strong><strong class="tag">iOS</strong>&nbsp;</p>


Resumes streaming audio









<h2><a class="anchor" name="StreamingVideoOptions" href="#StreamingVideoOptions"></a>StreamingVideoOptions</h2>

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
      successCallback
    </td>
    <td>
      <code>Function</code>
    </td>
    <td>
      
      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      errorCallback
    </td>
    <td>
      <code>Function</code>
    </td>
    <td>
      
      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      orientation
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      
      <em>(optional)</em>
    </td>
  </tr>
  
  </tbody>
</table>


<h2><a class="anchor" name="StreamingAudioOptions" href="#StreamingAudioOptions"></a>StreamingAudioOptions</h2>

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
      bgColor
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      
      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      bgImage
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      
      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      bgImageScale
    </td>
    <td>
      <code>string</code>
    </td>
    <td>
      
      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      initFullscreen
    </td>
    <td>
      <code>boolean</code>
    </td>
    <td>
      
      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      successCallback
    </td>
    <td>
      <code>Function</code>
    </td>
    <td>
      
      <em>(optional)</em>
    </td>
  </tr>
  
  <tr>
    <td>
      errorCallback
    </td>
    <td>
      <code>Function</code>
    </td>
    <td>
      
      <em>(optional)</em>
    </td>
  </tr>
  
  </tbody>
</table>





