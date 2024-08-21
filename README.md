<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>猫猫与老鼠的世界</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background: #f0f0f0;
        }
        header {
            background: #333;
            color: white;
            padding: 1rem;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        header h1 {
            margin: 0;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            margin-top: 1rem;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
            font-weight: bold;
        }
        nav a:hover {
            background: #575757;
            border-radius: 5px;
        }
        .container {
            padding: 2rem;
            max-width: 1200px;
            margin: 6rem auto 2rem;
        }
        .section {
            margin-bottom: 2rem;
            text-align: center;
        }
        .section img, .section video {
            max-width: 100%;
            border-radius: 10px;
            margin: 1rem 0;
        }
        .section h2 {
            margin-bottom: 1rem;
        }
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 1rem;
        }
        .fade-in {
            animation: fadeIn 2s ease-in;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .scroll-up {
            position: fixed;
            bottom: 1rem;
            right: 1rem;
            background: #333;
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            cursor: pointer;
        }
        .scroll-up:hover {
            background: #575757;
        }
    </style>
</head>
<body>
    <header>
        <h1>猫猫与老鼠的世界</h1>
        <nav>
            <a href="#home">首页</a>
            <a href="#about">关于我们</a>
            <a href="#gallery">图库</a>
            <a href="#contact">联系方式</a>
        </nav>
    </header>
    <div class="container">
        <section id="home" class="section fade-in">
            <h2>欢迎来到猫猫与老鼠的世界</h2>
            <p>这是一个展示猫猫和老鼠的美丽图片和视频的网站。希望你喜欢这些有趣的内容！</p>
            <img src="https://example.com/cat-image.jpg" alt="猫猫" />
            <video controls>
                <source src="https://example.com/cat-video.mp4" type="video/mp4">
                你的浏览器不支持视频播放。
            </video>
        </section>
        <section id="about" class="section fade-in">
            <h2>关于我们</h2>
            <p>我们专注于展示可爱的猫猫和有趣的老鼠内容，致力于为你带来欢笑和快乐。</p>
        </section>
        <section id="gallery" class="section fade-in">
            <h2>图库</h2>
            <img src="https://example.com/mouse-image.jpg" alt="老鼠" />
            <img src="https://example.com/cat-image2.jpg" alt="猫猫" />
        </section>
        <section id="contact" class="section fade-in">
            <h2>联系方式</h2>
            <p>如果你有任何问题或建议，请通过以下方式联系我。</p>
            <form>
                <input type="text" name="name" placeholder="你的名字" required>
                <input type="email" name="email" placeholder="你的邮箱" required>
                <textarea name="message" rows="5" placeholder="你的留言" required></textarea>
                <button type="submit">发送</button>
            </form>
        </section>
    </div>
    <footer>
        <p>&copy; 2024 猫猫与老鼠的世界. 版权所有.</p>
    </footer>
    <div class="scroll-up" onclick="scrollToTop()">返回顶部</div>
    <script>
        function scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }
    </script>
</body>
</html>
