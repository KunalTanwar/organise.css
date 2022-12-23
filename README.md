# organise.css

A modern alternative to CSS Reset.

### CDN

To rapidly include the minified production file in your webpage

```html
<link 
    rel="stylesheet" 
    href="https://cdn.jsdelivr.net/gh/KunalTanwar/organise.css/css/organise.min.css"
/>
```

```css
@import url('https://cdn.jsdelivr.net/gh/KunalTanwar/organise.css/css/organise.min.css');
```

### Optional Variant

A version in which [Inter](https://rsms.me/inter/) is set as default font with fallbacks. Also it contains different character variants.
`'cv07', 'cv08', 'cv10'`. You can find more variants [here](https://rsms.me/inter/#features/cvXX).

```html
<link 
    rel="stylesheet" 
    href="https://cdn.jsdelivr.net/gh/KunalTanwar/organise.css/css/organise.inter.min.css"
/>
```

```css
@import url('https://cdn.jsdelivr.net/gh/KunalTanwar/organise.css/css/organise.inter.min.css');
```

**Note** - Removed Inter font from `css` file because of layout shifts

<img src="https://user-images.githubusercontent.com/77537933/207933419-7a765fbb-c8d7-4162-938f-c433d104572e.gif" alt="Layout Shift" />

_Image Courtesy_ - [Pixel Point](https://pixelpoint.io/blog/advanced-web-font-optimization-techniques/)

Now, you need to add Inter manually; _(make sure add font CDN before `organise.inter.min.css`)_

#### HTML

```html
<!-- HTML in your document's head -->
<link rel="preconnect" href="https://rsms.me/">
<link rel="stylesheet" href="https://rsms.me/inter/inter.css">
```

### Bug

In chrome some emojis will replace by symbols. For that you can use `font-family: var(--emoji-font)`. There is an open [bug](https://bugs.chromium.org/p/chromium/issues/detail?id=964527) about this if you're interested on this topic.

### FYI

1. [normalize.css](https://github.com/necolas/normalize.css) is not updated since 4 years. So, I created this repo using the same principle. Addressed and fixed all the issues that are fixed by browsers or users. Added most of the PR fixes of **normalize.css** in this version.
2. If I left some issues open a PR for the same

### Contributing

Please read the [contribution guidlines](CONTRIBUTING.md) in order to make the contribution process easy and effective for everyone involved.
