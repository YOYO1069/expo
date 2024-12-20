id: magic-spring-party-registration-v13
name: 春尚CHiLL尾牙報名系統 - 預覽版
type: html
content: |-
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>春尚CHiLL尾牙 - 魔法報名系統 ✨</title>
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600&family=Noto+Sans+TC:wght@300;400;500;700&display=swap" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
    <style>
        :root {
            --glass-bg: rgba(255, 255, 255, 0.1);
            --glass-border: rgba(255, 255, 255, 0.2);
            --primary-color: #7000FF;
            --secondary-color: #FF3D9A;
            --accent-color: #00E1FF;
            --text-color: #FFFFFF;
        }

        body {
            margin: 0;
            padding: 0;
            min-height: 100vh;
            font-family: 'Noto Sans TC', sans-serif;
            background: linear-gradient(135deg, #1a0033, #4a0080);
            color: var(--text-color);
            overflow-x: hidden;
            position: relative;
        }

        /* 模擬預覽效果的樣式 */
        .preview-container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 20px;
        }

        .preview-step {
            background: rgba(0, 0, 0, 0.3);
            border-radius: 15px;
            padding: 20px;
            margin-bottom: 30px;
            backdrop-filter: blur(10px);
            border: 1px solid var(--glass-border);
            position: relative;
            overflow: hidden;
        }

        .preview-step::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg,
                rgba(112, 0, 255, 0.1),
                rgba(255, 61, 154, 0.1)
            );
            pointer-events: none;
        }

        .step-header {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 1px solid var(--glass-border);
        }

        .step-number {
            width: 40px;
            height: 40px;
            background: var(--primary-color);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            margin-right: 15px;
            box-shadow: 0 0 20px rgba(112, 0, 255, 0.3);
        }

        .step-title {
            font-size: 1.5em;
            margin: 0;
            background: linear-gradient(45deg,
                var(--primary-color),
                var(--secondary-color)
            );
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .preview-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            padding: 20px;
        }

        .preview-card {
            background: var(--glass-bg);
            border: 1px solid var(--glass-border);
            border-radius: 12px;
            padding: 20px;
            transition: transform 0.3s ease;
        }

        .preview-card:hover {
            transform: translateY(-5px);
        }

        .preview-image {
            width: 100%;
            height: 200px;
            background: var(--glass-bg);
            border-radius: 8px;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2em;
        }

        .preview-description {
            color: rgba(255, 255, 255, 0.8);
            line-height: 1.6;
        }

        .preview-features {
            list-style: none;
            padding: 0;
            margin: 15px 0;
        }

        .preview-features li {
            padding: 8px 0;
            padding-left: 25px;
            position: relative;
        }

        .preview-features li::before {
            content: '✨';
            position: absolute;
            left: 0;
            top: 8px;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .floating {
            animation: float 3s ease-in-out infinite;
        }
    </style>
</head>
<body>
    <div id="particles-js"></div>

    <div class="preview-container">
        <div class="preview-step">
            <div class="step-header">
                <div class="step-number">1</div>
                <h2 class="step-title">報名入學 - 選擇魔法團隊</h2>
            </div>
            <div class="preview-content">
                <div class="preview-card">
                    <div class="preview-image floating">🧙‍♂️</div>
                    <h3>選擇團隊規模</h3>
                    <ul class="preview-features">
                        <li>雙人魔法組合</li>
                        <li>魔法六人眾</li>
                        <li>自訂魔法團</li>
                    </ul>
                </div>
                <div class="preview-card">
                    <div class="preview-description">
                        在這個步驟中，您可以：
                        <ul class="preview-features">
                            <li>選擇預設的團隊人數</li>
                            <li>自訂2-10人的魔法團</li>
                            <li>享受互動式選擇體驗</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div class="preview-step">
            <div class="step-header">
                <div class="step-number">2</div>
                <h2 class="step-title">選召隊友 - 召喚魔法夥伴</h2>
            </div>
            <div class="preview-content">
                <div class="preview-card">
                    <div class="preview-image floating">✨</div>
                    <h3>輸入隊友資料</h3>
                    <ul class="preview-features">
                        <li>動態生成輸入欄位</li>
                        <li>即時驗證資料</li>
                        <li>魔法動畫效果</li>
                    </ul>
                </div>
                <div class="preview-card">
                    <div class="preview-description">
                        在這個步驟中，您將：
                        <ul class="preview-features">
                            <li>輸入每位隊友的名稱</li>
                            <li>享受順暢的表單體驗</li>
                            <li>觀賞魔法特效</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div class="preview-step">
            <div class="step-header">
                <div class="step-number">3</div>
                <h2 class="step-title">穿魔法裝備 - 選擇造型風格</h2>
            </div>
            <div class="preview-content">
                <div class="preview-card">
                    <div class="preview-image floating">🎭</div>
                    <h3>選擇裝備風格</h3>
                    <ul class="preview-features">
                        <li>魔法學院風格</li>
                        <li>星光魔法元素</li>
                        <li>自由創作風格</li>
                    </ul>
                </div>
                <div class="preview-card">
                    <div class="preview-description">
                        在這個步驟中，您可以：
                        <ul class="preview-features">
                            <li>挑選喜愛的造型風格</li>
                            <li>預覽視覺效果</li>
                            <li>體驗互動選擇</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div class="preview-step">
            <div class="step-header">
                <div class="step-number">4</div>
                <h2 class="step-title">確認入學 - 完成報名程序</h2>
            </div>
            <div class="preview-content">
                <div class="preview-card">
                    <div class="preview-image floating">📜</div>
                    <h3>確認報名資訊</h3>
                    <ul class="preview-features">
                        <li>檢視團隊資訊</li>
                        <li>確認隊友名單</li>
                        <li>提交報名表</li>
                    </ul>
                </div>
                <div class="preview-card">
                    <div class="preview-description">
                        最後一個步驟，您將：
                        <ul class="preview-features">
                            <li>確認所有填寫資料</li>
                            <li>享受提交動畫</li>
                            <li>收到確認通知</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // 初始化粒子效果
        particlesJS('particles-js', {
            particles: {
                number: {
                    value: 80,
                    density: {
                        enable: true,
                        value_area: 800
                    }
                },
                color: {
                    value: ['#7000FF', '#FF3D9A', '#00E1FF']
                },
                shape: {
                    type: 'circle'
                },
                opacity: {
                    value: 0.5,
                    random: true
                },
                size: {
                    value: 3,
                    random: true
                },
                move: {
                    enable: true,
                    speed: 2,
                    direction: 'none',
                    random: true,
                    out_mode: 'out'
                }
            }
        });
    </script>
</body>
</html>
