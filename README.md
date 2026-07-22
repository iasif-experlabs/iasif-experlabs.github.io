<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Saim Asif | AI Fullstack Engineer</title>
    <meta name="description" content="Saim Asif - Architecting intelligent systems. Full Stack Engineer specializing in Next.js, Node, and High-Performance AI Integrations.">
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Outfit:wght@400;600;700;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #030712; /* Very dark slate */
            --surface-color: rgba(17, 24, 39, 0.7); /* Translucent */
            --surface-hover: rgba(31, 41, 55, 0.9);
            --border-color: rgba(255, 255, 255, 0.1);
            --primary-color: #3b82f6; /* Blue */
            --primary-hover: #2563eb;
            --text-main: #f9fafb;
            --text-muted: #9ca3af;
            --font-heading: 'Outfit', sans-serif;
            --font-body: 'Inter', sans-serif;
            --glass-blur: 12px;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            font-family: var(--font-body);
            line-height: 1.6;
            overflow-x: hidden;
            /* Subtle radial gradients for premium feel */
            background-image: radial-gradient(circle at 15% 50%, rgba(59, 130, 246, 0.08), transparent 25%),
                              radial-gradient(circle at 85% 30%, rgba(139, 92, 246, 0.08), transparent 25%);
            background-attachment: fixed;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 0 20px;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: var(--font-heading);
            font-weight: 700;
            line-height: 1.2;
        }

        a {
            color: inherit;
            text-decoration: none;
        }

        ul {
            list-style: none;
        }

        /* Utilities */
        .mb-2 { margin-bottom: 0.5rem; }
        .mb-4 { margin-bottom: 1rem; }
        .mb-5 { margin-bottom: 2rem; }
        .mt-2 { margin-top: 0.5rem; }
        .mt-4 { margin-top: 1rem; }
        .mt-5 { margin-top: 2rem; }
        .text-center { text-align: center; }
        .w-100 { width: 100%; }

        .section-padding {
            padding: 100px 0;
        }

        .gradient-text {
            background: linear-gradient(135deg, #60a5fa, #a78bfa);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .glass {
            background: var(--surface-color);
            backdrop-filter: blur(var(--glass-blur));
            -webkit-backdrop-filter: blur(var(--glass-blur));
            border-bottom: 1px solid var(--border-color);
        }

        .badge {
            display: inline-block;
            padding: 6px 14px;
            border-radius: 20px;
            background: rgba(59, 130, 246, 0.1);
            border: 1px solid rgba(59, 130, 246, 0.3);
            color: #60a5fa;
            font-size: 0.85rem;
            font-weight: 500;
            letter-spacing: 0.5px;
            text-transform: uppercase;
            margin-bottom: 1rem;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 12px 24px;
            border-radius: 8px;
            font-weight: 600;
            font-family: var(--font-body);
            transition: all 0.3s ease;
            cursor: pointer;
            border: none;
        }

        .btn-sm {
            padding: 8px 16px;
            font-size: 0.9rem;
        }

        .btn-primary {
            background: var(--primary-color);
            color: white;
            box-shadow: 0 4px 14px rgba(59, 130, 246, 0.3);
        }

        .btn-primary:hover {
            background: var(--primary-hover);
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(59, 130, 246, 0.4);
        }

        .btn-secondary {
            background: rgba(255, 255, 255, 0.05);
            color: var(--text-main);
            border: 1px solid var(--border-color);
        }

        .btn-secondary:hover {
            background: rgba(255, 255, 255, 0.1);
            transform: translateY(-2px);
        }

        /* Animations */
        .fade-in-up {
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
        }

        .fade-in-up.appear {
            opacity: 1;
            transform: translateY(0);
        }

        /* Navbar */
        .navbar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            padding: 15px 0;
        }

        .nav-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: var(--font-heading);
            font-size: 1.5rem;
            font-weight: 800;
            letter-spacing: -1px;
            background: linear-gradient(135deg, #fff, #9ca3af);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .nav-links {
            display: flex;
            gap: 30px;
        }

        .nav-links a {
            font-size: 0.9rem;
            color: var(--text-muted);
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: var(--text-main);
        }

        /* Hero */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding-top: 80px;
        }

        .hero-content {
            max-width: 800px;
        }

        .hero-title {
            font-size: 5.5rem;
            letter-spacing: -2px;
            margin: 10px 0 5px;
            background: linear-gradient(180deg, #fff, #9ca3af);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero-subtitle {
            font-size: 2.5rem;
            color: var(--text-muted);
            margin-bottom: 25px;
            font-weight: 400;
        }

        .hero-desc {
            font-size: 1.25rem;
            color: var(--text-muted);
            max-width: 600px;
            margin-bottom: 40px;
        }

        .hero-actions {
            display: flex;
            gap: 15px;
        }

        /* Impact Section */
        .section-heading {
            font-size: 2.5rem;
            margin-bottom: 10px;
            letter-spacing: -1px;
        }

        .section-subheading {
            color: var(--text-muted);
            font-size: 1.1rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-weight: 600;
        }

        .impact-desc {
            max-width: 700px;
            margin: 20px auto 50px;
            color: var(--text-muted);
            font-size: 1.1rem;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
        }

        .stat-card {
            background: var(--surface-color);
            border: 1px solid var(--border-color);
            border-radius: 16px;
            padding: 30px;
            text-align: center;
            transition: transform 0.3s ease, border-color 0.3s ease;
        }

        .stat-card:hover {
            transform: translateY(-5px);
            border-color: rgba(59, 130, 246, 0.4);
        }

        .stat-value {
            font-size: 3.5rem;
            font-family: var(--font-heading);
            font-weight: 700;
            margin-bottom: 5px;
            background: linear-gradient(135deg, #ffffff, #60a5fa);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .stat-label {
            font-size: 1.1rem;
            font-weight: 600;
            color: var(--text-main);
            margin-bottom: 15px;
        }

        .stat-detail {
            font-size: 0.95rem;
            color: var(--text-muted);
        }

        /* About Section */
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: start;
        }

        .about-text p {
            color: var(--text-muted);
            font-size: 1.1rem;
            line-height: 1.8;
        }

        .about-mini-stats {
            display: flex;
            gap: 30px;
            font-size: 1.1rem;
        }

        /* Timeline */
        .timeline-item {
            position: relative;
            padding-left: 30px;
            margin-bottom: 40px;
            border-left: 1px solid rgba(255, 255, 255, 0.1);
        }

        .timeline-item:last-child {
            margin-bottom: 0;
        }

        .timeline-dot {
            position: absolute;
            left: -6px;
            top: 5px;
            width: 11px;
            height: 11px;
            background: var(--primary-color);
            border-radius: 50%;
            box-shadow: 0 0 10px rgba(59, 130, 246, 0.6);
        }

        .timeline-item h4 {
            font-size: 1.25rem;
            color: var(--text-main);
            margin-bottom: 5px;
        }

        .timeline-meta {
            font-size: 0.85rem;
            color: #60a5fa;
            margin-bottom: 15px;
            font-weight: 500;
        }

        .timeline-item ul {
            list-style: disc;
            padding-left: 20px;
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        .timeline-item li {
            margin-bottom: 8px;
        }

        /* Skills */
        .skills-flex {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            justify-content: center;
            max-width: 900px;
            margin: 0 auto;
        }

        .skill-tag {
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid var(--border-color);
            padding: 10px 18px;
            border-radius: 8px;
            font-size: 0.95rem;
            color: var(--text-muted);
            transition: all 0.3s ease;
            cursor: default;
        }

        .skill-tag:hover {
            background: rgba(255, 255, 255, 0.1);
            color: var(--text-main);
            border-color: rgba(255, 255, 255, 0.3);
            transform: translateY(-2px);
        }

        /* Projects */
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));
            gap: 30px;
        }

        .project-card {
            background: var(--surface-color);
            border: 1px solid var(--border-color);
            border-radius: 16px;
            overflow: hidden;
            transition: transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            display: flex;
            flex-direction: column;
        }

        .project-card:hover {
            transform: translateY(-8px);
            border-color: rgba(59, 130, 246, 0.3);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }

        .project-content {
            padding: 30px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }

        .project-highlight {
            font-size: 0.8rem;
            color: #60a5fa;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-weight: 600;
        }

        .project-title {
            font-size: 1.4rem;
            margin-bottom: 10px;
        }

        .project-desc {
            color: var(--text-muted);
            font-size: 0.95rem;
            margin-bottom: 20px;
            flex-grow: 1;
        }

        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .project-tech span {
            background: rgba(0, 0, 0, 0.3);
            color: #9ca3af;
            font-size: 0.75rem;
            padding: 4px 10px;
            border-radius: 4px;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }

        /* Contact */
        .contact-wrapper {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            background: var(--surface-color);
            border: 1px solid var(--border-color);
            border-radius: 20px;
            padding: 60px;
        }

        .contact-info p {
            color: var(--text-muted);
            font-size: 1.1rem;
            margin-top: 15px;
        }

        .contact-form .form-group {
            margin-bottom: 20px;
        }

        .contact-form label {
            display: block;
            margin-bottom: 8px;
            font-size: 0.9rem;
            font-weight: 500;
        }

        .contact-form input,
        .contact-form textarea {
            width: 100%;
            background: rgba(0, 0, 0, 0.2);
            border: 1px solid var(--border-color);
            padding: 12px 15px;
            border-radius: 8px;
            color: white;
            font-family: var(--font-body);
            font-size: 1rem;
            transition: border-color 0.3s ease;
        }

        .contact-form input:focus,
        .contact-form textarea:focus {
            outline: none;
            border-color: var(--primary-color);
        }

        /* CTA */
        .cta-links {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;
        }

        .cta-link {
            font-size: 1.2rem;
            color: var(--text-muted);
            transition: color 0.3s ease;
            border-bottom: 1px solid transparent;
        }

        .cta-link:hover {
            color: var(--primary-color);
            border-bottom: 1px solid var(--primary-color);
        }

        /* Footer */
        .footer {
            border-top: 1px solid var(--border-color);
            padding: 30px 0;
            margin-top: 50px;
        }

        .flex-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        /* Responsive */
        @media (max-width: 900px) {
            .about-grid, .contact-wrapper {
                grid-template-columns: 1fr;
                gap: 40px;
            }
            
            .contact-wrapper {
                padding: 40px 20px;
            }
            
            .hero-title {
                font-size: 4rem;
            }
            
            .hero-subtitle {
                font-size: 2rem;
            }
        }

        @media (max-width: 600px) {
            .nav-links {
                display: none;
            }
            
            .hero-title {
                font-size: 3rem;
            }
            
            .hero-subtitle {
                font-size: 1.5rem;
            }
            
            .stats-grid {
                grid-template-columns: 1fr;
            }
            
            .flex-footer {
                flex-direction: column;
                text-align: center;
                gap: 15px;
            }
        }
    </style>
</head>
<body>
    <nav class="navbar glass">
        <div class="nav-content container">
            <a href="#" class="logo">SA</a>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <a href="#contact" class="btn btn-primary btn-sm">Let's Talk</a>
        </div>
    </nav>

    <main>
        <!-- Hero -->
        <section id="home" class="hero section-padding">
            <div class="container hero-content fade-in-up">
                <div class="badge">Available for highly impactful roles</div>
                <h1 class="hero-title">Saim Asif.</h1>
                <h2 class="hero-subtitle">Architecting intelligent systems.</h2>
                <p class="hero-desc">Full Stack Engineer specializing in Next.js, Node, and High-Performance AI Integrations.</p>
                <div class="hero-actions">
                    <a href="#projects" class="btn btn-primary">View Projects</a>
                    <a href="#contact" class="btn btn-secondary">Contact Me</a>
                </div>
            </div>
        </section>

        <!-- Impact -->
        <section class="impact section-padding">
            <div class="container">
                <h3 class="section-heading text-center fade-in-up">Impact at a Glance</h3>
                <p class="section-subheading text-center fade-in-up mb-5">Building at Scale</p>
                
                <div class="stats-grid">
                    <div class="stat-card fade-in-up">
                        <div class="stat-value">7+</div>
                        <div class="stat-label">Years Experience</div>
                        <div class="stat-detail">Building scalable enterprise SaaS platforms, complex Warehouse Management Systems, and high-traffic mobile applications from scratch.</div>
                    </div>
                    <div class="stat-card fade-in-up" style="transition-delay: 100ms;">
                        <div class="stat-value">70+</div>
                        <div class="stat-label">B2B Clients</div>
                        <div class="stat-detail">Successfully onboarded 70+ active high-paying B2B clients within the first quarter of launching the Case Management Hub SaaS platform.</div>
                    </div>
                    <div class="stat-card fade-in-up" style="transition-delay: 200ms;">
                        <div class="stat-value">4M+</div>
                        <div class="stat-label">Active Users</div>
                        <div class="stat-detail">Scaled the Seated restaurant reservation application to support 4 million concurrent active users globally.</div>
                    </div>
                    <div class="stat-card fade-in-up" style="transition-delay: 300ms;">
                        <div class="stat-value">HIPAA</div>
                        <div class="stat-label">Compliant Systems</div>
                        <div class="stat-detail">Architected secure, HIPAA-compliant enterprise infrastructure with end-to-end data encryption and granular role-based access control.</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- About -->
        <section id="about" class="about section-padding">
            <div class="container">
                <div class="about-grid">
                    <div class="about-text fade-in-up">
                        <div class="badge mb-2">About Me</div>
                        <h2 class="section-heading">Crafting the Future with<br><span class="gradient-text">AI & Full Stack</span></h2>
                        <p class="mt-4">Full Stack AI Engineer & Technical Team Lead with over 7 years of experience building scalable enterprise SaaS platforms, complex Warehouse Management Systems (WMS), and high-traffic mobile applications from scratch. Specialized in Next.js, NestJS, and modern backend architectures with hybrid database systems (MySQL + MongoDB), along with deep expertise in native Android (Kotlin/Java) hardware integrations and cross-platform ecosystems.</p>
                        
                        <div class="about-mini-stats mt-4">
                            <div><strong class="gradient-text">7+</strong> Years Experience</div>
                            <div><strong class="gradient-text">70+</strong> B2B Clients</div>
                        </div>
                    </div>
                    
                    <div class="experience-timeline fade-in-up">
                        <h3 class="mb-4">Professional Experience</h3>
                        
                        <div class="timeline-item">
                            <div class="timeline-dot"></div>
                            <h4>Senior Full Stack & AI Engineer</h4>
                            <div class="timeline-meta">Airiodion Group | Oct 2024 – Jun 2026 | USA / Remote</div>
                            <ul>
                                <li>Architected and led the full-stack development of a highly scalable, multi-tenant enterprise SaaS platform from scratch.</li>
                                <li>Engineered a secure backend infrastructure using NestJS and a hybrid database model (MySQL + MongoDB) to ensure strict data isolation and rapid query performance.</li>
                                <li>Implemented rigorous HIPAA compliance protocols, end-to-end data encryption, and granular role-based access control (RBAC).</li>
                                <li>Managed the complete product lifecycle from concept to production, successfully onboarding 70+ active high-paying clients between January and March alone.</li>
                                <li>Designed production-grade RESTful APIs to decouple systems and maximize processing speed across frontend and backend services.</li>
                                <li>Directed engineering workflows across distributed teams, standardizing code quality, performance optimizations, and continuous deployment pipelines.</li>
                            </ul>
                        </div>

                        <div class="timeline-item">
                            <div class="timeline-dot"></div>
                            <h4>Senior Software Engineer</h4>
                            <div class="timeline-meta">FORTNA | Mar 2022 – Sep 2024 | USA / Remote</div>
                            <ul>
                                <li>Developed and optimized enterprise-level applications tailored for complex warehouse operations, production logistics, and automated inventory flows.</li>
                                <li>Built out core features for heavy-duty Warehouse Management Systems (WMS), handling high-volume real-time data synchronization.</li>
                                <li>Engineered native Android solutions optimized for rugged warehouse environments, integrating physical Zebra enterprise hardware and PAX A920 smart payment terminals.</li>
                                <li>Focused extensively on low-latency multithreading, robust background processing, and Firebase-backed real-time messaging to ensure zero downtime on the floor.</li>
                            </ul>
                        </div>
                        
                        <div class="timeline-item">
                            <div class="timeline-dot"></div>
                            <h4>Android Engineer</h4>
                            <div class="timeline-meta">Connectavo | Mar 2019 – Jan 2022 | Germany / Remote</div>
                            <ul>
                                <li>Built and maintained the core native Android application for an industrial IoT plant-management platform, directly contributing to a successful platform acquisition by the German corporate giant WAFIOS.</li>
                                <li>Engineered features to maintain and monitor heavy gear machines and industrial equipment across automated factory floors.</li>
                                <li>Collaborated directly with backend infrastructure leads to rebuild API interaction contracts, driving a 90% improvement in cross-team development velocity.</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Skills -->
        <section class="skills section-padding">
            <div class="container fade-in-up">
                <h3 class="section-heading text-center">Technical Arsenal</h3>
                <div class="skills-flex mt-4">
                    <span class="skill-tag">Local LLM Deployment</span>
                    <span class="skill-tag">Ollama</span>
                    <span class="skill-tag">Qwen</span>
                    <span class="skill-tag">DeepSeek</span>
                    <span class="skill-tag">n8n Orchestration</span>
                    <span class="skill-tag">OpenAI API</span>
                    <span class="skill-tag">Prompt Engineering</span>
                    <span class="skill-tag">Autonomous Data Pipelines</span>
                    <span class="skill-tag">Next.js</span>
                    <span class="skill-tag">React</span>
                    <span class="skill-tag">TypeScript</span>
                    <span class="skill-tag">JavaScript</span>
                    <span class="skill-tag">Redux</span>
                    <span class="skill-tag">Tailwind CSS</span>
                    <span class="skill-tag">Android SDK</span>
                    <span class="skill-tag">Kotlin/Java</span>
                    <span class="skill-tag">React Native</span>
                    <span class="skill-tag">Node.js</span>
                    <span class="skill-tag">NestJS</span>
                    <span class="skill-tag">Python</span>
                    <span class="skill-tag">FastAPI</span>
                    <span class="skill-tag">REST APIs</span>
                    <span class="skill-tag">Microservices Architecture</span>
                    <span class="skill-tag">MySQL</span>
                    <span class="skill-tag">MongoDB</span>
                    <span class="skill-tag">PostgreSQL</span>
                    <span class="skill-tag">Firebase Realtime DB</span>
                    <span class="skill-tag">SaaS</span>
                    <span class="skill-tag">Multi-Tenancy</span>
                    <span class="skill-tag">HIPAA Compliance</span>
                    <span class="skill-tag">Docker</span>
                    <span class="skill-tag">CI/CD</span>
                    <span class="skill-tag">Zebra Hardware Integration</span>
                    <span class="skill-tag">Git</span>
                </div>
            </div>
        </section>

        <!-- Projects -->
        <section id="projects" class="projects section-padding">
            <div class="container">
                <div class="badge fade-in-up mb-2">Work & Architecture</div>
                <h2 class="section-heading fade-in-up">Featured Projects</h2>
                <p class="section-subheading fade-in-up mb-5">A selection of enterprise-grade applications, AI pipelines, and scalable systems I have architected and delivered.</p>

                <div class="project-grid mt-5">
                    <!-- Project 1 -->
                    <div class="project-card fade-in-up">
                        <div class="project-content">
                            <div class="project-highlight mb-2">70+ Active B2B Clients in Q1</div>
                            <h3 class="project-title">Case Management Hub (SaaS Platform)</h3>
                            <p class="project-desc mt-2">Architected and led the full-stack development of a highly scalable, multi-tenant enterprise SaaS platform from scratch. Engineered secure backend infrastructure using NestJS with a hybrid database model (MySQL + MongoDB) for strict data isolation. Implemented rigorous HIPAA compliance protocols, end-to-end data encryption, and granular RBAC. Successfully onboarded 70+ active high-paying B2B clients within the first quarter.</p>
                            <div class="project-tech mt-4">
                                <span>Next.js</span><span>NestJS</span><span>MySQL</span><span>MongoDB</span><span>HIPAA</span><span>RBAC</span><span>SaaS</span>
                            </div>
                        </div>
                    </div>

                    <!-- Project 2 -->
                    <div class="project-card fade-in-up">
                        <div class="project-content">
                            <div class="project-highlight mb-2">Cost & Latency Optimized</div>
                            <h3 class="project-title">Autonomous AI Job-Scraping & Data Pipeline</h3>
                            <p class="project-desc mt-2">Architected an automated n8n data harvesting pipeline, initially built with a 5-node OpenAI (GPT-5 Mini) architecture. Optimized API costs and latency by migrating to local LLM infrastructure running qwen3.6:35b via Ollama on an M4 Pro (48GB RAM). Engineered a secure, low-latency reverse tunnel using bore.pub to expose the local model endpoint directly to the cloud n8n instance. The pipeline autonomously aggregates, parses, and matures multi-source unstructured web streams into high-fidelity structured datasets.</p>
                            <div class="project-tech mt-4">
                                <span>n8n</span><span>Ollama</span><span>Qwen</span><span>OpenAI</span><span>Reverse Tunneling</span><span>Python</span>
                            </div>
                        </div>
                    </div>

                    <!-- Project 3 -->
                    <div class="project-card fade-in-up">
                        <div class="project-content">
                            <div class="project-highlight mb-2">Zero Downtime on Floor</div>
                            <h3 class="project-title">PackTrack (Enterprise Scanner Solution)</h3>
                            <p class="project-desc mt-2">Developed a specialized Android WMS application tailored for rugged enterprise Zebra hardware and PAX A920 smart payment terminals. Optimized barcode decoding, secure ledger tracking, and supply chain logistics throughput. Focused on low-latency multithreading, robust background processing, and Firebase-backed real-time messaging to ensure zero downtime in warehouse environments.</p>
                            <div class="project-tech mt-4">
                                <span>Kotlin</span><span>Java</span><span>Zebra SDK</span><span>PAX A920</span><span>Firebase</span><span>WMS</span>
                            </div>
                        </div>
                    </div>

                    <!-- Project 4 -->
                    <div class="project-card fade-in-up">
                        <div class="project-content">
                            <div class="project-highlight mb-2">Scaled to 4M Active Users</div>
                            <h3 class="project-title">Seated</h3>
                            <p class="project-desc mt-2">Built, scaled, and maintained the core native Android application for a high-traffic restaurant reservation platform. Successfully refactored and converted the application from React Native to native Android, scaling system capability to support 4 million active users. Collaborated with backend leads to rebuild API interaction contracts, driving a 90% improvement in cross-team development velocity.</p>
                            <div class="project-tech mt-4">
                                <span>Native Android</span><span>React Native</span><span>High Concurrency</span><span>API Contracts</span>
                            </div>
                        </div>
                    </div>

                    <!-- Project 5 -->
                    <div class="project-card fade-in-up">
                        <div class="project-content">
                            <div class="project-highlight mb-2">Acquired by WAFIOS</div>
                            <h3 class="project-title">Connectavo</h3>
                            <p class="project-desc mt-2">Developed an industrial maintenance application incorporating advanced predictive analytics and real-time asset monitoring for automated factory environments. Directly contributed to a successful platform acquisition by the German corporate giant WAFIOS. Rebuilt API interaction contracts to drive significant improvements in development velocity.</p>
                            <div class="project-tech mt-4">
                                <span>Android</span><span>IoT</span><span>Predictive Analytics</span><span>Real-time DB</span><span>WAFIOS</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact -->
        <section id="contact" class="contact section-padding">
            <div class="container fade-in-up">
                <div class="contact-wrapper">
                    <div class="contact-info">
                        <h2 class="section-heading mb-2">Get In Touch</h2>
                        <p>Interested in collaborating or have a project in mind? Feel free to reach out. I'm currently open to new opportunities and interesting challenges.</p>
                    </div>
                    <form class="contact-form" onsubmit="event.preventDefault(); alert('Message feature coming soon!');">
                        <div class="form-group">
                            <label for="name">Name</label>
                            <input type="text" id="name" placeholder="Your name" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" id="email" placeholder="your@email.com" required>
                        </div>
                        <div class="form-group">
                            <label for="message">Message</label>
                            <textarea id="message" rows="5" placeholder="How can I help you?" required></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary w-100">Send Message</button>
                    </form>
                </div>
            </div>
        </section>
        
        <!-- CTA Section -->
        <section class="cta section-padding">
            <div class="container text-center fade-in-up">
                <h2 class="section-heading mb-4">Let's Talk.</h2>
                <div class="cta-links">
                    <a href="mailto:saaim62@gmail.com" class="cta-link">saaim62@gmail.com</a>
                    <a href="https://linkedin.com/in/senior-software-engineer2" class="cta-link" target="_blank">linkedin.com/in/senior-software-engineer2</a>
                    <a href="https://github.com/saaim62" class="cta-link" target="_blank">github.com/saaim62</a>
                </div>
            </div>
        </section>
    </main>

    <footer class="footer">
        <div class="container flex-footer">
            <p>© 2026 Saim Asif. All rights reserved.</p>
            <p class="footer-tech">Built with High-Performance HTML, CSS & JS (Vanilla)</p>
        </div>
    </footer>

    <!-- Script -->
    <script>
        document.addEventListener("DOMContentLoaded", () => {
            const observerOptions = {
                root: null,
                rootMargin: '0px',
                threshold: 0.1
            };

            const observer = new IntersectionObserver((entries, observer) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('appear');
                        observer.unobserve(entry.target);
                    }
                });
            }, observerOptions);

            document.querySelectorAll('.fade-in-up').forEach(element => {
                observer.observe(element);
            });

            // Smooth scrolling for navigation links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    const target = document.querySelector(this.getAttribute('href'));
                    if (target) {
                        window.scrollTo({
                            top: target.offsetTop - 80, // Offset for fixed navbar
                            behavior: 'smooth'
                        });
                    }
                });
            });
        });
    </script>
</body>
</html>
