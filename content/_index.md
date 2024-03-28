---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing



sections:
  - block: hero
    demo: false # Only display this section in the Hugo Blox Builder demo site
    content:
      image: 
        filename: blank.png
      title: '**Hi,**'
      cta:
        label: 'Know more'
        url: '#about'
      text: |-
        {{< figure src="blank.png" >}}
        ## _It's [ME](https://www.youtube.com/watch?v=b1kbLwvqugk)_🎶   

        I am the problem

        ## _It's_ **_Wing_🪽**
    
        I explore fun things in immersive environment.
        {{< figure src="blank.png" >}}
    design:
      css_class: "dark min-h-screen"
      background:
        color: "zinc"
        video:
      # Name of video in `assets/media/`.
          filename: covervideo.mp4
      # Post-processing: flip the video horizontally?
          flip: false
        size: cover
        position: center
        text_color_light: true
  - block: about.biography
    id: about
    content: 
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
    design:
      background:
        image:
          filename: cover.jpg
      # Apply image filters?
          filters:
        # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.2
        size: cover
        position: center
        parallax: true
        text_color_light: true
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
        - name: User Experience
          tag: User Experience
        - name: Virtual Production
          tag: Virtual Production
        - name: Research Experience
          tag: Research Experience
        - name: Coursework
          tag: Coursework
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: true
      background:
        image:
          filename: cover.jpg
      # Apply image filters?
          filters:
        # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.1
        size: cover
        position: center
        parallax: true
        text_color_light: true
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
      background:
        image:
          filename: cover.jpg
      # Apply image filters?
          filters:
        # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.2
        size: cover
        position: center
        parallax: true
        text_color_light: true
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
      view: List
      background:
        image:
          filename: cover.jpg
      # Apply image filters?
          filters:
        # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.1
        size: cover
        position: center
        parallax: true
        text_color_light: true
  - block: experience
    content: 
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Internship in Oversea Influencer Marketing
          company: Netease youdao
          company_url: https://mobile.youdao.com
          company_logo: netease
          location: Guangzhou
          date_start: '2022-05-10'
          date_end: '2022-08-01'
          description: |2-
              Responsibilities include:

              * Translating oversea influencer videos.
              * Data Analysing.
              * Contacting oversea influencer.
        - title: Profesional Volunteer in Photography
          company: 2022 Beijing Winter Olympics and Paralympic
          company_url: https://olympics.com/ioc/theme-beijing-2022
          company_logo: wo2022
          location: Beijing
          date_start: '2022-01-01'
          date_end: '2022-03-15'
          description: |2-
              Responsibilities include:

              * Offering help for photography journalists.
              * Office work in the National Stadium photography department.
        - title: Internship in Music Marketing
          company: Tencent Music Entertainment
          company_url: https://www.tencentmusic.com
          company_logo: tme
          location: Beijing
          date_start: '2021-07-01'
          date_end: '2021-09-30'
          description: |2-
              Responsibilities include:

              * Estabilishing playlists for promotion.
              * Data Analysing.
    design:
      columns: '2'
      background:
        image:
          filename: cover.jpg
      # Apply image filters?
          filters:
        # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.2
        size: cover
        position: center
        parallax: true
        text_color_light: true
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
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
          date_start: '2022-12-25'
          description: ''
          icon: ''
          organization: Beijing Film Academy
          organization_url: https://www.bfa.edu.cn
          title: 'Academic Postgraduate Scholarship'
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2021-12-25'
          description: ''
          icon: ''
          organization: Beijing Film Academy
          organization_url: https://www.bfa.edu.cn
          title: 'First Class Academic Scholarship'
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2021-10-17'
          description: ''
          icon: ''
          organization: The 5th China Competition on Virtual Reality(CCVR 2022)
          organization_url: http://ccvr.aconf.cn/index.html
          title: 'CCVR First Pride'
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2020-12-25'
          description: ''
          icon: ''
          organization: Beijing Film Academy
          organization_url: https://www.bfa.edu.cn
          title: 'Thrid Class Academic Scholarship'
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2019-12-25'
          description: ''
          icon: ''
          organization: Beijing Film Academy
          organization_url: https://www.bfa.edu.cn
          title: 'Thrid Class Academic Scholarship'
          url: ''
    design:
      columns: '2'
      background:
        image:
          filename: cover.jpg
      # Apply image filters?
          filters:
        # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.1
        size: cover
        position: center
        parallax: true
        text_color_light: true
  - block: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '2'
      background:
        image:
          filename: cover.jpg
      # Apply image filters?
          filters:
        # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.2
        size: cover
        position: center
        parallax: true
        text_color_light: true
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Activities
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
      background:
        image:
          filename: cover.jpg
      # Apply image filters?
          filters:
        # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.1
        size: cover
        position: center
        parallax: true
        text_color_light: true
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Feel Free to contact me whether you have a question or just want to make friends!
      # Contact (add or remove contact options as necessary)
      email: zhongyingcw@mail.bfa.edu.cn
      phone: ''
      appointment_url: ''
      address:
        street: 4 Xitucheng Rd
        city: Beijing
        region: Beijing
        postcode: '100088'
        country: China
        country_code: CN
      directions: Bulding C, 2nd Floor, Virtual Reality Lab
      office_hours:
        - '10:00 to 24:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '116.355751'
        longitude: '39.9716'  
      contact_links:
        - icon: instagram
          icon_pack: fab
          name: DM Me
          link: 'https://www.instagram.com/aroastedchicken/'
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
      background:
        image:
          filename: cover.jpg
      # Apply image filters?
          filters:
        # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.2
        size: cover
        position: center
        parallax: true
        text_color_light: true
---
