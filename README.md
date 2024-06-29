# meinv 
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>看美女</title>
	<style>  
	</style>
	<link rel="icon" href="img/kk.png">
</head>  
<body>  
  <ul id="sidebar">
                  <li class="box-b mb20">
                      <span class="arrow-right"></span>
                      <h3 class="title pt10 pl10">
                          <span>每天看小姐姐预防老年痴呆</span>
                      </h3>
                      <div class="zz-list lh200 p10">
                          <style type="text/css">
                              #buttons {
                                  text-align: center;
                                  height: 50px;
                              }
  
                              #switch, #more, #next {
                                  background: #FFF;
                                  background: linear-gradient(to bottom, #FF2,#FB0);
                                  color: #AF2E08;
                                  font-size: 16px;
                                  font-weight: bold;
                                  height: 25px;
                                  padding: 0px 20px;
                                  margin: 0px 5px;
                                  border-radius: 20px;
                              }
                          </style>
                          <section id="main">
                              <video width="100%" height="400px" id="player" src="" controls="" webkit-playsinline="" playsinline="" muted poster="/content/uploadfile/tpl_options//logopic.png" preload="none"></video>
                          </section>
                          <section id="buttons">
                              <button id="switch">连续: 关</button>
                              <button id="next">播放下一个</button>
                              <button id="more" onclick="window.open('https://www.baidu.com/')">前往百度</button>
                          </section>
                          <script>
                              (function(window, document) {
                                  if (top != self) {
                                      window.top.location.replace(self.location.href);
                                  }
                                  var get = function(id) {
                                      return document.getElementById(id);
                                  }
                                  var bind = function(element, event, callback) {
                                      return element.addEventListener(event, callback);
                                  }
                                  var auto = false;
                                  var player = get('player');
                                  var randomm = function() {
                                      player.src = 'http://v.nrzj.vip/video.php?_t=0.0001703800875445527';
                                      player.volume = 0.2;
                                      player.play();
  
                                  }
                                  bind(get('next'), 'click', randomm);
                                  bind(player, 'error', function() {
                                      randomm();
                                  });
                                  bind(get('switch'), 'click', function() {
                                      auto = !auto;
                                      this.innerText = '连续: ' + (auto ? '开' : '关');
                                  });
                                  bind(player, 'ended', function() {
                                      if (auto)
                                          randomm();
                                  });
                              }
                              )(window, document);
                          </script>
                      </div>
                  </li>
              </ul>
</body>  
</html>
