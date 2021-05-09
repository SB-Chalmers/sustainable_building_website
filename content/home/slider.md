---
# An instance of the Blank widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: slider

weight: 10
headless: true  # This file represents a page section.

# ... Put Your Section Options Here (section position etc.) ...

# Slide interval.
# Use `false` to disable animation or enter a time in ms, e.g. `5000` (5s).
interval: 5000

# Minimum slide height.
# Specify a height to ensure a consistent height for each slide.
height: 300px

item:
  - title: Twinabler
    content: 'Checkout this project!'
    # Choose `center`, `left`, or `right` alignment.
    align: left
    # Overlay a color or image (optional).
    #   Deactivate an option by commenting out the line, prefixing it with `#`.
    overlay_color: '#6d597a'  # An HTML color value.
    overlay_img: twinable.png  # Image path relative to your `assets/media/` folder
    overlay_filter: 0.5  # Darken the image. Value in range 0-1.

  - title: Digitalisation of social sustainability in neighbourhood design
    content: 'Checkout this project!'
    align: left
    overlay_color: '#eaac8b'
    overlay_img: 'dssnd.jpg'
    overlay_filter: 0.5
    # Call to action button (optional).
    #   Activate the button by specifying a URL and button label below.
    #   Deactivate by commenting out parameters, prefixing lines with `#`.
    cta_label: See on GitHub
    cta_url: 'https://github.com/snjsomnath/PhDThesisrepo'
    cta_icon_pack: fas
    cta_icon: graduation-cap 
  - title: WELL Neighbourhood
    content: 'Checkout this project!'
    align: right
    overlay_color: '#e56b6f'
    overlay_img: 'well-neighbourhood.jpg'
    overlay_filter: 0.5
---
