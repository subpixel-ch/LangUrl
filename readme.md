# Language URL for Statamic 2

## Usage:
Intended to help build a language toggle for Statamic 2. For example, in a English and French site where English is the default language, you can use `{{ lang_url locale="fr" }}`  and `{{ lang_url locale="default" }}` in your templates to easily switch languages of the current page:
```
{{ if locale == "en" }}
  <a href='{{ lang_url locale="fr" }}'>Français</a>
{{/if}

{{ if locale == "fr" }}
  <a href='{{ lang_url locale="default" }}'>English</a>
{{/if}
```
## To Do:
 - Detect the default language instead of requiring "default" as the locale parameter.
 - Do not hardcode `en` as default locale