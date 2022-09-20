# This repo is ARCHIVED.  Latest is now here:
https://github.com/home-assistant-community-themes/matrix-reloaded

<br />
<br />
<br />
<br />


# Matrix Reloaded Theme

[![Build Status](https://github.com/home-assistant-community-themes/template/workflows/.github/workflows/workflow.yml/badge.svg)](https://github.com/home-assistant-community-themes/template/actions)
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/custom-components/hacs)


This looks great with a Matrix "Code rain" motion background.  If you place a motion gif in the following location,  this theme will pick it up:

```
config_dir/www/backgrounds/matrix-code-rain.motion.gif
```

(Where "config_dir" is your Home Assistant config directory.  Some installs this might be /config, and some others /usr/share/hassio/homeassistant)


The "themes" directory of this repo contains a matrix-code-rain.motion.gif that you can move to the above location.

Installation instructions are at the bottom of this page.
**NOT** yet available in HACS
  
## Screenshots

### Overview

![Theme - Overview](./docs/theme-overview.gif)

### Pop-ups

![Theme - Pop-ups](./docs/theme-popup.png)

### Logbook

![Theme - Logbook](./docs/theme-logbook.png)

### History

![Theme - History](./docs/theme-history.png)

### Developer Tools

![Theme - Developer Tools](./docs/theme-developer-tools.png)

### Add-on's

![Theme - Configuration](./docs/theme-addons.png)

### Profile

![Theme - Profile](./docs/theme-profile.png)

## Installation

Add the following code to your `configuration.yaml` file (reboot required).

```yaml
frontend:
  ... # your configuration.
  themes: !include_dir_merge_named themes
  ... # your configuration.
```

Then get the theme into your themes directory using one of the following steps.  After that, either call the reload themes service, or restart your HA system.

### HACS

** NOT AVAILABLE YET **
1. Go to the Community Store.
2. Search for `Matrix Reloaded`.
3. Navigate to the theme.
4. Press `Install`.

### Manual with github

Clone this repository in your existing (or create it) `themes/` folder.

```bash
cd themes/
git clone https://github.com/mrand/matrix_reloaded.git
```

Or using submodules:

```bash
cd themes/
git submodule add https://github.com/mrand/matrix_reloaded.git
```

### Manual without github
```
wget https://raw.githubusercontent.com/mrand/matrix_reloaded/master/themes/matrix_reloaded.yaml
```

-or-

Go to https://raw.githubusercontent.com/mrand/matrix_reloaded/master/themes/matrix_reloaded.yaml and copy and paste it to a file in your themes directory

