# content/_index.md
# Leave the homepage title empty to use the site title
title: "Xiaolei"
date: 2022-10-24
type: landing
design:
  # Default section spacing
  spacing: "6rem"
sections:
  # Bio区块 - 对应菜单中的 Bio (/)
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
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
  
  # Prospective PhD Students 区块
  - block: markdown
    content:
      title: '🎓 Prospective PhD Students' 
      subtitle: ''
      text: |-
        I am always looking for self-motivated Ph.D. students who would like to carry on top-notch research on Software and Systems Security. 
        
        Candidates are expected to have:
        - Solid background in compilers and operating systems
        - Strong programming skills
        - Passion for security research
        
        If you meet these requirements, please contact me with your CV and research interests.
    design:
      columns: '1'

  # Honors & Awards区块 - 对应菜单中的 Honors & Awards (#awards)
  - block: accomplishments
    id: awards
    content:
      title: 🏆 Honors & Awards
      subtitle: ''
      # Automatically link email and phone or display as text?
      autolink: true
      # Choose which content types to display
      content_types:
        - accomplishments
    design:
      columns: '1'

  # Publications区块 - 对应菜单中的 Publications (#publications) 
  - block: collection
    id: publications
    content:
      title: 📚 Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: citation
      columns: 2
  
  # Recent Publications
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: list

  # Team区块 - 对应菜单中的 Team (#team)
  - block: collection
    id: team
    content:
      title: 👥 Team
      text: "Meet our research team members"
      filters:
        type: author
        exclude_me: true
    design:
      view: card
      columns: 3

  # Contact区块 - 对应菜单中的 Contact (#contact)
  - block: contact
    id: contact
    content:
      title: 📬 Contact
      subtitle: Get in touch
      text: |-
        Feel free to reach out for research collaboration, academic inquiries, or prospective student applications.
      # Contact details - edit or remove as needed
      email: xlren@must.edu.mo
      address:
        street: Avenida Wai Long, Taipa
        city: Macau
        region: Macau SAR
        country: China
        country_code: MO
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '22.1562'
        longitude: '113.5592'  
      contact_links:
        - icon: google-scholar
          icon_pack: ai
          name: Google Scholar
          link: 'https://scholar.google.com/citations?user=E4KRUtoAAAAJ&hl=en'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '1'
---
