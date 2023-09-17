---
# Leave the homepage title empty to use the site title
# NOTE: you can use HTML and CSS as regular.
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: Welcome to Marionville FBLA
      image:
        filename: logo-in-website.png
      cta:
        label: '**Subscribe**'
        url: example.com
      cta_alt:
        label: Make a Request
        url: https://docs.google.com/forms/d/e/1FAIpQLSc9zGAn356-OcOvZ19PWAkMEsnyEOkG-NtaK8t-QRmmJ8Y1cA/viewform?usp=sf_link
      cta_note:
        label: >-
    
      text: |-
        <br>
        We are a high school organization that teaches and guides members about business-related education.
        <br>
        -
        <br>

        **Want to subscribe to our newsletter or make a request?**

        <button class="button" style="
        background-color: #ffffff; 
        color: #104d92; 
        text-decoration: none; 
        padding:  12px 20px; 
        border-radius: 5px; 
        font-weight: bold;">
          Some Text
        </button>

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
      title: FBLA's Objective 
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: marionville-fbla
  - block: features
    content:
      title: Monthly Newsletter <br><br>
      items:
        - name:
          description:
          icon:
          icon_pack:
        - name: October Newsletter
          description: Our FBLA school organization believes in recognizing the outstanding achievements of our members. Each month, we curate a special newsletter highlighting deserving individuals who have excelled in their commitment to business and leadership. This initiative aims to celebrate their hard work, dedication, and contributions within our community, fostering a culture of appreciation and motivation for all our members.
          icon: r-project
          icon_pack: fab
        - name:
          description:
          icon:
          icon_pack:
  - block: experience
    content:
      title: Dates for Events
      #   Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: =title field=
          company: Marionville FBLA
          company_url: 'https://example.com'
          company_logo: null-icon
          location: =location field=
          date_start: '2023-09-01'
          date_end: ''
          description: |2-
              ~ Description Field:

              * Supports syntaxing.
              * Supports basic rich text.
        - title: =title field=
          company: Marionville FBLA
          company_url: 'https://example.com'
          company_logo: null-icon
          location: =location field=
          date_start: '2023-09-01'
          date_end: '2023-09-02'
          description: |2-
              ~ Description Field:
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: FBLA Posts
      subtitle: ''
      text: |-
        {{% callout note %}}
          Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
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
        {{< gallery album="fbla-gallery" >}}
    design:
      columns: '1'
  
  # Put Publications you Want to Show First
  
  #- block: collection
  #  id: featured
  #  content:
  #    title: Featured Publications
  #    filters:
  #      folders:
  #        - publication
  #      featured_only: true
  #  design:
  #    columns: '2'
  #    view: card
  
  # Put Recent Publications
  
  #- block: collection
  #  content:
  #    title: Recent Publications
  #   text: |-
  #      {{% callout note %}}
  #      Quickly discover relevant content by [filtering publications](./publication/).
  #      {{% /callout %}}
  #    filters:
  #      folders:
  #        - publication
  #      exclude_featured: true
  #  design:
  #    columns: '2'
  #    view: citation
  
  # Talks and Discussions | Slides
  
  #- block: collection
  # id: talks
  #  content:
  #    title: Recent & Upcoming Talks
  #    filters:
  #      folders:
  #        - event
  #  design:
  #    columns: '2'
  #    view: compact

  # List Popular Topics

  #- block: tag_cloud
  #content:
  #   title: Popular Topics
  # design:
  #   columns: '2'

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-

      # Commented Out Additional Contacts:

      # Contact (add or remove contact options)
      # email: kallen@marionville.us
      # phone: (417) 403-4341
    
      # Below are commented out addresses, contact hours, and appointment URL:
    
      # appointment_url: 'https://calendly.com'
      # address:
      # street: 450 Serra Mall
      # city: Stanford
      # region: CA
      # postcode: '94305'
      # country: United States
      # country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #  - 'Monday 10:00 to 13:00'
      #  - 'Wednesday 09:00 to 10:00'
    
      contact_links:
        - icon: instagram
          icon_pack: fab
          name: Instagram
          link: 'https://www.instagram.com/marionville_fbla/'
        - icon: snapchat
          icon_pack: fab
          name: Snapchat
          link: 'example.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: true
    design:
      columns: '2'
---