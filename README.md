//video标签再ios下自动全屏问题解决办法

webkit-playsinline

给 video 标签增加 webkit-playsinline 属性，这个属性是为了让 video 视频在 ios 的 uiwebview 里面可以不全屏播放，默认 ios 会全屏播放视频，需要给 uiwebview 设置 allowsInlineMediaPlayback＝YES。 业界比较成熟的 videojs，可以根据不同平台选择不同的策略，例如 ios 使用 video 标签，pc 使用 flash 等


<pre class="prettyprint xml" style="color:#008080;"><span class="tag">&lt;<span class="title">video</span> <span class="attribute">autoplay</span> <span class="attribute">webkit-playsinline</span>&gt;</span>  
     <span class="tag">&lt;<span class="title">source</span> <span class="attribute">src</span>=<span class="value">"http://10.66.69.77:8080/hls/mystream.m3u8"</span> <span class="attribute">type</span>=<span class="value">"application/vnd.apple.mpegurl"</span> /&gt;</span>  
     <span class="tag">&lt;<span class="title">p</span> <span class="attribute">class</span>=<span class="value">"warning"</span>&gt;</span>Your browser does not support HTML5 video.<span class="tag">&lt;/<span class="title">p</span>&gt;</span>  
 <span class="tag">&lt;/<span class="title">video</span>&gt;</span></pre>

