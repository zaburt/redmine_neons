# Neons

A cyberpunk neon theme for Redmine, inspired by glowing cityscape color
palettes — deep near-black backgrounds with electric cyan, magenta and
purple accents.

## Installation

1. Clone this theme ([https://github.com/zaburt/redmine_neons](https://github.com/zaburt/redmine_neons)) into the Redmine `themes/`
   directory at the application root (Redmine 7+) as `neons`:

   ```
   git clone https://github.com/zaburt/redmine_neons.git themes/neons
   ```

   The result should contain:

   ```
   themes/neons/stylesheets/application.css
   ```

   > Note: Redmine 6 and earlier used `public/themes/` instead of `themes/`.

2. Restart Redmine so the new theme appears in the list of available themes.
   In production, precompile assets so the theme CSS/images are served:

   ```
   RAILS_ENV=production bin/rails assets:precompile
   ```

3. Go to `Administration -> Settings -> Display` and select "Neons" in the
   "Theme" drop-down list. Save your settings.

Redmine should now be displayed using the `neons` theme.

## Customize

1. You can change `images/logo.svg` to update the header/login logo, and
   `favicon/favicon.svg` to update the browser tab icon.
2. If you don't want to use a logo in the header, you can remove the
   `#header > h1` styles in `stylesheets/application.css`.
3. The full neon color palette is defined inline as hex values throughout
   `stylesheets/application.css`:

   | Role               | Color     |
   |--------------------|-----------|
   | Page background    | `#07050D` |
   | Panel / box bg     | `#17102A` |
   | Text               | `#E6E4FF` |
   | Muted text         | `#9A8FC4` |
   | Primary accent     | `#00F0FF` (cyan) |
   | Secondary accent   | `#FF2BD6` (magenta) |
   | Tertiary accent    | `#B967FF` (purple) |
   | Success            | `#39FF8F` |
   | Error              | `#FF3366` |
   | Warning            | `#FFE066` |

4. In production, re-run `assets:precompile` after editing any theme file.

## License

Licensed under [GNU GPLv2](LICENSE).

Copyright (c) 2026 Onur Küçük (onur [at] delipenguen.net)
