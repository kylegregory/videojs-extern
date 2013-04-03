# Video.js - Extern Plugin
Allow you to play external videos from YouTube or Vimeo. More to come, let me know which one you need.

## How does it work?
This isn't really a plugin you have to register. Just by including media.X.js, you can use this by adding a new source with type="video/X"

Here is an example with YouTube:

	<video id="vid1" class="video-js vjs-default-skin" controls preload="auto" width="640" height="264">
	  <source src="http://www.youtube.com/watch?v=ebO5jK5NKXw" type="video/youtube">
	  <p>Video Playback Not Supported</p>
	</video>
	
	<script>
	vid1 = vjs('vid1', { techOrder: ['youtube'] });
	</script>

Here is an example with Vimeo:

	<video id="vid1" class="video-js vjs-default-skin" controls preload="auto" width="640" height="264">
	  <source src="https://vimeo.com/62596239" type="video/vimeo">
	  <p>Video Playback Not Supported</p>
	</video>
	
	<script>
	vid1 = vjs('vid1', { techOrder: ['vimeo'] });
	</script>

If you want to use the YouTube control instead of Video.js, you can set the option ytcontrol to true.

You cannot use the Video.js control with Vimeo. They do not allow it.

##Special Thank You
Thanks to John Hurliman for the original code on the old Video.js