
<!DOCTYPE html>
<html lang="zh">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Phantom视频播放器</title>
  <style>
    :root {
      --primary-color: #4a90e2;
      --overlay-bg: rgba(0,0,0,0.7);
    }
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    html, body {
      width: 100%;
      height: 100%;
      overflow: hidden;
      background: #000;
      font-family: 'Arial', sans-serif;
    }
    #video-container {
      position: relative;
      width: 100%;
      height: 100%;
    }
    video {
      width: 100%;
      height: 100%;
      object-fit: contain;
    }
    #overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background: var(--overlay-bg);
      color: #fff;
      font-size: 1.5rem;
      cursor: pointer;
      z-index: 10;
      transition: opacity 0.3s ease;
    }
    #overlay-text {
      margin-bottom: 1rem;
      text-align: center;
      max-width: 80%;
    }
    #play-btn {
      padding: 0.8rem 1.5rem;
      background: var(--primary-color);
      color: white;
      border: none;
      border-radius: 4px;
      font-size: 1rem;
      cursor: pointer;
      transition: transform 0.2s ease;
    }
    #play-btn:hover {
      transform: scale(1.05);
    }
    #error-message {
      display: none;
      color: #ff6b6b;
      margin-top: 1rem;
    }
    #loading {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      color: white;
      z-index: 5;
    }
  </style>
</head>
<body>
  <div id="video-container">
    <div id="loading">视频加载中...</div>
    <video id="video" autoplay muted loop playsinline>
      <source src="videos/Phantom.mp4" type="video/mp4">
      <source src="videos/Phantom.webm" type="video/webm">
      您的浏览器不支持HTML5视频播放
    </video>
    <div id="overlay">
      <div id="overlay-text">点击下方按钮开始播放声音</div>
      <button id="play-btn">播放声音</button>
      <div id="error-message"></div>
    </div>
  </div>

  <script>
    const video = document.getElementById('video');
    const overlay = document.getElementById('overlay');
    const playBtn = document.getElementById('play-btn');
    const errorMsg = document.getElementById('error-message');
    const loading = document.getElementById('loading');

    // 视频加载状态检测
    video.addEventListener('waiting', () => {
      loading.style.display = 'block';
    });
    
    video.addEventListener('playing', () => {
      loading.style.display = 'none';
    });

    // 自动播放尝试
    const tryAutoplay = () => {
      video.play()
        .then(() => {
          console.log('自动播放成功');
        })
        .catch(err => {
          console.log('自动播放受限:', err);
          errorMsg.textContent = '提示：请点击按钮解除静音播放';
          errorMsg.style.display = 'block';
        });
    };

    // 激活声音播放
    const enableSound = () => {
      video.muted = false;
      video.play()
        .then(() => {
          overlay.style.opacity = '0';
          setTimeout(() => {
            overlay.style.display = 'none';
          }, 300);
        })
        .catch(err => {
          errorMsg.textContent = '播放失败: ' + err.message;
          errorMsg.style.display = 'block';
        });
    };

    // 事件监听
    playBtn.addEventListener('click', enableSound);
    overlay.addEventListener('click', enableSound);

    // 初始化
    window.addEventListener('DOMContentLoaded', () => {
      tryAutoplay();
      
      // 视频错误处理
      video.addEventListener('error', () => {
        errorMsg.textContent = `视频加载失败，请检查路径：${video.querySelector('source').src}`;
        errorMsg.style.display = 'block';
        loading.style.display = 'none';
      });
    });
  </script>
</body>
</html>
