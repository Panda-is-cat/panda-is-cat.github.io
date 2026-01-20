<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Panda is Cat | 熊猫即猫</title>
    <style>
        :root {
            --bg-color: #f9f9f9;
            --text-color: #333;
            --accent-color: #2c3e50; /* 深蓝灰色 */
            --card-bg: #ffffff;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }

        /* 顶部导航 */
        header {
            background-color: var(--accent-color);
            color: white;
            padding: 2rem 1rem;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 2.5rem;
            font-weight: 700;
        }

        header p {
            font-size: 1.1rem;
            opacity: 0.9;
            margin-top: 10px;
        }

        /* 熊猫/猫的Emoji装饰 */
        .mascot {
            font-size: 3rem;
            margin-bottom: 10px;
            display: block;
        }

        /* 主容器 */
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 2rem 1rem;
        }

        /* 简介卡片 */
        .intro-card {
            background: var(--card-bg);
            padding: 2rem;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            text-align: center;
            margin-bottom: 3rem;
        }

        /* 博客文章列表 */
        .post-list {
            list-style: none;
            padding: 0;
        }

        .post-item {
            background: var(--card-bg);
            margin-bottom: 1.5rem;
            padding: 1.5rem;
            border-radius: 8px;
            border-left: 5px solid var(--accent-color);
            transition: transform 0.2s ease;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }

        .post-item:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0,0,0,0.1);
        }

        .post-date {
            font-size: 0.85rem;
            color: #888;
        }

        .post-title {
            font-size: 1.5rem;
            margin: 0.5rem 0;
            color: var(--accent-color);
        }

        .post-excerpt {
            color: #555;
        }

        /* 底部 */
        footer {
            text-align: center;
            padding: 2rem;
            color: #888;
            font-size: 0.9rem;
            border-top: 1px solid #eee;
        }

        a {
            text-decoration: none;
            color: inherit;
        }
    </style>
</head>
<body>

    <header>
        <span class="mascot">🐼=😺</span>
        <h1>Panda is Cat</h1>
    </header>

    <div class="container">
        <!-- 简介区域 -->
        <section class="intro-card">
            <h2>🎉你好，欢迎来到我的Blog</h2>
            <p>这是一个托管在github，运行在 Cloudflare Pages 上的博客。</p>
            <p>在这个特殊的空间里，我们相信熊猫其实就是一种很胖的猫。</p>
        </section>

        <!-- 文章列表 -->
        <section>
            <h3 style="margin-bottom: 1.5rem;">📝 最新文章</h3>
            <ul class="post-list">
                <li class="post-item">
                    <a href="#">
                        <div class="post-date">2023年 10月 24日</div>
                        <h3 class="post-title">为什么熊猫喜欢吃竹子？</h3>
                        <p class="post-excerpt">这就像猫喜欢吃猫草一样，是一种谜一般的信仰...</p>
                    </a>
                </li>
                <li class="post-item">
                    <a href="#">
                        <div class="post-date">2023年 10月 20日</div>
                        <h3 class="post-title">Hello World</h3>
                        <p class="post-excerpt">这是我的第一篇博客，用于测试 Cloudflare 的部署。</p>
                    </a>
                </li>
            
            </ul>
        </section>
    </div>

    <footer>
        <p>&copy; 2026 Panda is Cat. Hosted on Cloudflare Pages.</p>
    </footer>

</body>
</html>
