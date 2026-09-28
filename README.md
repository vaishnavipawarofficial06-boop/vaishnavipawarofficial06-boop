<!DOCTYPE html>
<html lang="mr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vaishnavi Pawar GitHub Banner</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="banner-container">
        <!-- डावीकडील लॅपटॉप आणि कोड विभाग -->
        <div class="laptop-section">
            <div class="laptop-mockup">
                <div class="screen">
                    <div class="editor-sidebar">
                        <span>📁 src</span>
                        <span class="active">📄 App.jsx</span>
                    </div>
                    <div class="code-area">
                        <span class="comment">// Dynamic Typing Code</span>
                        <p class="typing-code">const App = () => { return &lt;div className="min-h-screen"&gt; &lt;h1&gt;Dream • Build • Grow&lt;/h1&gt; &lt;/div&gt; };</p>
                    </div>
                </div>
            </div>
            <div class="coffee-cup">&lt;/&gt;</div>
        </div>

        <!-- मधला मुख्य नाव आणि घोषणा विभाग -->
        <div class="main-content">
            <h1 class="name">VAISHNAVI PAWAR<span class="cursor">|</span></h1>
            <p class="subtitle">&lt;/&gt; Frontend Developer | Full-Stack Web Development Enthusiast</p>
            
            <!-- build. learn. grow. ॲनिमेशन -->
            <div class="terminal-box">
                <span class="arrow">&gt;</span>
                <span class="animated-text">build . learn . grow !</span>
            </div>
        </div>

        <!-- उजवीकडील गिट कमिट आणि टेक स्टॅक -->
        <div class="right-section">
            <div class="terminal-git">
                <div class="dots"><span></span><span></span><span></span></div>
                <p class="git-command">$ git commit -m <span class="commit-text">"Better Code . Brighter Future"</span><span class="git-cursor">_</span></p>
            </div>
            
            <div class="skills-list">
                <ul>
                    <li>HTML</li>
                    <li>CSS</li>
                    <li>JavaScript</li>
                    <li class="glow">React</li>
                    <li>Node.js</li>
                    <li>MongoDB</li>
                </ul>
            </div>
        </div>

        <!-- पार्श्वभूमीवरील डिजिटल आणि बायनरी लहरी -->
        <div class="matrix-bg">01001000 01000101 01001100 01001100 01001111</div>
    </div>
</body>
</html>
:root {
    --bg-color: #03001e;
    --neon-pink: #ff007f;
    --neon-blue: #00f0ff;
    --neon-purple: #7b2cbf;
    --text-color: #ffffff;
}

body {
    margin: 0;
    padding: 0;
    background: var(--bg-color);
    font-family: 'Courier New', Courier, monospace;
    overflow: hidden;
    color: var(--text-color);
}

/* मुख्य बॅनर कंटेनर */
.banner-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 350px;
    background: radial-gradient(circle at center, #0b022b 0%, #030013 100%);
    position: relative;
    padding: 20px;
    box-sizing: border-box;
    border: 1px solid rgba(0, 240, 255, 0.2);
    overflow: hidden;
}

/* १. मुख्य नावाचे Glow व Pulsing ॲनिमेशन */
.name {
    font-size: 3.2rem;
    font-weight: bold;
    background: linear-gradient(45deg, var(--neon-blue), var(--neon-pink));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    text-shadow: 0 0 10px rgba(0, 240, 255, 0.6), 0 0 20px rgba(255, 0, 127, 0.6);
    animation: pulseGlow 3s infinite alternate;
}

@keyframes pulseGlow {
    0% { transform: scale(1); filter: drop-shadow(0 0 2px rgba(0,240,255,0.5)); }
    100% { transform: scale(1.02); filter: drop-shadow(0 0 15px rgba(255, 0, 127, 0.8)); }
}

/* २. ब्लिंकिंग कर्सर ॲनिमेशन */
.cursor, .git-cursor {
    color: var(--neon-pink);
    animation: blink 0.8s infinite;
}

@keyframes blink {
    50% { opacity: 0; }
}

/* ३. टर्मिनल बॉक्स (Build. Learn. Grow) ॲनिमेशन */
.terminal-box {
    margin-top: 20px;
    background: rgba(255, 255, 255, 0.05);
    border: 1px solid var(--neon-blue);
    padding: 10px 20px;
    border-radius: 5px;
    display: inline-block;
    box-shadow: 0 0 15px rgba(0, 240, 255, 0.2);
}

.animated-text {
    border-right: 2px solid var(--neon-pink);
    white-space: nowrap;
    overflow: hidden;
    display: inline-block;
    animation: typing 4s steps(25) infinite alternate;
}

@keyframes typing {
    0% { width: 0; }
    50%, 100% { width: 100%; }
}

/* ४. डिजिटल पार्श्वभूमी - मुव्हिंग लाईन्स (Background Network Effect) */
.banner-container::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 200%;
    height: 100%;
    background: linear-gradient(90deg, transparent 50%, rgba(0, 240, 255, 0.05) 50%);
    background-size: 40px 40px;
    animation: backgroundScroll 20s linear infinite;
    z-index: 1;
}

@keyframes backgroundScroll {
    0% { transform: translateX(0); }
    100% { transform: translateX(-50%); }
}

/* ५. बायनरी नंबर्स फॉलिंग इफेक्ट (Matrix Style) */
.matrix-bg {
    position: absolute;
    right: 20px;
    bottom: 10px;
    font-size: 0.8rem;
    color: rgba(0, 240, 255, 0.25);
    writing-mode: vertical-rl;
    text-orientation: monospace;
    animation: matrixFall 10s linear infinite;
    z-index: 0;
}

@keyframes matrixFall {
    0% { transform: translateY(-100%); }
    100% { transform: translateY(100%); }
}

/* ६. डावीकडील चहाचा/कॉफीचा कप 'ग्लॉइंग' */
.coffee-cup {
    font-size: 1.5rem;
    color: var(--neon-blue);
    text-shadow: 0 0 5px var(--neon-blue);
    animation: heatVapour 2s infinite ease-in-out;
}

@keyframes heatVapour {
    0%, 100% { transform: translateY(0); opacity: 0.8; }
    50% { transform: translateY(-5px); opacity: 1; filter: blur(0.5px); }
}


# Hi 👋, I'm Vaishnavi Pawar

### 💻 Frontend Developer | Full-Stack Web Development Enthusiast

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=vaishnavipawarofficial06-boop&label=Profile%20Views&color=0e75b6&style=flat" />
</p>

<p align="center">
  <a href="https://github.com/vaishnavipawarofficial06-boop">
    <img src="https://img.shields.io/github/followers/vaishnavipawarofficial06-boop?label=Followers&style=for-the-badge" />
  </a>
  <a href="https://github.com/vaishnavipawarofficial06-boop">
    <img src="https://img.shields.io/github/stars/vaishnavipawarofficial06-boop?label=Stars&style=for-the-badge" />
  </a>
</p>

---

## 👩‍💻 About Me

I'm a passionate **Frontend Developer** interested in building modern, responsive,
and user-friendly web applications.

- 💻 I'm a **Frontend Developer**
- 🌐 I'm interested in **Full-Stack Web Development**
- 🌱 Currently learning **Python, Cloud Technologies & Web Development**
- 📚 Currently working on improving my **programming languages and technical skills**
- 💡 Interested in building **real-world web applications**
- 👯 Looking to collaborate on **Web Development & Open Source projects**
- 💬 Ask me about **HTML, CSS, JavaScript, Python, Git & GitHub**
- 📫 Reach me at **vaishnavipawarofficial06@gmail.com**
- ⚡ Fun fact: **I love turning ideas into working projects!**

---

## 🛠️ Tech Stack

### 🌐 Frontend Development

<p>
<img src="https://skillicons.dev/icons?i=html,css,javascript" />
</p>

### 🐍 Programming Languages

<p>
<img src="https://skillicons.dev/icons?i=python,java,cpp,c" />
</p>

### ☁️ Cloud & Technologies

<p>
<img src="https://skillicons.dev/icons?i=aws,azure,gcp" />
</p>

### 🗄️ Databases

<p>
<img src="https://skillicons.dev/icons?i=mysql,mongodb,sqlite" />
</p>

### 🔧 Tools

<p>
<img src="https://skillicons.dev/icons?i=git,github,vscode,linux" />
</p>

---

## 🌱 Currently Learning

```text
Frontend Development
        ↓
Full-Stack Web Development
        ↓
Python
        ↓
Cloud Technologies
        ↓
Backend Development
