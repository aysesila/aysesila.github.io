---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: admin
      text: ''
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      css_class: hbx-bg-gradient
      avatar:
        size: medium   # small | medium | large | xl | xxl
        shape: circle  # circle | square | rounded

  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I’m a PhD student exploring the intersections of communication, computation, and intelligence across scales from biological information transfer to memory and representation in computational neuroscience. 

        My work aims to uncover how localization and communication processes, whether in physical, biological, or neural systems, can give rise to efficient computation, adaptive learning, and collective intelligence. I combine mathematical modeling, machine learning, and theoretical neuroscience to develop frameworks that bridge biological communication and artificial information processing.
        
        Always open to ideas that challenge how we understand computation in nature and engineered systems. 🧠
    design:
      columns: '1'

  - block: collection
    id: papers
    content:
      title: Publications
      filters:
        folders:
          - publications
        featured_only: false
    design:
      view: list
      columns: 1
      page_type: publication
      count: 5
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      offset: 0
      order: desc
      spacing:
        padding: [0, 0, 0, 0]
    # ... keep your resume-biography-3 block as is ...

  - block: buttons
    content:
      buttons:
        - text: Download CV
          url: uploads/resume.pdf     # file should live at /static/uploads/resume.pdf
          icon: download              # optional: try download / file-text / arrow-down-tray
          type: primary               # primary | secondary | link
          new_tab: false
    design:
      align: center                   # left | center | right

---
