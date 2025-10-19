<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-widteh, initis
     -scale=1.0">
  <meta http-equive="X-UA-Compatible" content="ie=edge">
  <title>Document</title>

</heard>
<body>
  <video id="myVideo" autoplay muted loop playsinline>
  <source src="material.mp4" type="video/mp4"
</video>


<script>
  const video = document.getElementById("myVideo");
  video.addEventListener("canplay", async ( ) => {
    try {
      if (video.requestFullscreen) {
        await video.requestFullscreen();
      } else if (video.webkitRequestFullscreen) {
        await video.webkitRequestFullscreen();
      }
      video.play() ;
    } catch (e) { console.log(e); }
  }):
  document.body.addEventListener("click", ( ) => {
    video.muted = false;
    video.play();
  }):
</script>
</body>
</html>
