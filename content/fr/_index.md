---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

# design:
#   # Default section spacing
#   spacing: ''

sections:
  - block: resume-biography
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      # headings:
      #   about: 'This about'
      #   education: 'This is education'
      #   interests: 'This intereste'
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded

  - block: hero
    content:
      title: 
      # primary_action:
      #   text: Let's connect on Linkedin
      #   url: https://www.linkedin.com/in/philippe-neveux/
      #   icon: rocket-launch
      # secondary_action:
      #   text: Read the docs
      #   url: https://docs.hugoblox.com
      # announcement:
      #   text: "Announcing the release of version 1."
      #   link:
      #     text: "Read more"
      #     url: "/blog/"
    design:
      spacing:
        padding: [0, 0, 0, 0]
        margin: [0, 0, 0, 0]
      # For full-screen, add `min-h-screen` below
      css_class: "min-h-screen"
      background:
        # color: "navy"
        image:
          # Add your image background to `assets/media/`.
          filename: convictions.svg
          # filters:
          #   brightness: 0.5
          size: cover
          position: center
          parallax: true


  - block: markdown
    id: services
    content:
      title: ''
      subtitle: ''
      text: |-
        <div style="text-align: center;">

        # Mes services

        </div>

    design:
      columns: '1'
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["0", "0", "0", "0"]
      # background:
      #   color: "navy"


  # - block: stats
  #   content:
  #     items:
  #       - statistic: "Deploy MLOps Platform"
  #         description: "Trust me I am an Engineer"
  #       - statistic: "Deploy ML Use cases"
  #         description: "From a POC to an industrialized project"
  #       - statistic: "Upskill your AI Team"
  #         description: "Already taught 300+ collabs"
  #   design:
  #     background:
  #       color: "gray-900"
  #       text_color_light: true
  #     columns: "2"
  #     spacing:
  #       # Customize the section spacing. Order is top, right, bottom, left.
  #       padding: ["0", "0", "0", "0"]
  
      
  - block: cta-image-paragraph
    content:
      items:
        - title: Designer et déployer des plateformes IA
          text: Permettrent à vos équipes de développer des produits IA, du POC à la Production, en toute autonomie
          feature_icon: check
          features:
            - Une plateforme adaptée à votre SI et vos compétences internes
            - Une conception en collaboration avec vos équipes opérationnelles et de gouvernance 
            - Des choix technologiques modernes et fléxible pour une évolutivité dans le temps   
          # Upload image to `assets/media/` and reference the filename here
          image: 'Workflow 3.png'
          button:
            text: Ma Méthode
            url: https://hugoblox.com/templates/
        - title: Développement de produits IA
          text: Apporter une excellence opérationnelle pour délivrer des produits IA à forte valeur ajoutée 
          feature_icon: bolt
          features:
            - Construire avec les équipes opérationnelles des produits IA de bout en bout
            - Travailler en étroite collaboration avec les équipes métier pour atteindre leurs objectifs
            - Appliquer les meilleurs pratiques de DevOps et Software Engineering pour des livraisons régulières et fiables
          # Upload image to `assets/media/` and reference the filename here
          image: 'Team Coding.png'
          button:
            text: Ma Méthode
            url: https://discord.gg/z8wNYzb
        - title: Former vos équipes IA
          text: Accélérer et robustifier la production de produits IA à l'echelle
          feature_icon: arrow-trending-up
          features:
            - Former vos équipes aux outils et méthodologie de développements de produits IA
            - Structurer et standardiser les pratiques de développement de vos équipes Data Science / ML Engineer
            - Coacher vos équipes au quotidien afin d'améliorer leur vélocité et prise de recul en projet.
          # Upload image to `assets/media/` and reference the filename here
          image: 'Workflow 1.png'
          button:
            text: Ma Méthode
            url: https://discord.gg/z8wNYzb
    design:
      # css_class: "tight-spacing"
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["0px", "0", "0", "0"]
        margin: [0, 0, 0, 0]

  - block: stats
    content:
      items:
        - statistic: "30"
          description: "Data Scientists use my last deployed ML Platform"
        - statistic: "50%"
          description: "Reducing time to deploy AI systems in Production "
        - statistic: "300"
          description: "Trained Clients and colleagues to Data Science / Machine Learning Engineering"
    design:
      background:
        color: "gray-900"
        text_color_light: true
      columns: "2"
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["0", "0", "0", "0"]
        margin: [0, 0, 0, 0]
      # css_class: "tight-spacing"

  # - block: markdown
  #   content:
  #     # title: 'Why my clients trust me ? 🤝'
  #     subtitle: ''
  #     text: |-
  #         <b> <span style="font-size: 35px;">Why my clients trust me ? 🤝</span> </b>
  #   design:
  #     spacing:
  #       # Customize the section spacing. Order is top, right, bottom, left.
  #       padding: ["0", "0", "0", "0"]
  - block: collection
    id: projects
    content:
      title: My Clients & Open Source Projects 
      filters:
        folders:
          - projects
    design:
      view: article-grid
      columns: 3


  - block: resume-experience
    id: experiences
    content:
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false

  - block: features
    id: skills
    content:
      title: "My Skills"
      text: "Discover what makes our platform special"
      items:
        - name: "Fast Performance"
          description: "Lightning-fast load times for better user experience"
          icon: "devicon/python"
        - name: "Easy to Use"
          description: "Intuitive interface that anyone can master"
          icon: "custom/databricks_logo"
        - name: "Secure"
          description: "Enterprise-grade security built-in"
          icon: "custom/azure_ml_logo"
        - name: "Easy to Use"
          description: "Intuitive interface that anyone can master"
          icon: "devicon/azure"
        - name: "Secure"
          description: "Enterprise-grade security built-in"
          icon: "shield-check"
    design:
      columns: "5"
      background:
        color: "gray-50"


  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     view: card
  # - block: collection
  #   id: news
  #   content:
  #     title: Recent News
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: post
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       author: ''
  #       category: ''
  #       tag: ''
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ''
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: card
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 0, 0]

  # - block: resume-awards
  #   content:
  #     username: "admin"
  #     title: "My Section Title"
  #     text: "This is sample text content for the section."
  #   design:
  #     background:
  #       color: ""
  #       gradient_start: "#4f46e5"
  #       gradient_end: "#7c3aed"
  #       text_color_light: true
  #     spacing:
  #       padding: ["6", "6", "6", "6"]
  #     columns: "1"
  # - block: collection
  #   content:
  #     title: Blog posts
  #     text: ''
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: false
  #   design:
  #     view: citation
  - block: testimonials
    content:
      title: "What My Clients Say"
      items:
        - name: "Hugo Smith"
          role: "Marketing Executive at X"
          # Upload image to `assets/media/` and reference the filename here
          image: "testimonial-1.jpg"
          text: "Awesome, so easy to use and saved me so much work with the swappable pre-designed sections!"
        - name: "Hugo Smith"
          role: "Marketing Executive at X"
          # Upload image to `assets/media/` and reference the filename here
          image: "testimonial-1.jpg"
          text: "Awesome, so easy to use and saved me so much work with the swappable pre-designed sections!"
    design:
      spacing:
        # Reduce bottom spacing so the testimonial appears vertically centered between sections
        padding: [0, 0, 0, 0]
      columns: "1"
  - block: hero
    content:
      title: If you'd like to work with me 👇
      # text: 🧱 EASY. FREE (OPEN SOURCE). NO-CODE  🧱
      primary_action:
        text: Let's connect on Linkedin
        url: https://www.linkedin.com/in/philippe-neveux/
        icon: rocket-launch
      # secondary_action:
      #   text: Read the docs
      #   url: https://docs.hugoblox.com
      # announcement:
      #   text: "Announcing the release of version 1."
      #   link:
      #     text: "Read more"
      #     url: "/blog/"
    design:
      spacing:
        padding: [0, 0, 0, 0]
        margin: [0, 0, 0, 0]
      # For full-screen, add `min-h-screen` below
      css_class: "dark"
      background:
        color: "navy"
        image:
          # Add your image background to `assets/media/`.
          filename: bg-triangles.svg
          filters:
            brightness: 0.5
          size: cover
          position: center
          parallax: false
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: 'bg-primary-700'
        css_style: ''
---
