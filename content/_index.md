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
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: resume-skills
    content:
      username: "admin"
      title: "My skills"
      text: "This is sample text content for the section."
    design:
      background:
        # color: ""
        gradient_start: "#4f46e5"
        gradient_end: "#7c3aed"
        text_color_light: true
      spacing:
        padding: ["16", "16", "16", "16"]
      columns: "3"
  - block: stats
    content:
      items:
        - statistic: "50K+"
          description: "Happy Users"
        - statistic: "99.9%"
          description: "Uptime"
        - statistic: "24/7"
          description: "Support"
    design:
      background:
        color: "gray-900"
        text_color_light: true
      columns: "3"
  - block: markdown
    id: section-2
    content:
      title: Section 2
      subtitle: A subtitle
      text: Add your Section 2 content here...
    design:
      background:
        # Choose colors such as from https://html-color-codes.info
        gradient_start: '#52bf90'
        gradient_end: '#317256'
        # The gradient angle from 0-360 degrees
        gradient_angle: 45
        # Text color (true=light, false=dark, or remove for the dynamic theme color).
        text_color_light: true
  - block: testimonials
    content:
      title: "What Our Users Say"
      items:
        - name: "John Doe"
          role: "Product Manager"
          organization: "Tech Company"
          avatar: "path/to/avatar.jpg"
          content: "This platform has revolutionized how we build websites!"
        - name: "Jane Smith"
          role: "Designer"
          organization: "Creative Agency"
          content: "The blocks are beautiful and so easy to customize."
    design:
      columns: "2"
  - block: resume-awards
    content:
      username: "admin"
      title: "My Section Title"
      text: "This is sample text content for the section."
    design:
      background:
        color: ""
        gradient_start: "#4f46e5"
        gradient_end: "#7c3aed"
        text_color_light: true
      spacing:
        padding: ["6", "6", "6", "6"]
      columns: "1"
  - block: features
    content:
      title: "Amazing Features"
      text: "Discover what makes our platform special"
      items:
        - name: "Fast Performance"
          description: "Lightning-fast load times for better user experience"
          icon: "bolt"
        - name: "Easy to Use"
          description: "Intuitive interface that anyone can master"
          icon: "heart"
        - name: "Secure"
          description: "Enterprise-grade security built-in"
          icon: "shield-check"
    design:
      columns: "3"
      background:
        color: "gray-50"
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.

        I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.

        Please reach out to collaborate 😃
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
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
      text: ''
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
      view: card
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
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
