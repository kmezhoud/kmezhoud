---
# An instance of the Portfolio widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: portfolio

# This file represents a page section.
headless: true

active: true

# Order that this section appears on the page.
weight: 30

title: Projects
subtitle: ''

content:
  # Page type to display. E.g. project.
  page_type: project

  # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
  filter_default: 0

  # Filter toolbar (optional).
  # Add or remove as many filters (`filter_button` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove the toolbar, delete the entire `filter_button` block.
  filter_button:
  - name: All
    tag: '*'
  - name: EDA
    tag: eda
  - name: R
    tag: r
  - name: Python
    tag: python
  - name: Pharma
    tag: pharma
  - name: Image
    tag: image
  - name: Forcast
    tag: forcast
  - name: Business
    tag: business
  - name: Dashboard
    tag: dashboard
  - name: Mobile
    tag: mobile
  - name: Shiny
    tag: Shiny
  - name: Shinyproxy
    tag: Shinyproxy
  - name: Docker
    tag: Docker
  - name: Cloudflare
    tag: Cloudflare
  - name: Auth0
    tag: Auth0
  - name: Digital Ocean
    tag: Digital Ocean

design:
  # Choose how many columns the section has. Valid values: '1' or '2'.
  columns: '3'

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   5 = Showcase
  view: 3

  # For Showcase view, flip alternate rows?
  flip_alt_rows: false
---
