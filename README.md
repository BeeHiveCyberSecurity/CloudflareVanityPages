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

To initiate the customization process, [clone the repository by clicking on this link while logged into your GitHub account](https://github.com/new?template_name=CloudflareVanityPages&template_owner=BeeHiveCyberSecurity).

After cloning, proceed to download the repository and commence the customization of your pages using an appropriate development environment. Suitable software includes Notepad++, Cursor, and Visual Studio Code.

Each template offers various customizable elements to align with your brand identity. Focus on the following key aspects when personalizing each page template:
- Brand colors
- Brand logo (if applicable)
- Typography choices
- Background color of the page

The templates are initially configured with our branding. You will need to locate and modify our branding elements, such as colors, URLs, and language, to reflect your brand. For example, change "Back to BeeHive" to "Back to [Your Business Name]" and update the URL to your business's website.

Once you have tailored a template to your organization's branding within your repository, the subsequent step is to implement it on Cloudflare.

Cloudflare will integrate the HTML, CSS, and JavaScript from your custom page, assuming all components are accessible and return a `200 OK` status upon setup.

To set up a custom page, navigate to the desired page within your GitHub repository. For instance, consider the [ipcountryblock.html](https://github.com/BeeHiveCyberSecurity/CloudflareVanityPages/blob/main/modern/ipcountryblock.html) page. Click on the "Raw" button, located at the top right corner of the file viewer.

![GIF](https://i.imgur.com/S18eybv.gif)

Now, copy the URL shown at the top of your screen. For this example, ours is 

```https://raw.githubusercontent.com/BeeHiveCyberSecurity/CloudflareVanityPages/main/modern/ipcountryblock.html```

Now, go to "Custom Pages" under any website in your Cloudflare repertoire that is on a Pro+ plan.

![IMG](https://i.imgur.com/N1SVxle.png)

In this example, we're intending to set the appropriately named "IP/Country Block" page. Using the link we just prior copied from GitHub, we'll set the page in Cloudflare Custom Pages.

![IMG](https://i.imgur.com/NI3bJY3.png)

Click publish, and you're done! If you'd like, you can even click "Preview" to test that your page is showing correctly. 

**It's important to remember that Cloudflare will not actively update your page when you make changes to it! You will need to go in and remove and re-set your page for new changes to be pulled down by Cloudflare and shown to visitors.**
