# Liquid Glass Theme

[![Validations](https://github.com/cristian-rincon/homeassistant-liquid-glass-theme/actions/workflows/validate.yml/badge.svg)](https://github.com/cristian-rincon/homeassistant-liquid-glass-theme/actions/workflows/validate.yml)

Theme inspired by Liquid Glass for Home Assistant with automatic dark mode support.

[![Demo day](assets/bd-day.png)](assets/bd-day.png)
[![Demo night](assets/bd-night.png)](assets/bd-night.png)


## Installation

1. You can install the theme with [HACS](https://hacs.xyz/docs/setup/download):

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=cristian-rincon&repository=homeassistant-liquid-glass-theme&category=theme)

> [!NOTE]  
> The background blur effects require Home Assistant 2025.5

2. You should see the "liquid-glass" theme appear in your list of themes.

If it's missing, try reloading your themes or adding the following code to your `configuration.yaml` file (reboot required):

```yaml
frontend:
  themes: !include_dir_merge_named themes
```

3. (Optional) You can set this as the default theme with the following automation:
```
alias: Frontend - Change theme
trigger:
  - platform: homeassistant
    event: start
action:
  - service: frontend.set_theme
    data:
      name: liquid-glass
```

## Remarks

- Based on [homeassistant-visionos-theme](https://github.com/Nezz/homeassistant-visionos-theme)
- Photo by <a href="https://unsplash.com/@3dottawa?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Point3D Commercial Imaging Ltd.</a> on <a href="https://unsplash.com/photos/white-wooden-framed-glass-door-nQlVMCHPysY?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
      