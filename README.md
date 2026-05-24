<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CCgogoMKT</title>
    <style>
        :root {
            --bg-color: #0d0f14;          /* 极简深邃纯黑底 */
            --container-bg: #161922;      /* 精致暗色卡片背景 */
            --text-main: #f3f4f6;          /* 主文字纯白 */
            --text-muted: #a5a9b8;         /* 次要信息灰紫 */
            --accent-primary: #dcd0ff;    /* 核心亮淡紫（完全替代原来的黄色文字） */
            --accent-secondary: #bdb2ff;  /* 柔和薰衣草紫（用于小装饰线和图标） */
            --border-color: #232838;       /* 微弱高级质感边框 */
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
            padding: 40px 20px;
        }

        .container {
            max-width: 650px;
            margin: 0 auto;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
            padding-bottom: 20px;
            border-bottom: 1px solid var(--border-color);
        }

        header h1 {
            font-size: 2.2rem;
            font-weight: 700;
            letter-spacing: -0.025em;
            background: linear-gradient(to right, var(--accent-primary), var(--accent-secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* 每一个大板块的标题：全面换成淡紫色 */
        .section-title {
            font-size: 1.25rem;
            color: var(--accent-primary);
            margin: 35px 0 15px 0;
            padding-left: 10px;
            border-left: 3px solid var(--accent-secondary);
            letter-spacing: 0.05em;
            font-weight: 600;
        }

        .grid {
            display: block;
        }

        .card {
            background-color: var(--container-bg);
            border: 1px solid var(--border-color);
            border-radius: 10px;
            padding: 18px 20px;
            margin-bottom: 12px;
            transition: all 0.25s ease;
            text-decoration: none;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        /* 鼠标悬停时，边框和霓虹阴影都呈现浪漫淡紫色 */
        .card:hover {
            transform: translateY(-2px);
            border-color: var(--accent-primary);
            box-shadow: 0 8px 24px rgba(189, 178, 255, 0.2); 
        }

        .card-title {
            font-size: 1.05rem;
            font-weight: 500;
            color: var(--text-main);
        }

        .card-icon {
            color: var(--accent-secondary);
            font-size: 1.1rem;
            opacity: 0.9;
        }

        footer {
            margin-top: 50px;
            padding-top: 25px;
            border-top: 1px solid var(--border-color);
        }

        .contact-box {
            background: linear-gradient(135deg, #161922 0%, #1e2230 100%);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            padding: 24px;
            text-align: center;
        }

        .contact-title {
            font-size: 1.15rem;
            color: var(--text-main);
            margin-bottom: 15px;
            font-weight: 600;
        }

        .contact-info {
            display: block;
            margin: 8px 0;
            font-size: 1rem;
            color: var(--text-muted);
        }

        /* Contact 里面的重点提示文字换成淡紫 */
        .contact-info strong {
            color: var(--accent-primary);
        }

        @media (max-width: 600px) {
            body {
                padding: 20px 15px;
            }
            header h1 {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>CCgogoMKT</h1>
        </header>

        <div class="section-title">品牌营销排期与服务报价</div>
        <div class="grid">
            <a href="服务排期表1.jpg" target="_blank" class="card">
                <div class="card-title">Camellia 品牌内容方向定位表</div>
                <div class="card-icon">🖼️</div>
            </a>
            <a href="服务排期表2.jpg" target="_blank" class="card">
                <div class="card-title">Camellia & Luxloop 月服务费明细表（初版）</div>
                <div class="card-icon">🖼️</div>
            </a>
            <a href="服务排期表3.jpg" target="_blank" class="card">
                <div class="card-title">Camellia & Luxloop 自创/博主/Meta 打包优惠价</div>
                <div class="card-icon">🖼️</div>
            </a>
        </div>

        <div class="section-title">MKT训练营</div>
        <div class="grid">
            <a href="品牌营销全案思维框架训练营.pdf" target="_blank" class="card">
                <div class="card-title">品牌营销全案思维框架训练营</div>
                <div class="card-icon">📄</div>
            </a>
            <a href="Meta Ads实战训练营.pdf" target="_blank" class="card">
                <div class="card-title">Meta Ads实战训练营</div>
                <div class="card-icon">📄</div>
            </a>
        </div>

        <div class="section-title">出海营销</div>
        <div class="grid">
            <a href="出海营销陪跑群.pdf" target="_blank" class="card">
                <div class="card-title">出海营销陪跑群</div>
                <div class="card-icon">📄</div>
            </a>
            <a href="出海营销增长咨询.pdf" target="_blank" class="card">
                <div class="card-title">出海营销增长咨询</div>
                <div class="card-icon">📄</div>
            </a>
        </div>

        <div class="section-title">MKT求职</div>
        <div class="grid">
            <a href="MKT1v1求职服务.png" target="_blank" class="card">
                <div class="card-title">MKT 1v1 求职服务</div>
                <div class="card-icon">🖼️</div>
            </a>
        </div>

        <footer>
            <div class="contact-box">
                <div class="contact-title">Contact Me</div>
                <div class="contact-info"><strong>WeChat:</strong> xieqiao172132</div>
                <div class="contact-info"><strong>Email:</strong> ccgogo2024@gmail.com</div>
            </div>
        </footer>
    </div>

</body>
</html>
