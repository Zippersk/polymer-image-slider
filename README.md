[![Build status](https://travis-ci.org/philipjkim/polymer-image-slider.svg?branch=master)](https://travis-ci.org/philipjkim/polymer-image-slider)

_[Demo](https://philipjkim.github.io/)_


##&lt;polymer-image-slider&gt;

`polymer-image-slider` allows user to show multiple images one at a time, with `prev` and `next` buttons.

Example:

```html
<image-slider images='["images/a.jpg","images/b.jpg","images/c.jpg"]'></image-slider>
```


### API Reference

#### Properties

| Name | Type | Description |
| --- | --- | --- |
| `images` | `Array`, Default: `[]` | Image source(s). If this is empty, the slider is hidden. |
| `currentPos` | `Number`, Default: `0` - readonly | The index of images for the currently shown image |
| `currentImg` | `String`, Default: `""` - readonly | Image source for the currently shown image |
| `maxWidth` | `Number`, Default: `0` | If greater than 0, max-width for the image is set to the value. |
| `noBullets` | `Boolean`, Default: `false` | If true, bullets below image are hidden. |

#### Methods

| Name | Description |
| --- | --- |
| `prev()` | Change the currently shown image to `images[currentPos-1]`, or the last element of `images` when `currentPos` is `0`. |
| `next()` | Change the currently shown image to `images[currentPos+1]`, or the first element of `images` when `currentPos` is `images.length - 1`. |


### TODOs

PRs are always welcomed.

- API docs
- Auto-scrolling
