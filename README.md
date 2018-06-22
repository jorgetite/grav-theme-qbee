# QBoss - Grav Theme

QBoss is a clean, lightweight and minimal HTML 5 theme for [Grav](https://getgrav.org) built with the [Kube](https://imperavi.com/kube/) CSS &amp; JS Framework.

## Features
* Clean and minimal
* Responsive and mobile friendly
* Lightweight and fast loading
* Clean typography
* Search engine optimized
* Modern browser compatible
* Very extensible and customizable
* HTML5, CSS3, JavaScript

### Supported Page Templates

* Default view template `default.md`
* Error view template `error.md`
* Modular view templates: `modular.md`
    + Splash Modular view template `splash.md`
    + Profile Modular view template `profile.md`
    + Features Modular view template `features.md`
    + Hero Modular view template `hero.md`
    + Text Modular view template `text.md`

### Supported Browsers
QBoss supports the latest, stable releases of all major browsers:

- Latest Chrome
- Latest Firefox
- Latest Safari
- Latest Opera
- Microsoft Edge
- Internet Explorer 11

## Installation

Installing the QBoss theme can be done in one of two ways:

- The GPM (Grav Package Manager) installation method enables you to quickly and easily install the theme with a simple terminal command
- The manual method enables you to do so via a zip file.

### GPM Installation (Preferred)

The simplest way to install this theme is via the Grav Package Manager (GPM) through your system's Terminal (also called the command line). From the root of your Grav install type:

```Shell
bin/gpm install qboss
```

This will install the QBoss theme into your `/user/themes` directory within Grav. Its files can be found under `/your/site/grav/user/themes/qboss`.

### Manual Installation

To install this theme, just download the zip version of this repository and unzip it under `/your/site/grav/user/themes`. Then, rename the folder to `qboss`. You can find these files either on [GitHub](https://github.com/jorgetite/QBoss) or via [GetGrav.org](http://getgrav.org/downloads/themes).

You should now have all the theme files under

```Shell
/your/site/grav/user/themes/qboss
```

### Requirements

* Grav 1.4+

## Theme Options

QBoss allows you to set the following options site-wide:

```yaml
enabled: true               # Enable the theme
production_mode: true       # Whether CSS and JS files are minimized (true), or not
header_sticky: false        # Keeps the header sticky at the top of the page
menu_style: menu-links      # Controls how menu items are rendered
show_site_name: 1           # Displays or not the site name in the header
show_site_logo: 1           # Displays or not the site logo in the header
site_logo:                  # The relative path to the site logo, defaults to 'images/logo.png'
site_copy:                  # The copyright notice displayed in the site footer
```

To make modifications, you can copy the `user/themes/qboss/qboss.yaml` file to `user/config/themes/` folder and modify, or you can use the admin plugin.

> NOTE: Do not modify the `user/themes/qboss/qboss.yaml` file directly or your changes will be lost with any updates

### Page Options

QBoss provides several options in the page frontmatter to fine control how pages are displayed and styled. These options are divide in the following three categories:

#### Layout Settings

```yaml
subtitle: ''                # The page subheading
show_header: true      # Whether the site header is displayed or not for this page

```

## License
The files contained in this project are released under the MIT License. You can
find a copy of this license in LICENSE.txt file.
