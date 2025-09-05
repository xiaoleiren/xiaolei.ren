sections:
  # Bio区块 - 对应菜单Bio
  - block: resume-biography-3
    content:
      username: admin
      text: ""
    design:
      css_class: dark
      background:
        color: black
        image:
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  
  # Prospective PhD Students
  - block: markdown
    content:
      title: '🎓 Prospective PhD Students' 
      text: |-
        I am always looking for self-motivated Ph.D. students...
    design:
      columns: '1'

  # Awards区块 - 对应菜单Honors & Awards (#awards)
  - block: accomplishments
    id: awards
    content:
      title: 🏆 Honors & Awards
      subtitle: ''
    design:
      columns: '1'

  # Publications区块 - 对应菜单Publications (#publications)
  - block: collection
    id: publications
    content:
      title: 📚 Publications
      filters:
        folders:
          - publication
    design:
      view: citation

  # Team区块 - 对应菜单Team (#team)
  - block: collection
    id: team
    content:
      title: 👥 Team
      filters:
        folders:
          - authors
        exclude_me: true
    design:
      view: card

  # Contact区块 - 对应菜单Contact (#contact)
  - block: contact
    id: contact
    content:
      title: 📬 Contact
      email: xlren@must.edu.mo
    design:
      columns: '1'
