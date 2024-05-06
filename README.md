# ![Cloudflare](https://asset.brandfetch.io/idJ3Cg8ymG/idN3oIY8Ao.svg) Customizable Vanity Pages
Customized variants of block and security check pages for users of Cloudflare's WAF.

## Overview
Cloudflare uses a wide range of error codes to identify issues in handling request traffic. By default, these error pages mention Cloudflare; however, custom error pages help you provide a consistent brand experience for your users. 

If you are on the Pro, Business, or Enterprise plan you can customize and brand these pages for your whole account or for specific domains. You can design custom error pages to appear during a security challenge or when an error occurs.

`500`, `501`, `503`, and `505` responses do **not** trigger custom error pages to avoid breaking specific API endpoints and other web applications.

Alternatively, Enterprise customers can customize `5XX` error pages at their origin via "Enable Origin Error Pages" in the "Custom Pages" app in the dashboard.

> Enable Origin Error Pages excludes errors 520 to 527.

# How to use these
Like our WAF-IPDB tool for Cloudflare - this is a template repo. 

**First**. [clone this repository by clicking here while signed into a GitHub account](https://github.com/new?template_name=CloudflareVanityPages&template_owner=BeeHiveCyberSecurity).

Then, pull down and begin customizing your pages in any proper development software. 
Notepad++ works, Cursor works, Visual Studio Code works.

Each template has different aspects that are customizable according to your branding. The primary items you'll want to focus on when customizing each individual page template, is
- Brand colors
- Brand logo (if selected)
- Font selection
- Page background coloring
