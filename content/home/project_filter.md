---
widget: portfolio
headless: true
weight: 40
# ... Put Your Section Options Here (title etc.) ...

content:
  # Page type to display. E.g. project.
  page_type: project

# Uncomment to only show content with specific tags
#  filters:
#    tags:
#      - featured project

  # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below)
  filter_default: 0

  # Filter toolbar (optional).
  # Add or remove as many filters (`filter_button` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `filter_button` below.
  filter_button:
    - name: All
      tag: 'Projects'
    - name: Life Cycle
      tag: LCA
    - name: Energy
      tag: Energy
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
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns: '1'
  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact  
  #   3 = Card
  #   5 = Showcase
  view: 3
  flip_alt_rows: false
---
