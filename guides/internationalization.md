# Internationalization

All of our guest facing text gets translated into multiple languages using a library called `i18n-next`. You're responsible only for adding the english language translation in `i18n/en.js`, and using the `i18n.t("somePage.key")` in your components and helper functions.

The translation strings in `i18n/en.js` are grouped by component. The names top level keys mirror the name of the component they are used in.