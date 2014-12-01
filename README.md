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

3) The following is sample code to paste into `body`
```bash

<video width="640" height="267">
    <source src="http://embed.wistia.com/deliveries/afe41e4a3b366c5599fb17d96c469ad85007e2df/file.mp4" type="video/mp4">
</video>
```
![Alt text](https://raw.githubusercontent.com/timchunght/tim-html5-player-rails/master/tim-html5-video.png)

Click [demo](https://timplayer.herokuapp.com/) for a live version.

You can also fork the demo app [here](https://github.com/timchunght/timplayerdemo)

Modified and Styled by Timothy Chung

Copyright [Timothy Chung](www.linkedin.com/in/timchunght)

Please feel free to use it for any of your projects

Special thanks to Designmodo for their free UI assets!
