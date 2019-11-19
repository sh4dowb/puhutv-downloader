<html>
<head>
  <meta charset="UTF-8">
  <style>*{font-family:Arial;}a{text-decoration:none;}</style>
  <link rel="stylesheet" href="https://unpkg.com/purecss@0.6.2/build/forms-min.css">
  <link rel="stylesheet" href="https://unpkg.com/purecss@0.6.2/build/buttons-min.css">
  <title>puhutv indirici</title>
</head>
<body>
  <a target="_blank" href="https://github.com/sh4dowb/puhutv-downloader"><img style="position: absolute; top: 0; left: 0; border: 0;" src="https://s3.amazonaws.com/github/ribbons/forkme_left_red_aa0000.png" alt="Fork me on GitHub"></a>
  <center>
    <form method="post" class="pure-form"><b>tekrardan çalışıyor!</b><br><br>
      puhutv bölüm <b>izleme</b> linki: <br><input type="text" id="link" placeholder="https://puhutv.com/cember-7-bolum-hayalet-gemi-izle" style="height:40px;width:400px;"><br>
      <button id="download" type="submit" class="pure-button pure-input-1-2 pure-button-primary" style="width:100px;">indir</button>
    </form>
    <br>
    <p id="log" style="font-size:70%;"></p>
    <div id="videos"></div><br>
    <span>not: VPN kullanıyorsanız videolar açılmayabilir.<br>not 2: tüm kaliteler (örn. 2160p) var olmayabilir.</span>
    <!-- <span style="display:hidden;">yeni güncelleme yüzünden "sağ tık -> farklı kaydet" mümkün değil.<br>lütfen önce linke tıklayın, yönlendirmeden sonra ctrl-s veya sağ tık yaparak kaydedin.</span> -->
    <script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
    <script>
      $("#download").click(function(e){
       e.preventDefault();
       $(this).attr("disabled","disabled");
       $("#videos").text("");
       $("#log").text("");
       $("#log").append("bölüm ID alınıyor...<br>");
       $.ajax({
        url: $("#link").val().replace('-detay','-izle'),
        success: function(data){
	console.log(data.split("player.video.loader(")[1].split("', '"));
         var episode_id = data.split("player.video.loader(")[1].split("', '")[1];
         $("#log").append("bölüm ID: "+episode_id+"<br>");

        $("#log").append("Video listesi alınıyor...<br>");
        getvideos(episode_id);
      },
      error: function(xhr, status, error){
       $("#log").append("<font color=\"red\">hata: bölüm ID alınamadı. lütfen tekrar deneyin.</font><br>");
       $("#download").removeAttr("disabled");
     }
   });
     });
      var replacequalities = {"720p": "<b>720p</b>", "1080p": "<b>1080p</b>", "1440p": '<b style="color:limegreen;">1440p</b>', "2160p": '<b style="color:limegreen;">2160p</b>'};
      function getvideos(episode_id){
       $.ajax({
        url: "https://dygvideo.dygdigital.com/api/video_info?akamai=true&PublisherId=29&ReferenceId="+episode_id+"&SecretKey=NtvApiSecret2014*",
        dataType: "json",
        async: true,
        success: function(data){
         var source = data.data.flavors.hls;
         var videos = [];
         var qualities = ["144","240","360","480","720","1080","2160"];
         for(var i in qualities)
         {
           //var realsrc = source.url.split('/mp4/')[0] + "/mp4/" + source.quality.toString() + "p.mp4?" + source.url.split('.mp4?')[1];
           // videos.push(["https://cagriari.com/referer.php?to=" + realsrc, source.quality]);

           videos.push([source.replace(/hls\/.*?playlist\.m3u8/gi,'mp4/'+qualities[i]+'p.mp4'), qualities[i]]);
       }
/*       videos.sort(function(x, y) {
        if (x[1] < y[1]) {
          return 1;
        }
        if (x[1] > y[1]) {
          return -1;
        }
        return 0;
      });
*/
       for(var i in videos){
        var video = videos[i];
        var qualityfixed = video[1].toString() + "p";
        if(qualityfixed in replacequalities)
          qualityfixed = replacequalities[qualityfixed];
        $("#videos").append('<a href="'+video[0]+'" target="_blank">'+ qualityfixed +'</a><br>');
      }

      $("#download").removeAttr("disabled");
    },
    error: function(){
     $("#log").append("<font color=\"red\">hata: video listesi alınamadı, lütfen tekrar deneyin.</font><br>");
     $("#download").removeAttr("disabled");
   }
 });
     }
   </script>
 </center>
</body>
</html>
