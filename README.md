# Jekyll files for <https://floraconnections.com>

## Notes about site structure

1. The index page uses the layout `_layouts/splash.html`. All others use `_layouts/one-column.html`. 

2. Layouts are sandwiched between `_includes/header.html` and `_includes/footer.html`.

3. `_includes/card_code.html` contains every taxon card in the Priority Species List. It gets included in `priority-plants.md`, which contains the MixItUp interface for users to filter the cards by state/territory, and the blurb text about what this list is about. The two are separated for easier maintenance of the taxon cards only.

4. The site is styled by three non-overlapping stylesheets. `_assets/css/structure.css` handles alignment and flow of block-level elements to control the layout of the page. `_assets/css/aesthetic.css` styles elements for visual appeal (text display, borders, whitespacing). `_assets/css/mixitup.css` styles the MixItUp elements that appear in the Priority Plants List.

5. The contact form is handled externally by Cognito Forms (has anti-spam and anti-bot safeguards that ideally are never even shown to human users).


## Deployment info

TODO: Update with instructions about updating this with ALA's framework.

For building locally on Windows, ensure Jekyll is installed and in PATH, then run `_build_site.bat`.
