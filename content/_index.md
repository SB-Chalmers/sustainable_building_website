---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: |
        Sustainable building
        Research Group
      image:
        filename: welcome.jpg
      text: |
        <br>
        
        The research group Sustainable building works with concepts, tools and strategies to enhance the sustainability 
        performance of construction materials, building products, buildings as well as entire cities. 
        The research is related to ecological and economic life cycle assessment of construction materials, 
        buildings and infrastructures, sustainability assessment tools for buildings, social-cultural and climate 
        adapted design concepts as well as energy and material resource based building stock modeling and its visualization.

  
  - block: collection
    content:
      title: Latest News
      subtitle:
      text:
      count: 5
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: post
    design:
      view: compact
      columns: '1'
  
  - block: portfolio
    id: projects
    content:
      title: Projects
      subtitle: 
      text: 
      filters:
        # Folders to display content from
        folders:
          - project
        # Only show content with these tags
        tags: []
        # Exclude content with these tags
        exclude_tags: []
        # Which Hugo page kinds to show (https://gohugo.io/templates/section-templates/#page-kinds)
        kinds:
          - page
      # Field to sort by, such as Date or Title
      sort_by: 'Date'
      sort_ascending: false
      # Default portfolio filter button
      # 0 corresponds to the first button below and so on
      # For example, 0 will default to showing all content as the first button below shows content with *any* tag
      default_button_index: 0
      # Filter button toolbar (optional).
      # Add or remove as many buttons as you like.
      # To show all content, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the button toolbar, delete the entire `buttons` block.
      buttons:
        - name: All
          tag: 'Projects'
        - name: Life Cycle
          tag: 'LCA'
        - name: Energy
          tag: 'Energy'
        - name: Computational Sustainable design
          tag: ComputationalSustainableDesign
        - name: Sustainable Building
          tag: SustainableBuilding
        - name: Digital Twins
          tag: DTCC
        - name: Digital Tools
          tag: DigitalTools
        - name: Courses
          tag: Teaching_Courses
    design:
      # See Page Builder docs for all section customization options.
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      # Choose a listing view
      view: card
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  
  - block: tag_cloud
    content:
      title: 
      subtitle: 
      text: 
      # Choose a taxonomy from the `taxonomies` list in `config.yaml` to display (e.g. tags, categories, authors)
      taxonomy: tags
      # Choose how many tags you would like to display (0 = all tags)
      count: 20
    design:
      # Minimum and maximum font sizes (1.0 = 100%).
      font_size_min: 0.7
      font_size_max: 2.0
---