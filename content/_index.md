---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: features
    content:
      title: Skills
      items:
        - name: R
          description: 90%
          icon: r-project
          icon_pack: fab
        - name: Python
          description: 100%
          icon: python
          icon_pack: fab
        - name: Stata
          description: 10%
          icon: camera-retro
          icon_pack: fas
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
        - title: Postdoctoral Researcher
          company: UC Berkeley, Institute of Governmental Studies
          company_url: ''
          company_logo: org-gc
          location: Berkeley, CA
          date_start: '2023-07-01'
          date_end: ''
          description: |2-
              Responsibilities include:
              
              * Clean and process big data in R and Python
              * Grant writing
              * Conduct analyses using causal inference and machine learning techniques
              * Develop, write, and publish peer-reviewed academic papers
              
        - title: City Research Scientist
          company:  NYC Department of Housing Preservation and Development
          company_url: ''
          company_logo: org-gc
          location: New York City, NY
          date_start: '2022-09-01'
          date_end: '2023-05-31'
          description: |2-
              Responsibilities include:

              * Design, manage, and execute research project with other HPD research
              * Create Stata documentation of previous analyses to promote replication
              * Develop internal and public-facing reports, data products, and research documentation
              * Present and field questions on research findings to internal and external audiences
              * Clean, process, and  data products to the US Census
              * Update NYCHVS survey methodology documentation
              * Develop post-stratification weights
              
        - title: Research Associate
          company: Professor Van Tran
          company_url: ''
          company_logo: org2-gc
          location: New York City, NY
          date_start: '2021-09-01'
          date_end: '2022-09-01'
          description: |2-
              Responsibilities include:
          
              * Construct US Census dataset to study ethno-racial neighborhood integration in metro New York
              * Fit multinomial logistic regression models and interpreted marginal effects plots in R for analyses
              * Write methodological section, create descriptive plots in R, and manage project development on GitHub
    design:
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
        - name: Superdiversity 
          tag: Superdiversity
        - name: Housing Literacy
          tag: Housing Literacy
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
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
---
