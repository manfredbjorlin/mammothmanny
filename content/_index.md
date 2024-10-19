---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        icon: {{< ico bootstrap house >}}
        text: Twitch
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: mammothgrey.png
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false  
  - block: cta-button-list
    id: links
    content:
      buttons:
        - text: Twitch
          icon: brands/twitch
          url: http://tvitch.com/mamnmothmannny
        - text: Discord
          icon: brands/discord
          url: https://discord.gg/jSTymXqSAC
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  
---
