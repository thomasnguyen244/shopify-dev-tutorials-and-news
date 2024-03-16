# Shopify Developer Tutorials and News
List of shopify frontend/backend developer tutorials and news

# I. Shopify theme develop tutorial
*Build Shopify themes*
Themes shape the online store experience for merchants and their customers. Build fast, flexible themes at scale using Liquid, Shopify's theme templating language, along with HTML, CSS, JavaScript, and JSON.

## SECTION 1. Theme architecture
A theme controls the organization, features, and style of a merchant's online store. Theme code is organized with a standard directory structure of files specific to Shopify themes, as well as supporting assets such as images, stylesheets, and scripts. To learn how themes fit into Shopify, and learn how to set up an environment to build and test themes, refer to the Shopify themes overview.

### Theme files fall into the following general categories
- *Markup and features* - These files control the layout and functionality of a theme. They use Liquid to generate the HTML markup that makes up the pages of the merchant's online store.
- *Supporting assets* - These files are assets, scripts, or locale files that are either called or consumed by other files in the theme.
- *Config files* - These files use JSON to store configuration data that can be customized by merchants using the theme editor.
  
```
Shopify theme directory structure
.
├── assets
├── config
├── layout
├── locales
├── sections
├── snippets
└── templates
    └── customers
```

*assets:* The assets directory contains all of the assets used in a theme, including image, CSS, and JavaScript files.
*config:* The config directory contains the config files for a theme. Config files define settings in the Theme settings area of the theme editor, as well as store their values.
*layout:* The layout directory contains the layout files for a theme, through which template files are rendered.
*locales:* The locales directory contains the locale files for a theme, which are used to provide translated content.
*sections:* The sections directory contains a theme’s sections and section groups.
*snippets:* The snippets directory contains Liquid files that host smaller reusable snippets of code. You can reference these snippets throughout the theme with the Liquid render tag.
*templates:* The templates directory contains a theme’s template files, which control what's rendered on each type of page.

## SECTION 2. Build a new theme
*In this tutorial, you'll use Shopify CLI and Dawn to create a new theme and upload it to Shopify.*

### What you'll learn
- Set up your local development environment
- Cloned [Dawn](https://shopify.dev/docs/themes/tools/dawn), Shopify's reference theme
- Previewed changes made to your local code
- Pushed theme code to your Shopify store and published your theme

Link: https://shopify.dev/docs/themes/getting-started/create
  
## SECTION 3. Custom the theme
*As a theme developer, you can customize themes for Shopify merchants. These customizations might range from small tweaks to complete redesigns*

### What you'll learn
- Gained access to the merchant's store
- Set up your local development environment
- Downloaded a copy of the merchant's theme
- Made a change and previewed it
- Shared your changes with the merchant
- Published your changes

Link: https://shopify.dev/docs/themes/getting-started/customize

## SECTION 4. Liquid reference
*Liquid is a template language created by Shopify. It's available as an open source project on GitHub, and is used by many different software projects and companies.*
This reference documents the Liquid tags, filters, and objects that you can use to build Shopify Themes.

Link: https://shopify.dev/docs/api/liquid

## SECTION 5. Ajax API
*The Ajax API provides a suite of lightweight REST API endpoints for development of Shopify themes.*

### Use cases
Possible uses of the Ajax API include:
- Add products to the cart and update the cart item counter.
- Display related product recommendations.
- Suggest products and collections to visitors as they type in a search field.
  
Link: https://shopify.dev/docs/api/ajax

## SECION 6. Tools for building Shopify themes
*Shopify provides a range of tools to help you build Shopify themes faster.*

- Tools for building and editing themes
- Legacy tools
- Web-based editors for themes
- Access tools
- Version control tools
- Testing tools
- Tools for learning Liquid

Link: https://shopify.dev/docs/themes/tools#access-tools

## SECTION 7. Example theme Dawn
*Dawn is Shopify's reference theme, which is built for performance, flexibility, and ease of use. It uses Online Store 2.0 features, including JSON templates, which support app blocks and sections on all pages. Dawn is used as the basis of all free Shopify themes.*

Link: https://shopify.dev/docs/themes/tools/dawn

# II. Build Shopify App
*Build the best commerce apps*
It's never been easier to create high-quality apps that look, feel, and perform like they’re part of Shopify. Quickly build performant apps with our updated CLI, optimized APIs, and App Design Guidelines.
In this tutorial, you'll create an app that users can access in the Shopify admin. You'll generate starter code and use Shopify CLI to develop your app.

Link: https://shopify.dev/docs/apps/getting-started/create

## What you'll learn
- Initialize a Remix app that uses Shopify CLI
- Install your app on a development store
- Generate a product using your new app

## Requirements
- You've created a Partner account and a development store.
- You've installed Node.js 18 or higher.
- You've installed a Node.js package manager: either npm, Yarn 1.x, or pnpm.
- You've installed Git 2.28.0 or higher.
- You're using the latest version of Chrome or Firefox.

## Step 1: Create a new app
*You can create a new Shopify app using an npm, yarn, or pnpm command.*
- Navigate to the directory where you want to create your app. Your app will be created in a new subdirectory.
- Run one of the following commands to create a new app: ``npm init @shopify/app@latest`` or ``yarn create @shopify/app``
- When prompted, enter a name for your app, and then select Start with Remix to use the [Remix template](https://github.com/Shopify/shopify-app-template-remix)

## Step 2: Start a local development server
*After your app is created, you can work with using a local development server and the [Shopify CLI](https://shopify.dev/docs/apps/tools/cli).*
Shopify CLI uses [Cloudflare](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/do-more-with-tunnels/trycloudflare/) to create a tunnel that enables your app to be accessed using a HTTPS URL.
- Navigate to your newly created app directory. ``cd my-new-app``
- Run the following command to start a local server for your app: ``npm run dev`` or ``yarn dev``
- Shopify CLI guides you through the following tasks:
- + Logging into your [Partner account](https://help.shopify.com/partners/about?shpxid=4587ddf3-F4FD-4153-64DC-6319D92E6280) and selecting a Partner organization
- + Creating an app in the Partner Dashboard, and connecting your local code to the app
- + Creating your [Prisma SQLite database](https://github.com/Shopify/shopify-app-template-remix#application-storage)
- + Creating a tunnel between your local machine and the development store

## Step 3: Install your app on your development store
*You can install your app on your development store, and automatically populate your development store with products that you can use for app testing.*
- With the server running, press p to open your app's preview URL in a browser.
When you open the URL, you're prompted to install the app on your development store.
- Click Install app to install the app on the development store.
You now have a development store running with your new app installed:
- From the home page of the new app, click Generate a product to create a product for your development store.

  
# Build a Shopify app using Remix
*After you create an app, you can add your own functionality to pages inside and outside of the Shopify admin.*

Link: https://shopify.dev/docs/apps/getting-started/build-qr-code-app?framework=remix

# Submit app to shopify app store
Following the guide: [Crucial guidelines to remember when submitting your Shopify app](https://github.com/thomasnguyen244/shopify-dev-tutorials-and-news)


# FAQs
*Question 1*: How to submit my app for review for approval
*Answer*: To submit your app for review for approval
- Log in to your Partner Dashboard.
- Click Apps.
- Click the name of your app.
- Click Distribution.
- If you haven't selected a distribution method yet, then select Public distribution, and click Confirm.
- Click Create listing or Manage listing.
- Select an existing listing, or click Add translated listing.
- Fill out all the required fields, making sure to follow our listing guidelines.
- Click Preview listing to see what your listing will look like when it's live. Make sure that the content, formatting, and images appear as expected.
- Click Save.
- At the top of the form, click the back button ← to return to the app listing page.
- Click Submit app.
- Check the checkbox to acknowledge that your app meets the submission requirements, then click Submit for review.
- Shopify will notify you by email of updates or things to fix during the process. To make sure that you receive emails from the Shopify review team, adjust your email settings to allow emails from app-submissions@shopify.com and noreply@shopify.com.

*To make sure you receive your review updates and communications, add app-submissions@shopify.com and noreply@shopify.com to your allowed senders list in your email service provider’s settings.
You’ll get a response from us within 7 days of submitting your app.*


# Shopify News
- [Shopify Trends for 2024: Embracing Innovation and Enhancing E-Commerce Success](https://www.linkedin.com/pulse/shopify-trends-2024-embracing-innovation-enhancing-e-commerce-6wiwf/)
- [Shopify Industry News and Trends](https://www.shopify.com/retail/topics/industry-news-trends)
