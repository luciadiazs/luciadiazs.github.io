---
# Leave the homepage title empty to use the site title
title: ""
date: 2025-08-31
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: |-
        **Español** · Soy socióloga especializada en migración, criminalidad y desigualdad. Combino métodos cuantitativos (análisis multivariado, procesamiento de lenguaje natural, visualización) y cualitativos (entrevistas, trabajo de campo) para **informar la toma de decisiones basada en evidencia** en políticas públicas e innovación social.

        **English** · I am a sociologist focusing on migration, crime, and social inequality. I bridge quantitative methods (multivariate analysis, natural language processing, visualization) with qualitative research (interviews, fieldwork) to **inform evidence-based decision-making** in public policy and social innovation.
      # Call-to-action (opcional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      # Avatar customization
      avatar:
        size: medium  # small | medium | large | xl | xxl
        shape: circle  # circle | square | rounded
      background:
        # Solid aubergine background
        color: "#5B264B"
        # (Opcional) Deja comentado el patrón para mantener color sólido
        image:
          filename: uploads/background_1.png
          filters:
            brightness: 1.0
            opacity: 0.6
          size: cover
          position: center
          parallax: false

  - block: collection
    id: papers
    content:
      title: Featured Publications
      subtitle: ""
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1

  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ""
      text: ""
      page_type: post
      count: 5
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      offset: 0
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [0, 0, 0, 0]
---
