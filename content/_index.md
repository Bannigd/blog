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
      text: Стариков Данила Андреевич является студентом первого курса факультета физико-математических и естественных наук Российского университета дружбы народов, и также работает на кафедре прикладной информатики и теории вероятностей Российского университета дружбы народов. Научные интересы - математическое моделирование волноводных структур.
      
  - block: markdown
    id: section-1
    content:
      title: Интересы
      subtitle:
      text: |2-
        * Математическое моделирование
        * LaTeX
        * Конструкторские решения болидов Формулы-1
    design:
      columns: '2'
  - block: features
    content:
      title: Навыки
      items:
        - name: Python
          icon: python
          icon_pack: fab
        - name: Maple
          icon: mapleCAS
          icon_pack: custom
        - name: LaTeX
          icon: LaTeX
          icon_pack: custom
  - block: experience
    content:
      title: Образование
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Российский универститет дружбы народов
          company: бакалавриат
          company_url: ''
          company_logo: school
          location:
          date_start: '2022-09-01'
          date_end: ''
          description: "Направление: 09.03.03 Прикладная информатика"
       
    design:
      columns: '1'
      
  - block: experience
    content:
      title: Опыт
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Составление научно-технических отчетов
          company: самозанятость
          date_start: '2022-05-01'
          date_end: ''
          description: |2-
              Обязанности:

              * Редактура текста
              * Написание введения и заключения
              * Подготовка текста в соответствие с ГОСТ 7.32: оглавление, автоматическая нумерация рисунков, таблиц и тд.
              * Объем текста в одном проекте от 30 до 230 страниц (средний объем 70-80 стр.)

    design:
      columns: '2'

  - block: collection
    id: posts
    content:
      title: Последние посты
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
      email: 1132226531@pfur.ru
      #phone: 888 888 88 88
     # appointment_url: 'https://calendly.com'
      
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
