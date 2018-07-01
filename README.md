# QBee - Grav Theme

QBee is a clean, lightweight and minimal HTML 5 theme for [Grav](https://getgrav.org) built with the [Kube](https://imperavi.com/kube/) CSS &amp; JS Framework.

![QBee Theme](https://raw.githubusercontent.com/jorgetite/grav-theme-qbee/master/screenshot.png "QBee Screenshot")

## Features
* Clean and minimal
* Responsive and mobile friendly
* Lightweight and fast loading
* Clean typography
* Search engine optimized
* Modern browser compatible
* Very extensible and customizable
* Kube Framework
* Font Awesome
* HTML5, CSS3, JavaScript

### Supported Browsers
QBee supports the latest, stable releases of all major browsers:

- Latest Chrome
- Latest Firefox
- Latest Safari
- Latest Opera
- Microsoft Edge
- Internet Explorer 11

## Installation

Installing the QBee theme can be done in one of two ways:

- The GPM (Grav Package Manager) installation method enables you to quickly and easily install the theme with a simple terminal command
- The manual method enables you to do so via a zip file.

### GPM Installation (Preferred)

The simplest way to install this theme is via the Grav Package Manager (GPM) through your system's Terminal (also called the command line). From the root of your Grav install type:

```Shell
bin/gpm install qbee
```

This will install the QBee theme into your `/user/themes` directory within Grav. Its files can be found under `/your/site/grav/user/themes/qbee`.

### Manual Installation

To install this theme, just download the zip version of this repository and unzip it under `/your/site/grav/user/themes`. Then, rename the folder to `qbee`. You can find these files either on [GitHub](https://github.com/jorgetite/QBee) or via [GetGrav.org](http://getgrav.org/downloads/themes).

You should now have all the theme files under

```Shell
/your/site/grav/user/themes/qbee
```

### Requirements

* Grav 1.4+

## Theme Options

QBee allows you to set the following options site-wide:

| Setting Name     | Default  | Description 
|------------------|----------|----------------------
| `enabled`        | `true`   | Enables or disables the theme
| `production_mode`| `true`   | Serves CSS and JS files minimized
| `header_sticky`  | `false`  | Keeps the header always visible at the top of the page
| `show_site_name` | `true`   | Displays the site name in the header
| `show_site_logo` | `true`   | Displays the site logo in the header
| `site_logo`      |          | The relative path to the site logo. If no path is specified the them uses by default `images/logo.png`
| `site_copy`      |          | The copyright notice displayed in the footer

To make modifications, you can copy the `user/themes/qbee/qbee.yaml` file to `user/config/themes/` folder and modify, or you can use the admin plugin.

```yaml
enabled: true
production_mode: true
header_sticky: false
show_site_name: true
show_site_logo: true
```

> WARNING: Do not modify the `user/themes/qbee/qbee.yaml` file directly or your changes will be lost with any updates

## Pages

QBee supports the following page templates:

* Default view template `default.md`
* Error view template `error.md`
* Modular view templates: `modular.md`
    + Splash Modular view template `splash.md`
    + Profile Modular view template `profile.md`
    + Features Modular view template `features.md`
    + Hero Modular view template `hero.md`
    + Text Modular view template `text.md`

### Page Options

QBee provides several options in the page frontmatter to fine control how pages are displayed and styled. These options are divide in the following  categories:

#### Content Settings

| Setting Name     | Default  | Description 
|------------------|----------|----------------------
| `subtitle`       |          | The page or module subheading

```yaml
subtitle: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.'
```

#### Layout Settings

| Setting Name     | Default  | Description 
|------------------|----------|----------------------
| `show_header`    | `true`   | Controls whether the site header is displayed or not. This option is available only for top level pages
| `show_footer`    | `true`   | Controls whether the site footer is displayed or not. This option is available only for top level pages
| `show_heading`   | `true`   | Controls whether the title and subtitle are autiomatically displayed at the top of the page, or not
| `onpage_menu`    | `false`  | Renders a on page menu for modular pages

```yaml
show_header: true
show_footer: true
show_heading: true
onpage_menu: false
```

#### Style Settings

| Setting Name     | Default       | Description 
|------------------|---------------|----------------------
| `color_scheme`   | `scheme-light`| Sets the appearance of the page. The following values are available:<br />`scheme-light`: White (default)<br />`scheme-gray-light`: Lightgray<br />`scheme-gray-dark`: Dimgray<br />`scheme-dark`: Black
| `padding`        | `md-pad` | Sets the top and bottom padding of the page. The following values are available:<br /> `no-pad`: No padding<br />`xs-pad`: Smaller (16px)<br />`sm-pad`: Small (32px)<br />`md-pad`: Midium (64px)<br />`lg-pad`: Large (96px)<br />`xl-pad`: Larger (128px)
| `css_classes`    |          | Additional CSS classes space separated.

```yaml
color_scheme: scheme-light
padding: md-pad
css_classes: 'my-css-class'
```

## License
The files contained in this project are released under the MIT License. You can
find a copy of this license in LICENSE.txt file.
