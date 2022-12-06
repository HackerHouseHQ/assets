# HHHQ Assets

Various static assets for the HHHQ projects

## Structure

common assets should be in the root folder, then
one folder per project for dedicated data, internally structured as follow

```bash
[project]         # project name
    ├─ [config]  # static configuration objects
    ├─ fonts      # fonts and such for that specific project
    ├─ ...        # any other organization
    └─ images     # specific images for the project
```

### Landing page

```bash
landing-page
  ├─ config       # json with the landing page configurations
  ├─ fonts        # dedicated landing page fonts
  ├─ images       # Common images
  └─ pictures     # team pictures
```

## Images

Some files projects have already be structured as

```bash
(image_name[_number])[-size][-variant].(jpg|png|...)
```

or with a different order

```bash
(image_name[_number])[-variant][-size].(jpg|png|...)
```

where

- `image_name` is the actual file name, with the optional
  - `_number`: progressive id to differentiate them
- `variant` can be `default`, `white`, `black`, `transparent` (mostly)...
- `size` defines the size variation in pixels `WxH`

> As a general rule, *sections* of the name are split by a `-`, internal spacing
> uses a `_`

Examples would be

```bash
logo_01-transparent-64x64.png
john_doe_avatar_01-1218x128.png   # would be used as default if necessary
john_doe_avatar_01-default-1218x128.png
john_doe_avatar_01-white-1218x128.png
john_doe_avatar_01-transparent-1218x128.png
```

### Logos

Contains the logos of the businesses, one folder for each business. naming of the
files can be whatever we want, but over time it would be nice to have them
all follow the same convention.
