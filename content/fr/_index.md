---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

# design:
#   # Default section spacing
#   spacing: ''

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: 'Résumé'
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
          #  Image fit. Options are `cover` (default), `contain`, or `actual` size.
          size: contain
          # Image focal point. Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: false


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
          text: Permettre à vos équipes de développer des produits IA, du POC à la mise en Production, en toute autonomie
          feature_icon: bolt
          features:
            - Une conception en collaboration avec vos équipes opérationnelles et de gouvernance 
            - Une plateforme adaptée à votre SI et vos compétences internes
            - Des choix technologiques modernes et flexibles pour une évolutivité dans le temps
            - Autonomie des équipes et handover. Copetence humaine pour l'evolutivité de la plateforme  
          # Upload image to `assets/media/` and reference the filename here
          image: 'Workflow 3.png'
          button:
            text: Voir mon experience client
            url: https://hugoblox.com/templates/
        - title: Développement de produits IA
          text: Apporter une excellence opérationnelle pour délivrer des produits IA à forte valeur ajoutée 
          feature_icon: bolt
          features:
            - Travailler en étroite collaboration avec les équipes métier pour atteindre leurs objectifs
            - Construire avec les équipes opérationnelles des produits IA de bout en bout
            - Appliquer les meilleurs pratiques de DevOps et Software Engineering pour des livraisons régulières et fiables tout en assurant la montée en compétences des équipes
          # Upload image to `assets/media/` and reference the filename here
          image: 'Team Coding.png'
          button:
            text: Voir mon experience client
            url: https://discord.gg/z8wNYzb
        - title: Former vos équipes IA
          text: Accélérer et robustifier la production de produits IA à l'echelle
          feature_icon: bolt
          features:
            - Former vos équipes aux outils et méthodologies de développement de produits IA
            - Structurer et standardiser les pratiques de développement de vos équipes Data Science / ML Engineer
            - Suivre vos équipes au quotidien afin d'améliorer leur vélocité et prise de recul en projet ()
          # Upload image to `assets/media/` and reference the filename here
          image: 'Workflow 1.png'
          button:
            text: Voir mon experience client
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
          description: "Data Scientist utilisaient ma dernière plateforme IA"
        - statistic: "50%"
          description: "de temps réduit pour passer un produit IA en production"
        - statistic: "300"
          description: "clients / collègues formés à la Data Science / ML Engineering"
    design:
      background:
        color: "gray-900"
        text_color_light: true
      columns: "3"
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["0", "0", "0", "0"]
        margin: [0, 0, 0, 0]
      # css_class: "tight-spacing"

  - block: collection
    id: projects
    content:
      title: Mes projets clients & open source
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
        - name: "Développement logiciel Python"
          description: "6+ ans de développement Python sur des projets de ML dont la majorité utilisée en production utilisant des frameworks modernes de qualité: uv, pydantic, pytest, fastAPI "
          icon: "devicon/python"
        - name: "Data Processing"
          description: "Framework de data processing selon la volumétrie de données à disposition: numpy, pandas, polars, pyspark, SQL (Snowflake, AWS Athena). Orchestrateur de pipeline de données: Airflow"
          icon: "devicon/python"
        - name: "Machine Learning"
          description: "Développement d'IA prédictive (classification, régression, time series, NLP, ... ). Frameworks utilisé: plotly, streamlit, scikit-learn, XgBoost/LightGBM, Huggingface, ..."
          icon: "devicon/azure"
        - name: "Cycle de vie des modèles IA"
          description: |
            Méthodologie et framework pour passer un produit IA du POC à la production: MlFlow, Airflow, 
          icon: "devicon/azure"
        - name: "Databricks"
          description: "Développement d'une plateforme IA sur Databricks pendant 2 ans pour une 30aine de Data Scientists. Frameworks utilisés: Databricks Asset Bundle, Workflow Databricks, MlFlow, Unity Catalog."
          icon: "custom/databricks_logo"
        - name: "Azure Machine Learning"
          description: "Mise en production de 2 modèles de crédits bancaires déployés dans des API délivrant 15 000 prédictions à la semaine"
          icon: "custom/azure_ml_logo"
        
        - name: "Management"
          description: "TODO"
          icon: "shield-check"
    design:
      columns: "3"
      background:
        color: "gray-50"

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
          parallax: true

---
