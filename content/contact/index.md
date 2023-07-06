---
title: Contact
date: 2022-10-24

type: landing

sections:
  - block: contact
    content:
      title: Contact
      text: |-
        Fill in the contact form below and someone from the group will to respond to you as soon as possible.
      email: sanjay.somanath@chalmers.se
      phone: +46 31 772 10 00
      address:
        street: Sven Hultins gata 6
        city: Gothenburg
        region: GOT
        postcode: '41296'
        country: Sweden
        country_code: SWE
      coordinates:
        latitude: '57.68754773448353'
        longitude: '11.976424098148366'
      directions: Enter Building Sven Hultins gata 6 and take the stairs to level 3. There is a reception area adjacent to the stairwell, with the possibility to contact the person you are looking for.
      office_hours:
        - '9:00 to 17:00 Monday to Friday'
      #appointment_url: 'https://calendly.com'
      #contact_links:
      #  - icon: comments
      #    icon_pack: fas
      #    name: Discuss on Forum
      #    link: 'https://discourse.gohugo.io'
    
      # Automatically link email and phone or display as text?
      autolink: true
    
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle: ''
      text:
    design:
      columns: '1'
      background:
        image: 
          filename: contact.jpg
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['20px', '0', '20px', '0']
      css_class: fullscreen
---
