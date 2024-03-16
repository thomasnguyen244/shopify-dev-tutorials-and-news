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
- Cloned (Dawn)[https://shopify.dev/docs/themes/tools/dawn], Shopify's reference theme
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
## Step 2: Start a local development server
## Step 3: Install your app on your development store

# Build a Shopify app using Remix
*After you create an app, you can add your own functionality to pages inside and outside of the Shopify admin.*

Link: https://shopify.dev/docs/apps/getting-started/build-qr-code-app?framework=remix

# Submit app to shopify app store
Following the guide: [Crucial guidelines to remember when submitting your Shopify app]()


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



