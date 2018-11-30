# react-fluid-gallery ([demo](https://transitive-bullshit.github.io/react-fluid-gallery/))

> Fluid media gallery for React powered by WebGL.

[![NPM](https://img.shields.io/npm/v/react-fluid-gallery.svg)](https://www.npmjs.com/package/react-fluid-gallery) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

Inspired by [Tao Tajima](http://taotajima.jp/). Use the scroll wheel or mouse to transition fluidly between background images in a gallery.

## Install

```bash
npm install --save react-fluid-gallery
```

## Usage

```jsx
import React, { Component } from 'react'

import FluidGallery from 'react-fluid-gallery'

import image1 from './1.jpg'
import image2 from './2.jpg'
import image3 from './3.jpg'

export default class App extends Component {
  render () {
    return (
      <FluidGallery
        style={{ width: '100vw height: '100vh }}
        slides={[ image1, image2, image3 ]}
      />
    )
  }
}

```

## Props

| Property      | Type               | Default                               | Description                                                                                                                                  |
|:--------------|:-------------------|:--------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------|
| `slides`    | `Array<string>`           | **required**                                  | Array of images to use for the gallery slides. |
| `startAt`   | number          | random                                 | Default slide to show. |
| `onChange`  | function(index: number) | undefined   | Optional callback when the active slide is changed. |
| `...`       | ...              | undefined                            | Any other props are applied to the root canvas element. |

## Credits

The original versionon of this awesome gallery technique was published on the personal website of [Tao Tajima](http://taotajima.jp/).

## License

MIT © [Travis Fischer](https://github.com/transitive-bullshit)
