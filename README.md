<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simone Tomasella - Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', -apple-system, BlinkMacSystemFont, sans-serif;
            line-height: 1.6;
            color: #e6edf3;
            background-color: #0d1117;
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        header {
            margin-bottom: 40px;
        }

        .greeting {
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 2.2em;
            font-weight: 600;
            margin-bottom: 30px;
            color: #f0f6fc;
        }

        .wave {
            font-size: 1.2em;
            animation: wave 2s ease-in-out infinite;
        }

        @keyframes wave {
            0%, 100% { transform: rotate(0deg); }
            25% { transform: rotate(20deg); }
            75% { transform: rotate(-10deg); }
        }

        .welcome {
            font-size: 1.4em;
            color: #8b949e;
            margin-bottom: 40px;
        }

        .section {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 8px;
            padding: 24px;
            margin-bottom: 24px;
        }

        .section h2 {
            color: #f0f6fc;
            font-size: 1.5em;
            margin-bottom: 20px;
            font-weight: 600;
        }

        .tech-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            align-items: center;
        }

        .tech-icon {
            width: 48px;
            height: 48px;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 14px;
            color: white;
            transition: transform 0.2s ease;
        }

        .tech-icon:hover {
            transform: scale(1.1);
        }

        /* Language icons */
        .c { background: #00599c; }
        .cpp { background: #00599c; }
        .java { background: #ed8b00; }
        .python { background: #3776ab; }
        .html { background: #e34c26; }
        .css { background: #1572b6; }
        .js { background: #f7df1e; color: #000; }

        /* Framework/Tool icons */
        .vscode { background: #0078d4; }
        .visual-studio { background: #5c2d91; }
        .docker { background: #2496ed; }
        .vue { background: #4fc08d; }
        .raspberry { background: #c51a4a; }
        .arduino { background: #00979d; }

        .fun-facts {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 8px;
            padding: 24px;
        }

        .fun-facts h2 {
            color: #f0f6fc;
            font-size: 1.5em;
            margin-bottom: 20px;
            font-weight: 600;
        }

        .fun-facts ul {
            list-style: none;
            padding: 0;
        }

        .fun-facts li {
            color: #e6edf3;
            margin-bottom: 12px;
            padding-left: 20px;
            position: relative;
        }

        .fun-facts li:before {
            content: "•";
            color: #58a6ff;
            font-size: 1.2em;
            position: absolute;
            left: 0;
        }

        .fun-facts li:last-child {
            margin-bottom: 0;
        }

        .highlight {
            color: #ffa657;
        }

        .sparkle {
            color: #ffa657;
        }

        .social-links {
            display: flex;
            gap: 16px;
            margin-top: 30px;
            flex-wrap: wrap;
        }

        .social-link {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 8px 16px;
            background: #21262d;
            border: 1px solid #30363d;
            border-radius: 6px;
            color: #e6edf3;
            text-decoration: none;
            transition: all 0.2s ease;
            font-size: 14px;
        }

        .social-link:hover {
            background: #30363d;
            border-color: #58a6ff;
            color: #58a6ff;
        }

        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .project-card {
            background: #0d1117;
            border: 1px solid #30363d;
            border-radius: 8px;
            padding: 20px;
            transition: border-color 0.2s ease;
        }

        .project-card:hover {
            border-color: #58a6ff;
        }

        .project-card h3 {
            color: #58a6ff;
            margin-bottom: 12px;
            font-size: 1.2em;
        }

        .project-card p {
            color: #8b949e;
            margin-bottom: 16px;
            line-height: 1.5;
        }

        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
            margin-bottom: 16px;
        }

        .tech-tag {
            background: #21262d;
            color: #e6edf3;
            padding: 4px 8px;
            border-radius: 12px;
            font-size: 12px;
            border: 1px solid #30363d;
        }

        .project-links {
            display: flex;
            gap: 12px;
        }

        .project-link {
            color: #58a6ff;
            text-decoration: none;
            font-size: 14px;
            font-weight: 500;
        }

        .project-link:hover {
            text-decoration: underline;
        }

        @media (max-width: 768px) {
            .container {
                padding: 10px;
            }
            
            .greeting {
                font-size: 1.8em;
            }
            
            .welcome {
                font-size: 1.2em;
            }
            
            .tech-grid {
                justify-content: center;
            }
            
            .social-links {
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1 class="greeting">
                Hi there, I'm Simone Tomasella 
                <span class="wave">👋</span>
            </h1>
            <p class="welcome">Welcome to my GitHub page</p>
        </header>

        <div class="section">
            <h2>Programming languages</h2>
            <div class="tech-grid">
                <div class="tech-icon c">C</div>
                <div class="tech-icon cpp">C++</div>
                <div class="tech-icon java">Java</div>
                <div class="tech-icon python">Py</div>
                <div class="tech-icon html">HTML</div>
                <div class="tech-icon css">CSS</div>
                <div class="tech-icon js">JS</div>
            </div>
        </div>

        <div class="section">
            <h2>Softwares, Frameworks, and hardware</h2>
            <div class="tech-grid">
                <div class="tech-icon vscode">VS</div>
                <div class="tech-icon visual-studio">VS</div>
                <div class="tech-icon docker">🐳</div>
                <div class="tech-icon vue">Vue</div>
                <div class="tech-icon raspberry">🍓</div>
                <div class="tech-icon arduino">🤖</div>
            </div>
        </div>

        <div class="section">
            <h2>Featured Projects</h2>
            <div class="projects">
                <div class="project-card">
                    <h3>Web Application</h3>
                    <p>A modern web application built with Vue.js and responsive design principles.</p>
                    <div class="project-tech">
                        <span class="tech-tag">Vue.js</span>
                        <span class="tech-tag">JavaScript</span>
                        <span class="tech-tag">CSS</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">View Code</a>
                        <a href="#" class="project-link">Live Demo</a>
                    </div>
                </div>

                <div class="project-card">
                    <h3>Hardware Project</h3>
                    <p>IoT project using Raspberry Pi and Arduino for home automation.</p>
                    <div class="project-tech">
                        <span class="tech-tag">Python</span>
                        <span class="tech-tag">Raspberry Pi</span>
                        <span class="tech-tag">Arduino</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">View Code</a>
                        <a href="#" class="project-link">Documentation</a>
                    </div>
                </div>

                <div class="project-card">
                    <h3>Desktop Application</h3>
                    <p>Cross-platform desktop application developed in Java with modern UI.</p>
                    <div class="project-tech">
                        <span class="tech-tag">Java</span>
                        <span class="tech-tag">JavaFX</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">View Code</a>
                        <a href="#" class="project-link">Download</a>
                    </div>
                </div>
            </div>
        </div>

        <div class="fun-facts">
            <h2>Fun facts about me:</h2>
            <ul>
                <li>I focus too much on useless brackets of code, but I make them <span class="highlight">✨</span> pretty <span class="sparkle">✨</span></li>
                <li>I like studying how algorithms work (no, I wasn't bullied at school)</li>
                <li>CSS is sh**</li>
                <li>Math? What's math?</li>
            </ul>
        </div>

        <div class="social-links">
            <a href="https://github.com/SimoneTomasella" class="social-link">
                🐙 GitHub
            </a>
            <a href="https://linkedin.com/in/simone-tomasella" class="social-link">
                💼 LinkedIn
            </a>
            <a href="mailto:simone.tomasella@example.com" class="social-link">
                📧 Email
            </a>
        </div>
    </div>

    <script>
        // Add some interactive effects
        document.addEventListener('DOMContentLoaded', function() {
            // Animate tech icons on hover
            const techIcons = document.querySelectorAll('.tech-icon');
            techIcons.forEach(icon => {
                icon.addEventListener('mouseenter', function() {
                    this.style.transform = 'scale(1.1) rotate(5deg)';
                });
                
                icon.addEventListener('mouseleave', function() {
                    this.style.transform = 'scale(1) rotate(0deg)';
                });
            });

            // Animate project cards on scroll
            const cards = document.querySelectorAll('.project-card');
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });

            cards.forEach(card => {
                card.style.opacity = '0';
                card.style.transform = 'translateY(20px)';
                card.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
                observer.observe(card);
            });
        });
    </script>
</body>
</html>
