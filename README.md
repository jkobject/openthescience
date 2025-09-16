# Open the Science - Static Website

A Jekyll-based static website for the Open Science Publishing Club.

## Features

- Jekyll static site generator with minimal-mistakes theme
- Open science publishing platform for research briefs
- Community-driven peer review system
- Auto-deployment via GitHub Actions
- Fully responsive design

## Site Structure

- **Home Page**: Welcome and overview of the platform
- **About**: Mission and values of the open science movement
- **Research Briefs**: Collection of published research papers
- **Reviewers Club**: Information about joining the peer review community
- **Community**: How to get involved and connect with others
- **FAQ**: Frequently asked questions

## Development

### Local Setup

1. Install Ruby and Bundler
2. Clone this repository
3. Run `bundle install`
4. Run `bundle exec jekyll serve`
5. Visit `http://localhost:4000`

### Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

### Publishing Research Briefs

Research briefs should be added to the `_research-briefs` directory with the following front matter:

```yaml
---
title: "Your Research Title"
date: YYYY-MM-DD
authors: "Author Name(s)"
categories: ["Category1", "Category2"]
excerpt: "Brief description of your research"
layout: single
---
```

## Deployment

The site automatically deploys to GitHub Pages when changes are pushed to the main branch via GitHub Actions.

## License

This project is released under the Public Domain (Unlicense). See [LICENSE](LICENSE) for details.

## Hashtag

#OTS #OpenTheScience #openpub
