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
        url: http://eepurl.com/izlBpk
      cta_alt:
        label: Make a Request
        url: https://docs.google.com/forms/d/e/1FAIpQLSc9zGAn356-OcOvZ19PWAkMEsnyEOkG-NtaK8t-QRmmJ8Y1cA/viewform?usp=sf_link
      cta_note:
        label: '<a href="https://docs.google.com/forms/d/e/1FAIpQLSdX1Noxn0oGZrmlIvlHYKFDlBYGShRKTOzxF7AJRJ5r4WcF5g/viewform?usp=sf_link" target="_blank">**🎁 A CHRISTMAS SURPRISE 🎁**</a>'
    
      text: |-
        <br>
        We are a high school organization that teaches and guides members about business-related education.
        <br>
        -
        <br>

        **Want to subscribe to our newsletter or make a request?**

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
  - block: collection
    id: officers
    content:
      title: Marionville FBLA Officers <br><br>
      count: 0
      filters:
        folders: 
          - publication
  - block: experience
    id: upcoming
    content:
      title: Upcoming Activities
      #   Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: FBLA Christmas Party
          company: Marionville FBLA
          # company_url: '/talk/marionville-blood-drive-fall/'
          company_logo: fbla-christmas-party
          location: Marionville First Baptist Church
          date_start: '2016-01-01'
          date_end: '2020-12-31'
          description: |2-
              About:

              * Have Fun with Team Members!
              * Skip a Day from School!
              * And get a Present from FBLA!
    design:
      columns: '1'
  - block: collection
    id: posts
    content:
      title: FBLA Posts
      subtitle: ''
      text: |-
        {{% callout note %}}
          Discover all of our content by [accessing all posts](./post/).
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

  # Uncomment this if we have any projects we want to display.      
  - block: portfolio
    id: events
    content:
      title: Events
      filters:
        folders:
          - project
  # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
  #    # Filter toolbar (optional).
  #    # Add or remove as many filters (`filter_button` instances) as you like.
  #    # To show all items, set `tag` to "*".
  #    # To filter by a specific tag, set `tag` to an existing tag name.
  #    # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Competitions
          tag: Competitions
        - name: Resources
          tag: Resources
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  
  - block: markdown
    id: gallery
    content:
      title: FBLA Pictures
      subtitle: ''
      text: |-
        <br>
        <br>
        {{< gallery album="fbla-gallery" >}}
    design:
      columns: '1'

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-

##############

      contact_links:
        - icon: instagram
          icon_pack: fab
          name: Instagram
          link: 'https://www.instagram.com/marionville_fbla/'
        - icon: snapchat
          icon_pack: fab
          name: Snapchat
          link: 'example.com'
        - icon: facebook
          icon_pack: fab
          name: Facebook
          link: 'https://www.facebook.com/profile.php?id=100086585220209&mibextid=LQQJ4d'
        - icon: tiktok
          icon_pack: fab
          name: Tiktok
          link: 'https://www.tiktok.com/@marionville.fbla'
      text: |-
        <style>
          /* Styles for the image */
          #transparentImg {
            opacity: 0.4;
            transition: opacity 0.3s ease-in-out;
            cursor: pointer;
          }

          #transparentImg:hover {
            opacity: 1;
          }
        </style>

        <a href="https://docs.google.com/forms/d/e/1FAIpQLScGE2JJ97g_U24mERp4Bp3O8I7armahJ_estqGqus9rC-5pfg/viewform?usp=sf_link" target="_blank">
          <img id="transparentImg" src="https://raw.githubusercontent.com/CodeAPretzel/FBLA-Website/main/assets/media/website-image-christmas-challenge-1.png" alt="Christmas Game!" height=50 width=50>
        </a>
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