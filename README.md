![Cloudflare](https://asset.brandfetch.io/idJ3Cg8ymG/idN3oIY8Ao.svg)
# Custom Vanity Pages
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

Once you have customized a template page within your own repo to your organization's brand needs, you'll set it on Cloudflare's end. 

When you set a "Custom Page" on Cloudflare, Cloudflare pulls inline the HTML, CSS, and JS of the page you provide - as long as all required items return `200 **OK**` on page-set.

To set a page, go to the page in your GitHub repository that you'd like to set, for example in our case, [ipcountryblock.html](https://github.com/BeeHiveCyberSecurity/CloudflareVanityPages/blob/main/modern/ipcountryblock.html). Then, click "Raw" located on the top right of your file's border/button/area/thing.

![GIF](https://i.imgur.com/S18eybv.gif)

Now, copy the URL shown at the top of your screen. For this example, ours is 

```https://raw.githubusercontent.com/BeeHiveCyberSecurity/CloudflareVanityPages/main/modern/ipcountryblock.html```

Now, go to "Custom Pages" under any website in your Cloudflare repertoire that is on a Pro+ plan.

![IMG](https://i.imgur.com/N1SVxle.png)

In this example, we're intending to set the appropriately named "IP/Country Block" page. Using the link we just prior copied from GitHub, we'll set the page in Cloudflare Custom Pages.

![IMG](https://i.imgur.com/NI3bJY3.png)

Click publish, and you're done! If you'd like, you can even click "Preview" to test that your page is showing correctly. 

**It's important to remember that Cloudflare will not actively update your page when you make changes to it! You will need to go in and remove and re-set your page for new changes to be pulled down by Cloudflare and shown to visitors.**