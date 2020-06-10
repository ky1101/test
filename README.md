<!Doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>js-연습</title>
    <script>
      function nightday(self){
        var target = document.querySelector('body');
        if(self.value === 'night'){
          target.style.backgroundColor = 'black';
          target.style.color = 'white';
          self.value = 'day';

          var alist = document.querySelectorAll('a');
          var i = 0;
          while(i < alist.length){
            alist[i].style.color = 'powderblue';
            i = i + 1;
          }
        } else {
          target.style.backgroundColor = 'white';
          target.style.color = 'black';
          self.value = 'night';

          var alist = document.querySelectorAll('a');
          var i = 0;
          while(i < alist.length){
            alist[i].style.color = 'blue';
            i = i + 1;
          }
        }
      }
    </script>
  </head>
  <body>
    <a href="https://www.twitch.tv/sal_gu" target="_blank" title="sal_gu">sal_gu</a>
    <a href="https://www.youtube.com/channel/UCoGlmInGRIRoDg4NjAYv4-Q" target="_blank" title="sal_gu">레지나</a>
    <input id="night_day" type="button" value="night" onclick="
    nightday(this)
    ">
<h1>바보!</h1>
  </body>
</html>

