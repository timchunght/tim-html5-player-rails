This is a HTML5 Video Player built on top of mediaelement; ready to use with Rails

1) To use the Video player, copy the three folders into the assets directory and replace/merge them with the existing folders

2) Go to `layout/application.html.erb` and paste the following code within the header

```bash
  <script>
  $(document).ready(function() {
    $('video').mediaelementplayer({
      alwaysShowControls: false,
      videoVolume: 'horizontal',
      features: ['playpause','progress','volume','fullscreen']
    });
  });
  </script>
```