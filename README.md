# Local Business Directory
> Find it all under one roof

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Resources & Support](#resources--support)

## Overview
Local Business Directory is a responsive web directory featuring a clean, 3-column grid layout designed to showcase local businesses and services. The platform offers easy navigation through categories and provides a seamless experience for both visitors and administrators.

## Features
- Responsive 3-column grid layout
- Category-based filtering
- Search functionality
- Mobile-friendly design
- SEO-optimized structure
- Custom category labels
- Easy-to-update directory listings

## Getting Started

### Prerequisites
- Text editor (VS Code recommended)
- Basic knowledge of HTML/CSS
- Web hosting account

### Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/local-business-directory.git
```

2. Navigate to project directory:
```bash
cd local-business-directory
```

3. Open `index.html` in your browser to view locally

## Directory Structure
```
local-business-directory/
├── index.html
├── assets/
│   ├── css/
│   │   ├── style.css
│   │   └── responsive.css
│   ├── js/
│   │   └── main.js
│   └── images/
├── listings/
│   └── data.json
└── categories/
    └── categories.json
```

## Customization Guide

### Adding Directory Items
1. Open `listings/data.json`
2. Add new listing using the following format:
```json
{
  "id": "unique-id",
  "name": "Business Name",
  "category": "Category",
  "description": "Business description",
  "contact": {
    "phone": "123-456-7890",
    "email": "business@example.com",
    "website": "https://example.com"
  }
}
```

### Modifying Category Labels
1. Navigate to `categories/categories.json`
2. Edit or add categories:
```json
{
  "categories": [
    {
      "id": "category-id",
      "name": "Category Name",
      "slug": "category-slug"
    }
  ]
}
```

### Updating Hero Section
1. Open `index.html`
2. Locate the hero section:
```html
<section class="hero">
  <h1>Your Custom Title</h1>
  <p>Your custom description</p>
</section>
```

### Customizing Colors
1. Open `assets/css/style.css`
2. Modify the root variables:
```css
:root {
  --primary-color: #your-color;
  --secondary-color: #your-color;
  --text-color: #your-color;
}
```

## Deployment

### Standard Deployment
1. Upload all files to your hosting server
2. Ensure proper file permissions (typically 644 for files, 755 for directories)
3. Access your website through the domain

### GitHub Pages Deployment
1. Go to repository settings
2. Navigate to "Pages" section
3. Select main branch as source
4. Save changes

## Custom Domain Setup

### Using Your Own Domain
1. Add domain in hosting control panel
2. Update nameservers or DNS records
3. Configure A records:
```
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
```

### SSL Configuration
1. Enable SSL in hosting panel
2. Update internal links to HTTPS
3. Implement forced HTTPS redirect

## Troubleshooting

### Common Issues
- **Images not loading**: Check file paths and permissions
- **Categories not filtering**: Verify category IDs match in both JSON files
- **Responsive layout issues**: Clear browser cache and check media queries
- **Search not working**: Ensure JavaScript is enabled and properly loaded

### Debug Mode
Add `?debug=true` to URL to enable console logging

## Resources & Support

### Documentation
- [Full Documentation](docs/full-documentation.md)
- [API Reference](docs/api-reference.md)
- [Customization Guide](docs/customization.md)

### Support Channels
- GitHub Issues
- Email Support: support@example.com
- Community Forum: [Link to Forum]

### Updates and Maintenance
- Check for updates monthly
- Backup data before major changes
- Test in staging environment first

---

© 2024 Local Business Directory. All rights reserved.