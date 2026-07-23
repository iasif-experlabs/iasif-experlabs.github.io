<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ibtisam Asif · Principal Full Stack Engineer</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #f4f7fc;
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
      display: flex;
      justify-content: center;
      padding: 2rem 1.5rem;
      line-height: 1.5;
      color: #1e293b;
    }

    .container {
      max-width: 1200px;
      width: 100%;
      background: white;
      border-radius: 32px;
      box-shadow: 0 20px 40px -12px rgba(0,0,0,0.15);
      padding: 2.5rem 2.8rem;
      transition: all 0.2s;
    }

    .profile-header {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: flex-start;
      margin-bottom: 2.5rem;
      border-bottom: 1px solid #e9eef3;
      padding-bottom: 2rem;
    }

    .name-title h1 {
      font-size: 2.8rem;
      font-weight: 700;
      letter-spacing: -0.02em;
      color: #0b1e33;
      margin-bottom: 0.25rem;
    }

    .name-title .badge {
      display: inline-block;
      background: #dbeafe;
      color: #1e4a7a;
      font-weight: 600;
      font-size: 0.9rem;
      padding: 0.3rem 1rem;
      border-radius: 40px;
      margin-top: 0.2rem;
      letter-spacing: 0.3px;
    }

    .contact-links {
      display: flex;
      flex-wrap: wrap;
      gap: 1.5rem 2.5rem;
      margin-top: 0.5rem;
    }

    .contact-item {
      display: flex;
      align-items: center;
      gap: 0.6rem;
      font-size: 0.95rem;
      color: #1e3a5f;
      background: #f8fafc;
      padding: 0.3rem 1rem 0.3rem 0.8rem;
      border-radius: 40px;
      border: 1px solid #e2e8f0;
    }

    .contact-item i {
      color: #2563eb;
      width: 1.1rem;
      font-size: 1rem;
    }

    .contact-item a {
      text-decoration: none;
      color: #1e3a5f;
      font-weight: 500;
    }

    .contact-item a:hover {
      color: #2563eb;
    }

    .summary {
      background: #f8fafc;
      padding: 1.6rem 2rem;
      border-radius: 24px;
      margin-bottom: 2.8rem;
      border-left: 5px solid #2563eb;
      font-size: 1.05rem;
      line-height: 1.6;
      color: #1e293b;
      box-shadow: 0 2px 6px rgba(0,0,0,0.02);
    }

    .summary strong {
      color: #0b1e33;
    }

    .two-column {
      display: grid;
      grid-template-columns: 1fr 1.8fr;
      gap: 2.5rem;
    }

    .sidebar {
      display: flex;
      flex-direction: column;
      gap: 2.2rem;
    }

    .card {
      background: #fafcff;
      border-radius: 24px;
      padding: 1.6rem 1.8rem;
      border: 1px solid #eef2f6;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.02);
    }

    .card-title {
      font-size: 1.1rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.4px;
      color: #2563eb;
      margin-bottom: 1.4rem;
      border-bottom: 2px solid #e2e8f0;
      padding-bottom: 0.6rem;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    .card-title i {
      font-size: 1.1rem;
      color: #2563eb;
    }

    .skill-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem 0.6rem;
    }

    .skill-tag {
      background: #eef4ff;
      color: #1e3a5f;
      font-size: 0.8rem;
      font-weight: 500;
      padding: 0.3rem 1rem;
      border-radius: 40px;
      border: 1px solid #dbe4ed;
      letter-spacing: 0.2px;
    }

    .skill-tag.highlight {
      background: #2563eb;
      color: white;
      border-color: #2563eb;
    }

    .competency-list {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 0.7rem;
    }

    .competency-list li {
      display: flex;
      align-items: baseline;
      gap: 0.7rem;
      font-size: 0.95rem;
      font-weight: 500;
      color: #0b1e33;
    }

    .competency-list li i {
      color: #2563eb;
      font-size: 0.8rem;
      width: 1.2rem;
      text-align: center;
    }

    .project-item {
      margin-bottom: 1.2rem;
    }

    .project-item:last-child {
      margin-bottom: 0;
    }

    .project-item h4 {
      font-weight: 700;
      font-size: 1rem;
      color: #0b1e33;
      display: flex;
      align-items: center;
      gap: 0.3rem;
    }

    .project-item p {
      font-size: 0.9rem;
      color: #334155;
      margin-top: 0.1rem;
      padding-left: 0.2rem;
    }

    .education-item {
      margin-bottom: 0.3rem;
    }

    .education-item h4 {
      font-weight: 700;
      font-size: 1rem;
      color: #0b1e33;
    }

    .education-item .meta {
      font-size: 0.9rem;
      color: #475569;
    }

    .main-content {
      display: flex;
      flex-direction: column;
      gap: 2rem;
    }

    .exp-item {
      margin-bottom: 2rem;
      border-bottom: 1px solid #edf2f7;
      padding-bottom: 1.8rem;
    }

    .exp-item:last-child {
      border-bottom: 0;
      margin-bottom: 0;
      padding-bottom: 0;
    }

    .exp-header {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: baseline;
      margin-bottom: 0.3rem;
    }

    .exp-header h3 {
      font-size: 1.25rem;
      font-weight: 700;
      color: #0b1e33;
      letter-spacing: -0.3px;
    }

    .exp-header .company {
      font-weight: 600;
      color: #2563eb;
      font-size: 1rem;
    }

    .exp-header .date {
      font-size: 0.85rem;
      background: #eef2f6;
      padding: 0.15rem 0.9rem;
      border-radius: 40px;
      color: #1e3a5f;
      font-weight: 500;
    }

    .exp-desc {
      margin-top: 0.5rem;
      padding-left: 0.2rem;
    }

    .exp-desc ul {
      list-style: none;
      padding-left: 0.2rem;
    }

    .exp-desc ul li {
      position: relative;
      padding-left: 1.5rem;
      margin-bottom: 0.5rem;
      font-size: 0.95rem;
      color: #1e293b;
    }

    .exp-desc ul li::before {
      content: "▹";
      position: absolute;
      left: 0;
      color: #2563eb;
      font-weight: 700;
    }

    .tech-badge {
      display: inline-block;
      background: #eef4ff;
      border-radius: 30px;
      font-size: 0.7rem;
      font-weight: 600;
      padding: 0.15rem 0.8rem;
      margin-right: 0.3rem;
      color: #1e4a7a;
      border: 1px solid #dce6f0;
      letter-spacing: 0.2px;
    }

    .freelance-note {
      margin-top: 0.3rem;
      font-style: italic;
      color: #475569;
      font-size: 0.9rem;
      background: #f8fafc;
      padding: 0.4rem 0.8rem;
      border-radius: 30px;
      display: inline-block;
    }

    html {
      scroll-behavior: smooth;
    }

    .navbar {
      display: flex;
      justify-content: flex-end;
      padding-bottom: 1rem;
      margin-bottom: 1.5rem;
      position: sticky;
      top: 0;
      background: rgba(255, 255, 255, 0.95);
      backdrop-filter: blur(10px);
      z-index: 100;
      padding-top: 1rem;
      margin-top: -1rem;
      border-bottom: 1px solid #e9eef3;
    }
    .nav-links {
      display: flex;
      gap: 1.5rem;
      flex-wrap: wrap;
    }
    .nav-links a {
      text-decoration: none;
      color: #1e3a5f;
      font-weight: 600;
      font-size: 0.95rem;
      transition: all 0.2s;
      padding: 0.4rem 0.8rem;
      border-radius: 8px;
    }
    .nav-links a:hover {
      background: #eef4ff;
      color: #2563eb;
    }

    @media (max-width: 900px) {
      .container {
        padding: 1.8rem;
      }
      .two-column {
        grid-template-columns: 1fr;
        gap: 1.8rem;
      }
      .profile-header {
        flex-direction: column;
        gap: 1rem;
      }
      .contact-links {
        gap: 0.8rem 1.5rem;
      }
    }

    @media (max-width: 550px) {
      body {
        padding: 0.8rem;
      }
      .container {
        padding: 1.2rem;
        border-radius: 24px;
      }
      .name-title h1 {
        font-size: 2rem;
      }
      .exp-header {
        flex-direction: column;
        align-items: flex-start;
        gap: 0.3rem;
      }
      .summary {
        padding: 1.2rem;
        font-size: 0.95rem;
      }
      .contact-item {
        padding: 0.2rem 0.7rem 0.2rem 0.6rem;
        font-size: 0.8rem;
      }
    }
  </style>
</head>
<body>
<div class="container">

  <nav class="navbar">
    <div class="nav-links">
      <a href="#summary">Summary</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#experience">Experience</a>
    </div>
  </nav>

  <div class="profile-header">
    <div class="name-title">
      <div class="badge"><i class="fas fa-code" style="margin-right: 6px;"></i>Principal Full Stack Engineer · Engineering Lead</div>
      <div style="margin-top: 10px; font-size: 0.95rem; color: #1e3a5f; background: #f1f5f9; padding: 0.2rem 1rem; border-radius: 30px; display: inline-block;">
        <i class="fas fa-map-pin" style="margin-right: 6px; color: #2563eb;"></i> Lahore, Pakistan
      </div>
    </div>
    <div class="contact-links">
      <div class="contact-item"><i class="fas fa-phone-alt"></i> +92 301 4775234</div>
      <div class="contact-item"><i class="fas fa-envelope"></i> <a href="mailto:ibtisamasif@gmail.com">ibtisamasif@gmail.com</a></div>
      <div class="contact-item"><i class="fab fa-github"></i> <a href="https://github.com/ibtisamasif" target="_blank" rel="noopener noreferrer">GitHub</a></div>
      <div class="contact-item"><i class="fab fa-linkedin-in"></i> <a href="https://linkedin.com/in/ibtisamasif" target="_blank" rel="noopener noreferrer">LinkedIn</a></div>
    </div>
  </div>

  <div id="summary" class="summary">
    <strong>Engineering Lead & Principal Full Stack Engineer</strong> with 10+ years of experience delivering large-scale SaaS, eCommerce, logistics, fintech, and enterprise platforms. Proven track record of leading cross-functional engineering teams, owning end-to-end product delivery, and building scalable systems from concept to production. Experienced in stakeholder management, roadmap planning, system architecture, cloud infrastructure, and engineering execution.
  </div>

  <div class="two-column">

    <div class="sidebar">

      <div id="skills" class="card">
        <div class="card-title"><i class="fas fa-microchip"></i> Technical Skills</div>
        <div style="margin-bottom: 0.8rem;">
          <div style="font-weight: 600; font-size: 0.75rem; letter-spacing: 0.3px; color: #475569; margin-bottom: 0.2rem;">LEADERSHIP & DELIVERY</div>
          <div class="skill-tags">
            <span class="skill-tag">Engineering Leadership</span>
            <span class="skill-tag">Delivery Management</span>
            <span class="skill-tag">Roadmap Planning</span>
            <span class="skill-tag">Stakeholder Management</span>
            <span class="skill-tag">Team Building</span>
            <span class="skill-tag">Mentorship</span>
            <span class="skill-tag">Agile Delivery</span>
          </div>
        </div>
        <div style="margin-bottom: 0.8rem;">
          <div style="font-weight: 600; font-size: 0.75rem; letter-spacing: 0.3px; color: #475569; margin-bottom: 0.2rem;">FRONTEND</div>
          <div class="skill-tags">
            <span class="skill-tag highlight">Next.js</span>
            <span class="skill-tag">React</span>
            <span class="skill-tag">TypeScript</span>
            <span class="skill-tag">JavaScript</span>
            <span class="skill-tag">Redux</span>
            <span class="skill-tag">Tailwind CSS</span>
          </div>
        </div>
        <div style="margin-bottom: 0.8rem;">
          <div style="font-weight: 600; font-size: 0.75rem; letter-spacing: 0.3px; color: #475569; margin-bottom: 0.2rem;">BACKEND</div>
          <div class="skill-tags">
            <span class="skill-tag">Python (FastAPI)</span>
            <span class="skill-tag">NestJS</span>
            <span class="skill-tag">Node.js</span>
            <span class="skill-tag">Kotlin</span>
            <span class="skill-tag">Spring Boot</span>
            <span class="skill-tag">REST APIs</span>
            <span class="skill-tag">Microservices</span>
          </div>
        </div>
        <div style="margin-bottom: 0.8rem;">
          <div style="font-weight: 600; font-size: 0.75rem; letter-spacing: 0.3px; color: #475569; margin-bottom: 0.2rem;">DATABASES</div>
          <div class="skill-tags">
            <span class="skill-tag">PostgreSQL</span>
            <span class="skill-tag">MySQL</span>
            <span class="skill-tag">MongoDB</span>
            <span class="skill-tag">Firebase</span>
            <span class="skill-tag">Snowflake</span>
            <span class="skill-tag">SQL Server</span>
          </div>
        </div>
        <div style="margin-bottom: 0.2rem;">
          <div style="font-weight: 600; font-size: 0.75rem; letter-spacing: 0.3px; color: #475569; margin-bottom: 0.2rem;">CLOUD & DEVOPS</div>
          <div class="skill-tags">
            <span class="skill-tag">AWS EC2</span>
            <span class="skill-tag">Docker</span>
            <span class="skill-tag">CI/CD</span>
            <span class="skill-tag">Linux</span>
            <span class="skill-tag">Git</span>
            <span class="skill-tag">CloudFormation</span>
            <span class="skill-tag">ECR</span>
          </div>
        </div>
        <div style="margin-top: 0.6rem;">
          <div style="font-weight: 600; font-size: 0.75rem; letter-spacing: 0.3px; color: #475569; margin-bottom: 0.2rem;">ARCHITECTURE</div>
          <div class="skill-tags">
            <span class="skill-tag">SaaS Platforms</span>
            <span class="skill-tag">Multi-Tenant Systems</span>
            <span class="skill-tag">RBAC</span>
            <span class="skill-tag">Distributed Systems</span>
            <span class="skill-tag">System Design</span>
          </div>
        </div>
      </div>

      <div class="card">
        <div class="card-title"><i class="fas fa-bolt"></i> Core Competencies</div>
        <ul class="competency-list">
          <li><i class="fas fa-check-circle"></i> Full Stack SaaS Development</li>
          <li><i class="fas fa-check-circle"></i> System Design & Scalable Architecture</li>
          <li><i class="fas fa-check-circle"></i> Team Leadership & Mentorship</li>
          <li><i class="fas fa-check-circle"></i> High-Performance Backend Systems</li>
          <li><i class="fas fa-check-circle"></i> Product-Focused Engineering</li>
        </ul>
      </div>

      <div id="projects" class="card">
        <div class="card-title"><i class="fas fa-folder-open"></i> Key Projects</div>
        <div class="project-item">
          <h4><i class="fas fa-cube" style="color: #2563eb; font-size: 0.8rem;"></i> LogiSort</h4>
          <p>A CMP-based WMS SaaS platform for real-time warehouse operations.</p>
        </div>
        <div class="project-item">
          <h4><i class="fas fa-boxes" style="color: #2563eb; font-size: 0.8rem;"></i> PackTrack</h4>
          <p>A warehouse scanning system for optimizing logistics workflows.</p>
        </div>
        <div class="project-item">
          <h4><i class="fas fa-chair" style="color: #2563eb; font-size: 0.8rem;"></i> Seated</h4>
          <p>A scalable restaurant reservation platform serving millions of users.</p>
        </div>
      </div>

      <div class="card">
        <div class="card-title"><i class="fas fa-graduation-cap"></i> Education</div>
        <div class="education-item">
          <h4>Bachelor of Science in Computer Science</h4>
          <div class="meta">University of Lahore · 2010 – 2015</div>
        </div>
      </div>

    </div>

    <div id="experience" class="main-content">

      <div class="exp-item">
        <div class="exp-header">
          <div><h3>Senior Software Engineer · Engineering Lead</h3><span class="company">FullBeauty Brands</span></div>
          <span class="date">Jan 2024 – Present</span>
        </div>
        <div class="exp-desc">
          <ul>
            <li>Led design and delivery of the Full Beauty Product Costing Tool, an enterprise apparel sourcing platform automating seasonal RFQs, vendor quote collection, and Estimated Landed Cost (ELC) reporting.</li>
            <li>Architected a FastAPI/Python backend integrating Snowflake (PLM), SQL Server (QAD planning), and PostgreSQL, replacing spreadsheet-based costing with near-real-time reporting refreshed every 15 minutes.</li>
            <li>Built a high-complexity costing engine computing ocean/air landed costs across duties, surcharges, agent commissions, and freight — processing thousands of SKUs per seasonal buy cycle.</li>
            <li>Delivered end-to-end RFQ automation: PLM-driven item ingestion → vendor assignment → SMTP invitations → secure vendor self-service portal → three-stage approval workflow.</li>
            <li>Implemented multi-source data pipelines with daily PLM sync, automated HTS/tariff modeling, and Teams alerting — reducing manual data reconciliation effort by ~75% and cutting RFQ turnaround time by ~60%.</li>
            <li>Established Microsoft Entra ID SSO for internal admin APIs and token-based auth for external vendor portals, with session-based audit logging across 8+ reference datasets.</li>
            <li>Operated AWS EC2/Docker deployments across dev/prod with cron-scheduled batch jobs, ECR-based releases, and production reliability practices — maintaining 99.5%+ uptime.</li>
            <li><strong>Owned end-to-end product lifecycle:</strong> architecture → development → deployment.</li>
          </ul>
          <div style="margin-top: 0.4rem;"><span class="tech-badge">FastAPI</span><span class="tech-badge">Snowflake</span><span class="tech-badge">PostgreSQL</span><span class="tech-badge">AWS EC2</span><span class="tech-badge">Docker</span><span class="tech-badge">Entra ID</span></div>
        </div>
      </div>

      <div class="exp-item">
        <div class="exp-header">
          <div><h3>Principal Software Engineer · Full Stack Lead</h3><span class="company">Seated</span></div>
          <span class="date">Jan 2020 – Jan 2024</span>
        </div>
        <div class="exp-desc">
          <ul>
            <li>Led full-stack development using Next.js and NestJS, ensuring scalable and maintainable architecture.</li>
            <li>Designed and implemented high-performance APIs and backend services.</li>
            <li>Built and optimized user-facing features, improving customer conversion rates by 19%.</li>
            <li>Improved system performance and key business metrics, increasing restaurant revenue by 18%.</li>
            <li>Designed A/B testing pipelines and analytics integrations for data-driven product decisions.</li>
            <li>Collaborated with cross-functional teams to deliver scalable product features.</li>
            <li>Led a team of 15+ engineers, driving architecture decisions and code quality standards.</li>
            <li>Implemented fraud detection systems, reducing fraudulent activities by 20%.</li>
            <li><strong>Owned end-to-end product lifecycle:</strong> architecture → development → deployment.</li>
          </ul>
          <div style="margin-top: 0.4rem;"><span class="tech-badge">Next.js</span><span class="tech-badge">NestJS</span><span class="tech-badge">TypeScript</span><span class="tech-badge">React</span><span class="tech-badge">PostgreSQL</span></div>
        </div>
      </div>

      <div class="exp-item">
        <div class="exp-header">
          <div><h3>Senior Software Engineer · Full Stack Developer</h3><span class="company">WAFIOS (Connectavo)</span></div>
          <span class="date">Aug 2018 – Jan 2020</span>
        </div>
        <div class="exp-desc">
          <ul>
            <li>Built scalable web and backend systems for industrial automation platforms.</li>
            <li>Developed APIs and services using modern backend practices.</li>
            <li>Collaborated with frontend teams to deliver real-time monitoring dashboards.</li>
            <li>Contributed to building a product from scratch, onboarding enterprise clients.</li>
            <li>Improved development speed across teams by 90% through optimized workflows.</li>
            <li>Ensured high performance and reliability in regulated environments.</li>
          </ul>
        </div>
      </div>

      <div class="exp-item">
        <div class="exp-header">
          <div><h3>Tech Lead & Consultant (Full Stack)</h3><span class="company">Outstart Tech</span></div>
          <span class="date">Aug 2017 – Aug 2018</span>
        </div>
        <div class="exp-desc">
          <ul>
            <li>Designed and implemented full-stack architectures for multiple client projects.</li>
            <li>Led development teams and ensured high-quality deliverables.</li>
            <li>Managed project lifecycle including planning, execution, and deployment.</li>
            <li>Worked closely with stakeholders to translate business needs into technical solutions.</li>
          </ul>
        </div>
      </div>

      <div class="exp-item">
        <div class="exp-header">
          <div><h3>Senior Software Engineer (Full Stack)</h3><span class="company">LastingSales</span></div>
          <span class="date">Sep 2016 – July 2017</span>
        </div>
        <div class="exp-desc">
          <ul>
            <li>Developed scalable web applications and backend systems.</li>
            <li>Designed APIs and handled database integrations.</li>
            <li>Collaborated with teams to deliver production-grade applications.</li>
            <li>Focused on performance optimization and maintainability.</li>
          </ul>
        </div>
      </div>

      <div class="exp-item">
        <div class="exp-header">
          <div><h3>Lecturer – Software Engineering / Web Development</h3><span class="company">UOL</span></div>
          <span class="date">Sep 2016 – July 2018</span>
        </div>
        <div class="exp-desc">
          <ul>
            <li>Taught software engineering, system design, and web development concepts.</li>
            <li>Mentored students in modern development practices.</li>
          </ul>
        </div>
      </div>

      <div class="exp-item">
        <div class="exp-header">
          <div><h3>Freelance Full Stack Developer & SEO Consultant</h3><span class="company">Upwork</span></div>
          <span class="date">2009 – 2016</span>
        </div>
        <div class="exp-desc">
          <ul>
            <li>Built and managed web applications and SEO projects.</li>
            <li>Led a team of 8–10 developers and marketers.</li>
          </ul>
          <div class="freelance-note"><i class="fas fa-briefcase" style="margin-right: 6px;"></i> 7+ years of freelance & consulting experience</div>
        </div>
      </div>

    </div>
  </div>
</div>
</body>
</html>
