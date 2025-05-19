# Theme Blocks

## Folder structure:
<pre lang="markdown"> 
  └── theme   
      ├── assets  
      ├── blocks  
      │   ├── block-name.liquid  
      ... 
</pre>

## Block schema:
|No.|attributes|example/decription|
|---|----------|------------------|
| 1 |name|block title that's shown in the theme editor|
| 2 |settings|customizeable input settings|
| 3 |blocks|support other app and theme blocks as children|
| 4 |presets|predefined block configurations|
| 5 |tag|HTML element as a wrapper|
| 6 |class|css classes|

### Presets schema Attributes:
|No.|attributes|example/decription|
|---|----------|------------------|
| 1 |name|name displayed in the theme editor|
| 2 |category|Groups related presets together|
| 3 |settings|Default values for settings|
| 4 |blocks|Default blocks included in the preset|

## Accessing block settings: 
-- [block object](https://shopify.dev/docs/api/liquid/objects/block#block-settings)

## How to render:

### All Theme blocks
``` liquid
/sections/section.liquid

{% content_for 'blocks' %}

{% schema %}
{
  "name": "Section",
  "blocks": [{"type": "@theme"}]
}
{% endschema %}
```

### specific theme blocks:













# Resource:
[block](https://shopify.dev/docs/storefronts/themes/architecture/blocks/theme-blocks/quick-start?framework=liquid)
