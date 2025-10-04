---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing


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

      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["0", "0", "0", "0"]
        margin: [0, 0, "100px", 0]

  - block: hero
    content:
      title: 
    design:
      # spacing:
      #   # Customize the section spacing. Order is top, right, bottom, left.
      #   padding: ["0", "0", "0", "0"]
      #   margin: [0, 0, 0, 0]
      # For full-screen, add `min-h-screen` below
      # css_class: "min-h-screen"
      background:
        # color: "navy"
        image:
          # Add your image background to `assets/media/`.
          filename: convictions2.svg
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
      text: |-
        <div style="text-align: center;">

        # Mes services

          <div style="color: black;">

          Des offres modulables pour votre propre besoin et selon votre maturité Data / IA

          </div>

        </div>

    design:
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["0", "0", "0", "0"]
        margin: [0, 0, 0, 0]
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
      title: "Mes services"
      text: "Discover what makes our platform special"
      items:
        - title: Designer et déployer des plateformes IA
          text: Permettre à vos équipes de développer des produits IA, du POC à la mise en Production, en toute autonomie
          feature_icon: bolt
          features:
            - Une conception en collaboration avec vos équipes opérationnelles (Infrastructure, Data Scientists, ML Engineer, Data Engineer) et de gouvernance
            - Une plateforme adaptée à votre SI et vos compétences internes rendant son utilisation, sa maintenance et son évolutivité la plus fluide pour vos équipes.
            - Des choix technologiques modernes et flexibles pour une évolutivité dans le temps
          # Upload image to `assets/media/` and reference the filename here
          image: 'Workflow 3.png'
          button:
            text: Voir mon expérience client
            url: https://hugoblox.com/templates/
        - title: Développement de produits IA
          text: Apporter une excellence opérationnelle pour délivrer des produits IA à forte valeur ajoutée 
          feature_icon: bolt
          features:
            - Construire avec les équipes opérationnelles des produits IA de l'idéation des cas d'usage à leur run en suivant les meilleurs pratiques méthodologiques de l'IA de Confiance (performance, robustesse, cycle de vie des modèles, explicabilité, etc)
            - Travailler en étroite collaboration avec les équipes métiers pour atteindre des objectifs pertinents et réalistes (ateliers pédagogiques sur l'IA, co-construction de KPI cibles)
            - Faire échouer rapidement les projets à faible valeur ajoutée et fiabiliser ceux dont le ROI positif est prouvé
            - Appliquer les meilleurs pratiques de Software Engineering et DevOps (versionning, reproductibilité, automatisation, etc) pour des livraisons régulières et fiables tout en assurant la montée en compétences des équipes (Peer Programming, revus de code)
            
          # Upload image to `assets/media/` and reference the filename here
          image: 'Team Coding.png'
          button:
            text: Voir mon expérience client
            url: https://discord.gg/z8wNYzb
        - title: Former vos équipes IA
          text: Accélérer et robustifier la production de produits IA à l'échelle
          feature_icon: bolt
          features:
            - Former vos équipes aux derniers outils et méthodologies de développement de produits IA (théorie & pratique) personnalisées pour vos équipes
            - Structurer et standardiser les pratiques de développement de vos équipes Data Science / ML Engineer
            - Suivre vos équipes au quotidien afin d'améliorer leur vélocité et prise de recul en projet (design, ateliers, Peer Programming, etc)
          # Upload image to `assets/media/` and reference the filename here
          image: 'Workflow 1.png'
          button:
            text: Voir mon expérience client
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
          description: "Data Scientists utilisent ma dernière plateforme IA"
        - statistic: "50%"
          description: "de temps réduit pour passer un produit IA en production"
        - statistic: "300"
          description: "collaborateurs formés à la Data Science / ML Engineering"
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
        offset: 0
    design:
      view: article-grid
      columns: 3
      show_date: false
      # show_read_time: false
      show_read_more: false
      fill_image: false
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["60px", "0", "0", "0"]
        margin: [0, 0, 0, 0]


  - block: resume-experience
    id: experiences
    content:
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["60px", "0", "0", "0"]
        margin: [0, 0, 0, 0]

  - block: features
    id: skills
    content:
      title: "Mes compétences"
      text: "6+ années à déployer des algorithmes de ML / AI dans des infrastructures clouds"
      items:
        - name: "Développement logiciel Python"
          description: "Développement Python sur des **projets de ML utilisés en production** utilisant des frameworks modernes de qualité: uv, pydantic, pytest, fastAPI "
          icon: "custom/python"

        - name: "Data Processing"
          description: "Framework de data processing **selon la volumétrie de données à disposition**: numpy, pandas, polars, pyspark, SQL (Snowflake, AWS Athena). Orchestrateur de pipeline de données: Airflow"
          icon: "custom/data"

        - name: "Machine Learning"
          description: "Développement d'**IA prédictive** (classification, régression, time series, NLP, ... ). Frameworks: plotly, streamlit, scikit-learn, XgBoost/LightGBM, Huggingface, .... Et d'**IA Générative** (RAG). Frameworks: LangChain, Huggingface, Qdrant, ..."
          icon: "custom/machine-learning"

        - name: "IA de Confiance"
          description: |
            Méthodologie scientifiques et techniques basé sur les risques pour assurer des développements de produits IA en accords avec les **objectifs business et éthique de l'entreprise** (Performance, Robustesse, explicabilité, analyse des biais, cycle de vie des modèles, etc)
          icon: "custom/ia-confiance"

        - name: "MlOps"
          description: |
            Application de concepts DevOps appliqué au machine learning: **CI / CD, déploiement d'application containerisé, gestion d'environnement, Infrastructure as Code, gestion de serveur**. Les frameworks maitrisés: Git, Github Action, TeamCity, Azure DevOps, Docker, Kubernetes, Terraform, Ansible, Packer.
          icon: "custom/devops"

        - name: "Databricks"
          description: "Développement d'une **plateforme IA sur Databricks pour une 30aine de Data Scientists** pendant 2 ans. Frameworks utilisés: Databricks Asset Bundle, Workflow Databricks, MlFlow, Unity Catalog et Team City/Terraform pour la CI/CD."
          icon: "custom/databricks_logo"

        - name: "AWS"
          description: "Mise en production d'un **modèle de scoring marketing sur une stack hébergé sur un AWS**. Frameworks: Mlflow, Airflow, EC2, S3, Athena, Jenkins, Prometheus, Grafana"
          icon: "custom/aws"

        - name: "Azure"
          description: "Utilisant le service de ML managé **Azure Machine Learning**, mise en production de 2 modèles de crédits bancaires déployés dans des API délivrant 15 000 prédictions à la semaine. Frameworks: Kedro, Mlflow, Azure Pipelines, AKS et Azure DevOps pour la CI/CD"
          icon: "devicon/azure"
        
        - name: "Management"
          description: "**Management opérationnel** (production conjointe, design, ateliers et Peer Programming) et **de pilotage** (définition et priorisation des tâches, validation de qualité de delivery) sur **plusieurs projets Data Sciences en parallèle**. Sélection de consultants sur projets selon les compétences recherchés par le client."
          icon: "custom/management2"

        - name: "Design de formation & Formateur"
          description: "Création de contenus pédagogiques et animation de plus d'une **vingtaine de formations pour former environ 300 collaborateurs** (clients et internes) sur des thématiques diverses: Data Sciences général, IA de Confiance, python, SQL. Formateurs de la Yotta Academy, **bootcamp Machine Learninng Engineer** créé en 2020."
          icon: "custom/learn2"

        - name: "Communication"
          description: "Fluidifier les échanges en assurant l**e bon niveau de communication** entre le client (Head of AI), les équipes opérationnelles projets ainsi que les équipes métiers. **Embarquer et animer une équipe interne** sur l'IA de Confiance pour développer l'offre de formation sur le sujet."
          icon: "custom/communication"

        - name: "Maîtrise de la langue anglaise"
          description: "**Mission chez plusieurs clients en contexte internationnal** (Italie, États-Unis, Espagne, Allemagne). Formation IA de Confiance à destination d'une 50aine de collaborateurs au États-Unis. **Travail pendant 1 an en Nouvelle-Zélande (2025)**."
          icon: "custom/english"
    design:
      columns: "3"
      background:
        color: "gray-50"
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["0", "0", "0", "0"]
        margin: [0, 0, 0, 0]

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
