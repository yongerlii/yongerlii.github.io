---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: hero
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: Hugo Academic Theme
      image:
        filename: hero-academic.png
      cta:
        label: '**Get Started**'
        url: https://hugoblox.com/templates/
      cta_alt:
        label: Ask a question
        url: https://discord.gg/z8wNYzb
      cta_note:
        label: >-
          <div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star Hugo Blox Builder</a></div><div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/theme-academic-cv" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star the Academic template</a></div>
      text: |-
        **Generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 500,000+ sites.**

        **Easily build anything with blocks - no-code required!**

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.

        <!--Custom spacing-->
        <div class="mb-3"></div>
        <!--GitHub Button JS-->
        <script async defer src="https://buttons.github.io/buttons.js"></script>
    design:
      background:
        gradient_end: '#1976d2'
        gradient_start: '#004ba0'
        text_color_light: true
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '1'
  - block: experience
    id: experiences
    content:
      title: Experiences
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Assistant Professor/Postdoc
          company: Shanghai University
          company_url: ''
          company_logo: SHU
          location: Shanghai
          date_start: '2022-09-20'
          date_end: ''
          design:
            columns: '2'
          description: '' #|2-
              #Responsibilities include:

              #* Analysing
              #* Modellin
              #* Deploying
        - title: Visiting Scholar
          company: Politechnico di Milano
          company_url: ''
          company_logo: Polimi
          location: Milano
          date_start: '2019-09-04'
          date_end: '2021-11-12'
          description: '' #|2-
             #Taught electronic engineering 
             #* and researched semiconductor physics.
             #![png](output_1_0.png)
    design:
      columns: '2'
  - block: accomplishments
    id: activities
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: Academic Activities
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: ''
          date_end: ''
          date_start: '2020-07-01'
          description: |2-
              Member of IEEE:
              * Systems, Man, and Cybernetics Society Membership
              * Control Systems Society Membership
              * Reliability Society Membership

              Member of Chinese Association of Automation (CAA)  
              Member of Chinese Association for Artificial Intelligence (CAAI)  
              Member of China Instrument and Control Society (CIS)
          icon: (coursera)
          organization: #Coursera
          organization_url: #https://www.coursera.org
          title: Member
          url: ''
        - certificate_url: #https://www.edx.org
          date_end: ''
          date_start: '2020-07-01'
          description: |2-
              * [Instrumentation (English edition of a Chinese core/EI journal)](http://www.instrumentationjournal.com/inst/home)  
              * [AI and Autonomous Systems](https://elspub.com/journals/artificial-intelligence-and-autonomous-systems/home)
          icon: #edx
          organization: #edX
          organization_url: #https://www.edx.org
          title: Youth Editorial Board Member #Blockchain Fundamentals
          url: #https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
        - certificate_url: ''
          date_end: ''
          date_start: '2020-07-01'
          description: |2-
              [Machines (SCI index)](https://www.mdpi.com/journal/machines)
          icon: ''
          organization: #Coursera
          organization_url: #https://www.coursera.org
          title: Guset Editor
          url: ''
        - certificate_url: #https://www.datacamp.com
          date_end: ''
          date_start: '2020-07-01'
          description: |2-
               * the 6<sup>th</sup> IEEE International Conference on Industrial Cyber-Physical Systems (2023.05)  
               * the International Conference on 6<sup>th</sup> Robotics, Control and Automation Engineering (2023.11)
          icon: #datacamp
          organization: #DataCamp
          organization_url: #https://www.datacamp.com
          title: Conference Chair
          url: ''
        - certificate_url: #https://www.datacamp.com
          date_end: ''
          date_start: '2020-07-01'
          description: 'IEEE Transactions on Neural Networks and Learning Systems, IEEE Transactions on Instrumentation and Measurement, IEEE Transactions on Systems, Man, and Cybernetics: Systems, IEEE Transactions on Industrial Informatics, IEEE Transactions on Industrial Electronics, Sustainable Energy Grids and Networks, Mechtronics, and Asian Journal of Control, among others'
          icon: #datacamp
          organization: #DataCamp
          organization_url: #https://www.datacamp.com
          title: Reviewer
          url: ''
    design:
      columns: '2'
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
    content:
      title: Patents
      text: '' #|-
        #{{% callout note %}}
        #Quickly discover relevant content by [filtering publications](./publication/).
        #{{% /callout %}}
      filters:
        folders:
          - patent
        exclude_featured: true
    design:
      columns: '2'
      view: citation
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
        - name: Vertical Research Project
          tag: 'Vertical Research Project'
        - name: Horizontal Research Project
          tag: 'Horizontal Research Project'
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 0
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
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Seminar
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
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-   #Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
        Ciao, Amore! ❤️
      # Contact (add or remove contact options as necessary)
      email: yongerlii@163.com
      phone: 888 888 88 88
      appointment_url: 'https://calendly.com'
      address:
        street: No.99, Shangda Road
        city: Shanghai
        region: Shanghai
        postcode: '200444'
        country: China
        country_code: CN
      directions: ✨
      office_hours:
        - 'Monday 09:00 to 17:00'
        - 'Wednesday 09:00 to 17:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '31.31229'
        longitude: '121.39826'  
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/Twitter'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'skype:echo123?call'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
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


[def]: https://www.coursera.org
[def2]: http://www.instrumentationjournal.com/inst/home