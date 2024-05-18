---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: features
    content:
      title: Skills
      items:
        - name: Chatting
          description: 150%
          icon: telegram
          icon_pack: fab
        - name: Waste money
          description: 100%
          icon: cc-visa
          icon_pack: fab
        - name: Linux
          description: 200%
          icon: linux
          icon_pack: fab
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Student
          company: People's friendship university of Russia
          company_url: ''
          company_logo: Logo_rudn_znak
          location: Moscow
          date_start: '2022-09-01'
          date_end: ''
          description: |2-
              Studies include:

              * Math
              * Coding
              * Rutubing
        - title: Pupil
          company: School №1 with intensified english studies
          company_url: ''
          company_logo: org-x
          location: Vologda
          date_start: '2011-09-01'
          date_end: '2022-05-31'
          description: Spend my childhood there. 11 years of studies.
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.rudn.ru/
          date_end: ''
          date_start: '2022-09-01'
          description: ''
          organization: PFUR
          organization_url: https://www.rudn.ru/
          title: Entered RUDN University
          url: ''
        - certificate_url: https://www.youtube.com/@artyomnorm
          date_end: ''
          date_start: '2023-03-08'
          description: 
          organization: Youtube
          organization_url: https://youtube.com
          title: 11 subscribers on my Youtube chanel
          url: ''
        - certificate_url: https://ankudryashovNKA.github.io
          date_end: ''
          date_start: '2023-04-01'
          description: ''
          organization: Internet
          organization_url: https://google.com
          title: 'Created hugo site'
          url: ''
        - certificate_url: https://disk.yandex.ru/i/e8Z-j4K7rLIDPA
          date_end: '2024-05-18'
          date_start: '2024-02-17'
          description: 'Passed 100%'
          organization: Stepik
          organization_url: https://www.stepik.org
          title: The basics of cybersecurity
          url: https://stepik.org/course/111512/info
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
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
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
      # Contact (add or remove contact options as necessary)
      email: 1132226433@pfur.ru
      address:
        street: Mikluho-Malkaya Street, 6
        city: Moscow
        postcode: '117198'
        country: Russia
        country_code: RU
      contact_links:
        - icon: fab fa-etsy
          icon_pack: fab
          name: eLIBRARY
          link: 'https://www.elibrary.ru/'
        - icon: fab fa-google
          icon_pack: fab
          name: Google Scholar
          link: 'https://scholar.google.com/'
        - icon: fab fa-opera
          icon_pack: fab
          name: ORCID
          link: 'https://orcid.org/'
        - icon: fab fa-mendeley
          icon_pack: fab
          name: Mendeley
          link: 'https://www.mendeley.com/'
        - icon: fab fa-ravelry
          icon_pack: fab
          name: ResearchGate
          link: 'https://www.researchgate.net/profile/Artyom-Kudryashov-2'
        - icon: fab fa-autoprefixer
          icon_pack: fab
          name: Academia.edu
          link: 'https://independent.academia.edu/ArtyomKudryashov'
        - icon: fab fa-artstation
          icon_pack: fab
          name: arXiv
          link: 'https://arxiv.org/'
        - icon: fab fa-github
          icon_pack: fab
          name: Github
          link: 'https://github.com/ankudryashovNKA'
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
      columns: '2'
---
