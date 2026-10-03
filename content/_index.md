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
      # Hidden 2026-10-02: the old CV PDF was removed because it was out of date.
      # Re-enable once a corrected CV is placed in static/uploads/.
      # button:
      #   text: Download CV
      #   url: uploads/resume.pdf
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
        My research spans NLP, LLMs, distributed systems, and cybersecurity. At the AWS Generative AI Innovation Center, I work on agent infrastructure, prompt caching, model routing, and LLM inference efficiency. Before that, I built multilingual content-safety classifiers and responsible-AI guardrail models at Amazon Alexa. Earlier, I conducted clinical NLP research at the University of Colorado Anschutz Medical Campus, contributing to knowledge graph retrieval systems and clinical text summarization (Findings of EMNLP 2025). During my doctoral research at Purdue and the University of Akron, I designed decentralized ML systems for NASA spacecraft networks, built distributed learning on embedded devices, and developed blockchain-powered computing systems (2 US patents). I have 13 peer-reviewed publications, including IEEE journal and conference papers and an ACL 2026 main-conference paper.

        Please reach out to collaborate 😃
    design:
      columns: '1'

---
