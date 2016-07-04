webkit-playsinline

给 video 标签增加 webkit-playsinline 属性，这个属性是为了让 video 视频在 ios 的 uiwebview 里面可以不全屏播放，默认 ios 会全屏播放视频，需要给 uiwebview 设置 allowsInlineMediaPlayback＝YES。 业界比较成熟的 videojs，可以根据不同平台选择不同的策略，例如 ios 使用 video 标签，pc 使用 flash 等
