# iFrameSizer
Use jQuery to resize an iFrame proportionally. Ideally used for sizing iframe-based videos like Vimeo.

# Example Of Use
````
<style>
.videoWrapper,
.videoBorder {
  display: block;
  width: 100%;
}
</style>

<div class="videoWrapper" data-instructions='{"ratio":["16","9"]}'>
  <div class="videoBorder">
    <iframe src="//player.vimeo.com/video/1234567890" class="videoscope" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="width: 100%;"></iframe>
  </div>
</div>

<script>
// Instantiate
var VideoSizer = new iFrameSizer($);
// Create listener for these objects
VideoSizer.observer('div.videoWrapper',$('.videoBorder'),$('.videoscope'));
</script>

````
