---
title: Media
date: 2023-10-24
type: landing

sections:
  - block: hero_banner
    content:
      title: Media
    design:
      spacing:
        padding: [0, 0, 0, 0]
        margin: [0, 0, 0, 0]
      background:
        css_class: dark
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: banner_media.png
          filters:
            brightness: 1.0
          size: width
          position: bottom
          parallax: true
          
  - block: markdown_custom
    content:
      title: 
      subtitle:
      text: |
            <html>
            <body>
            <img class=image-left src="https://media.geeksforgeeks.org/wp-content/uploads/20240908110717/geekforgeek.png" alt="Flex Image" width=400px>
              <p>TEXT</p>
            <p>
            <br/><br/>
            <hr width="100%" size="2">
            <br/><br/>
            </p>
            </body>
            </html>
    design:
      spacing:
        padding: [0, 0, 0, 0]
        margin: [0, 0, 0, 0]
---
