# dkrichards Theme

A clean, minimal Hugo theme for Micro.blog, converted from Jekyll.

## Features

- Responsive design
- Pagination support
- RSS feeds
- Microformats (h-card, h-entry) for IndieWeb compatibility
- Support for title-less microblog posts
- Tag and category taxonomy support
- Clean, readable typography

## Installation

Add this theme to your Hugo site's `themes` directory or configure it in your `hugo.toml`:

```toml
theme = "dkrichards-theme"
```

## Configuration

Example `hugo.toml` configuration:

```toml
baseURL = "https://example.com"
languageCode = "en-us"
title = "Your Name"
theme = "dkrichards-theme"

paginate = 8
timeZone = "America/New_York"

[params]
  description = "Your bio/description here"
  author = "Your Name"
  defaultImage = "/assets/images/profile.jpg"

[params.social]
  github = "yourusername"
  linkedin = "yourusername"

[outputs]
  home = ["HTML", "RSS"]
  section = ["HTML", "RSS"]

[outputFormats.RSS]
  mediaType = "application/rss+xml"
  baseName = "feed"

[taxonomies]
  tag = "tags"
  category = "categories"
```

## Micro.blog Compatibility

This theme is designed to work seamlessly with Micro.blog:

- Supports posts with and without titles
- Custom RSS feed format
- Microformats markup for proper feed parsing
- IndieWeb-friendly markup

## License

MIT License - See LICENSE file for details.
