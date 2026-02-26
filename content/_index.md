---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        My research spans NLP, LLMs, distributed systems, and cybersecurity. At AWS GenAI, I work on LLM inference optimization and responsible AI guardrails. Previously, I conducted clinical NLP research at the University of Colorado Anschutz Medical Campus, contributing to knowledge graph retrieval systems and clinical text summarization (EMNLP 2025). During my PhD at Purdue, I designed decentralized ML systems for NASA spacecraft networks, built distributed learning on embedded devices, and developed blockchain-powered computing systems (2 US patents). I have published 15+ papers in IEEE, AAAI, EMNLP, and other top venues.

        Please reach out to collaborate 😃
    design:
      columns: '1'

---
