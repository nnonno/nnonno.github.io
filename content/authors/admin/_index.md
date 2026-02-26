---
# Display name
title: 吴一夫

# Name pronunciation (optional)
name_pronunciation: Yi Fu Wu

# Full name (for SEO)
first_name: Yifu
last_name: Wu

# Status emoji
status:
  icon: ☕️

# Is this the primary user of the site?
superuser: true

# Highlight the author in author lists? (true/false)
highlight_name: true

# Role/position/tagline
role: Applied Scientist

# Organizations/Affiliations to display in Biography blox
organizations:
  - name: AWS GenAI
    url: https://aws.amazon.com/ai/generative-ai/

# Social network links
# Need to use another icon? Simply download the SVG icon to your `assets/media/icons/` folder.
profiles:
  - icon: at-symbol
    url: 'mailto:wuyifu2f@gmail.com'
    label: E-mail Me
  - icon: brands/github
    url: https://github.com/nnonno
  - icon: brands/linkedin
    url: https://www.linkedin.com/in/yifu-wu-09609779/
  - icon: academicons/google-scholar
    url: https://scholar.google.com/citations?hl=en&user=DJw9oO0AAAAJ
  - icon: academicons/orcid
    url: https://orcid.org/0000-0001-5132-2980

interests:
  - NLP & Large Language Models
  - Distributed Systems & HPC
  - Cybersecurity & Privacy
  - AI Infrastructure

education:
  - area: PhD in Computer and Information Technology
    institution: Purdue University
    date_start: 2019-08-01
    date_end: 2024-05-01
    summary: |
      Dissertation: _Data-Driven Computing and Networking Solution for Securing Cyber-Physical Systems_. Supervised by [Prof Jin Wei-Kocsis](https://polytechnic.purdue.edu/profile/kocsis0). Research areas: distributed machine learning, HPC infrastructure, cybersecurity, resource allocation, AI for robotics. 15+ publications, 2 US patents.
    button:
      text: 'Read Thesis'
      url: "https://hammer.purdue.edu/articles/thesis/Data-Driven_Computing_and_Networking_Solution_for_Securing_Cyber-Physical_Systems/25744824?file=46078863"
  - area: ME in Electronic and Computer Engineering
    institution: University of Limerick
    date_start: 2013-09-01
    date_end: 2015-01-01
    summary: VLSI circuit design and test, embedded systems, hardware-software integration
  - area: BS in Automation
    institution: Harbin Institute of Technology
    date_start: 2007-09-01
    date_end: 2011-07-01
    summary: Industrial control systems and automation

work:
  - position: Applied Scientist
    company_name: AWS GenAI
    company_url: ''
    company_logo: ''
    date_start: 2025-04-14
    date_end: ''
    summary: |
      LLM inference optimization and responsible AI:
      - Optimized LLM inference with sglang and vLLM, achieving 50% latency reduction
      - Built multilingual PII and policy violation classifiers (Sparse RoBERTa, Qwen3-0.6B), improving precision by 60%
      - Developed guardrail models for Alexa's core LLM ensuring policy-compliant responses across languages
  - position: NLP Data Scientist
    company_name: University of Colorado Anschutz Medical Campus
    company_url: ''
    company_logo: ''
    date_start: 2024-08-20
    date_end: 2025-03-31
    summary: |
      Clinical NLP research:
      - Built clinical diagnosis reasoning via knowledge graph networks with LLM reasoning and response re-ranking
      - Designed LLM pretraining pipeline over large-scale healthcare knowledge bases with distributed training
      - Contributed to LogosKG: hardware-optimized scalable knowledge graph retrieval system
      - Coauthored paper on clinical text summarization with temporal reasoning (EMNLP 2025)
  - position: Machine Learning Engineer Intern
    company_name: AI Newsletter Startup
    company_url: ''
    company_logo: ''
    date_start: 2024-06-15
    date_end: 2024-08-15
    summary: |
      AI-powered newsletter generation:
      - Built event clustering/extraction on web-scraped data with RAG for news summarization
      - Engineered LLM-powered summarization and rewriting pipeline for production content workflows
  - position: Research Assistant
    company_name: Purdue University
    company_url: ''
    company_logo: ''
    date_start: 2019-12-01
    date_end: 2024-05-01
    summary: |
      HPC, distributed systems & AI infrastructure research:
      - Designed decentralized ML system for NASA spacecraft networks using blockchain-based coordination
      - Built distributed ML on embedded devices (Raspberry Pi, Nvidia Jetson) using Torch-TensorRT
      - Developed GPT-3.5 agentic coding workflow for autonomous robot control code generation
      - Published multiple papers in IEEE and top-tier venues on distributed systems and cybersecurity
  - position: Research Assistant
    company_name: Iowa State University
    company_url: ''
    company_logo: ''
    date_start: 2017-08-01
    date_end: 2017-12-31
    summary: |
      HPC storage systems:
      - Optimized HPC distributed storage I/O throughput prediction using LSTM/RNN models on Lustre parallel filesystem across 32-node clusters
  - position: Research Assistant
    company_name: University of Akron
    company_url: ''
    company_logo: ''
    date_start: 2015-08-01
    date_end: 2019-07-31
    summary: |
      Networking security & smart grid systems:
      - Designed HIL testing infrastructure for large-scale renewable energy systems
      - Implemented attack detection and resilient communication middleware for smart grids using ML and SDN
      - Developed blockchain-powered decentralized computing system (2 US patents granted)
  - position: Instructor
    company_name: Tsinghua IT Training School
    company_url: ''
    company_logo: ''
    date_start: 2015-01-01
    date_end: 2015-06-30
    summary: |
      Taught C programming fundamentals and web development (HTML/HTML5)
  - position: Software Engineer
    company_name: Haite Measurement and Control Technology Co.
    company_url: ''
    company_logo: ''
    date_start: 2011-09-01
    date_end: 2012-12-31
    summary: |
      Developed embedded system software using industrial fieldbuses (Modbus, Profibus-PA/DP) for measurement and control systems

# Skills
# Add your own SVG icons to `assets/media/icons/`
skills:
  - name: Technical Skills
    items:
      - name: Python
        description: ''
        percent: 100
        icon: devicon/python
      - name: PyTorch
        description: ''
        percent: 90
        icon: devicon/pytorch
      - name: Linux
        description: ''
        percent: 80
        icon: devicon/linux

  - name: Hobbies
    color: '#eeac02'
    color_border: '#f0bf23'
    items:
      - name: Hiking
        description: Mostly day hike and rarely backpacking
        percent: 75
        icon: person-simple-walk
      - name: Photography
        description: ''
        percent: 75
        icon: camera

languages:
  - name: Chinese
    percent: 100
  - name: English
    percent: 75

# Awards.
#   Add/remove as many awards below as you like.
#   Only `title`, `awarder`, and `date` are required.
#   Begin multi-line `summary` with YAML's `|` or `|2-` multi-line prefix and indent 2 spaces below.
awards:

---

## About Me
Yifu Wu is an Applied Scientist at AWS GenAI. He has 14+ years of experience spanning NLP, distributed systems, HPC, cybersecurity, and AI infrastructure. His work includes LLM inference optimization, production-scale multilingual classifiers, clinical NLP, and distributed ML systems for NASA spacecraft networks. He holds a PhD from Purdue University with 15+ peer-reviewed publications and 2 US patents.
