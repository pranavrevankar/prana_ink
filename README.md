# Pranav Revankar - Personal Website

A minimalistic, elegant one-page personal website showcasing projects, side hustles, and thoughts.

## Features

- **Clean Design**: Minimalistic layout inspired by modern personal websites
- **Filtering System**: Interactive tag-based filtering for different content categories
- **Blog Integration**: Individual blog posts with shared commenting system
- **Mobile Responsive**: Optimized for both desktop and mobile viewing
- **No Dependencies**: Uses TailwindCSS via CDN for styling

## Content Categories

- **Projects**: Technical projects and tools I've built
- **Side Hustles**: Business ventures and entrepreneurial experiments
- **Other**: Personal updates, thoughts, and miscellaneous content

## Blog System

- Individual blog post pages with rich content
- JSONBin-powered comment system for visitor interaction
- No authentication required - simple name + comment approach

## File Structure

```
├── index.html              # Main homepage with filtering
├── blog-2025-09-01.html    # Individual blog post
├── assets/                 # Static assets (images, documents)
└── README.md               # This file
```

## Setup for Comments

To enable the shared comment system:

1. Create a free account at [JSONBin.io](https://jsonbin.io)
2. Create a new bin with initial data: `{"comments": []}`
3. Generate an API key with read/write permissions
4. Update the `binId` and `apiKey` in `blog-2025-09-01.html`

## Adding New Content

### Adding a Project/Side Hustle

1. Copy an existing `<article>` block in `index.html`
2. Update the link, title, and description
3. Set appropriate `data-tags` for filtering
4. Add corresponding tag styles if needed

### Adding a New Blog Post

1. Copy `blog-2025-09-01.html` to a new filename
2. Update the content, title, and metadata
3. Link to it from the main page
4. Each blog post gets its own comment section

## Technology Stack

- **HTML5**: Semantic markup
- **TailwindCSS**: Utility-first styling via CDN
- **Vanilla JavaScript**: Filtering and comment functionality
- **JSONBin API**: Shared comment storage

## License

Personal project - All rights reserved.