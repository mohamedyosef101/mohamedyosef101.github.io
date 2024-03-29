---
# Leave the homepage title empty to use the site title
title: ''
date: 2024-02-14
type: landing

sections:

  ### BIO ###
  - block: about.biography
    id: bio
    content:
      title: Welcome 👋
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin

  ### FEATURED ###
  - block: collection
    id: featured
    content:
      title: Featured
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: compact

  ### PUBLICATIONS ###
  - block: portfolio
    id: publications
    content:
      title: Publications
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
        - name: User Experience
          tag: User Experience
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: compact


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
