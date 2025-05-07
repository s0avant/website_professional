---
title: Page de type gallerie 
type: gallery-masonry
params:
    catchline: "Style Instagram ou Masonry!"
    button: "Je veux voir ✨"
---

# Gallerie d'image Masonry !
## Fonctionnalités
✨ Image gallery rendered from page bundle  
✨ Images are resized with [Hugo Resize function](https://gohugo.io/content-management/image-processing/#resize)  
✨ Masonry grid layout is [recalculated once all images are loaded to prevent any display issues](https://github.com/francoiducat/hugo-air/blob/main/layouts/partials/gallery-masonry.html)  
✨ FancyBox effect on click  
✨ [Zoom effect on hover](https://github.com/francoiducat/hugo-air/blob/main/assets/sass/main.scss)

## Usage

Add images to your page bundle  
Edit the page type with `type: gallery-masonry` or `type: gallery-insta` 

```yaml
---
title: Gallery Page Type
type: gallery-masonry
params:
    catchline: "Instagram or Masonry Gallery!"
---
```

## Gallery