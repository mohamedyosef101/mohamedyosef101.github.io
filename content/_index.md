---
# Leave the homepage title empty to use the site title
title: ''
date: 2024-02-14
type: landing

sections:

  - block: hero
    id: hero
    demo: false
    content:
      title: 'Putting data into action'
      username: admin
      image:
        filename: 'hero-img.png'
      cta:
        label: 
        url: 
      cta_alt: 
        label: 
        url: 
      text: |-
        <p style="font-size: 90%; padding-top: 0.1rem;">
        <b> Hi, I’m Mohamed, and welcome to my journey in Data Science and Analytics.</b><br><br>
        My focus is on building data-driven solutions and leveraging advanced analytics to solve real-world challenges. I specialise in developing machine learning models, predictive analytics, and time series forecasting to help businesses make smarter, data-backed decisions. By bridging the gap between data science theory and practical application, I explore how analytics can drive innovation across industries and provide deeper insights into the world around us.
        </p>

    design:
      background:
        gradient_end: '#FEFEFE'
        gradient_start: '#FEFEFE'
        text_color_light: false

  ### BIO ###
  - block: about.biography
    id: bio
    content:
      title: 'About Me'
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin

  ### FEATURED ###
  - block: features
    id: featured
    content:
      title: Featured
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card

  ### LEARNINGS ###
  - block: collection
    id: reviews
    content:
      title: Lit. Reviews
      filters:
        folders:
          - publication
        publication_type: "review"
    design:
      columns: '2'
      view: compact

  ### PUBLICATIONS ###
  - block: portfolio
    id: publications
    content:
      title: All Publications
      filters:
        folders:
          - publication
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Reinforcement Learning
          tag: Reinforcement Learning
        - name: Analytics
          tag: Data Analysis
          tag: Data Science 
        - name: User Experience
          tag: User Experience
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: masonry


  ### TALKS ### 
  - block: collection
    id: talks
    content: 
      title: Talks
      filters: 
        folders: 
          - event
    design: 
      columns: '2'
      view: youtube

  ### TAGS ###
  - block: tag_cloud
    id: tags
    content:
      title: 
    design:
      columns: '1'
---
