---
title: 'Experience'
date: 2023-10-24
type: landing

design:
  spacing: '5rem'
  background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: pic_me 5.jpg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: resume-experience
    content:
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
  - block: resume-skills
    content:
      title: Other Skills & Hobbies
      username: admin
    design:
      show_skill_percentage: false
  - block: resume-awards
    content:
      title: Non Academic Awards


      username: admin
  - block: resume-languages
    content:
      title: Languages
      username: admin
---
