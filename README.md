# vue-pannellum
Vue wrap of the brilliant panorama viewer Pannellum

## Usage
install
```
npm install vue-pannellum
```

register
```js
import Vue from 'vue'
import VuePannellum from 'vue-pannellum'

Vue.component('VPannellumn', VuePannellum)
```

use
```html
<v-pannellum :src="equirectangularUrl"></v-pannellum>
```

## API

component props:

- **src (required)**: The equirectangular image url or cubemap urls in this format: {px: pxUrl, nx: nxUrl, ... }.
- **preview**: The preview image url before loaded.
- **autoLoad (boolean, default: true)**: Whether automatically load.
- **autoRotate (number|boolean, default: 0)**: The auto-rotate speed, 0 or false means disabled, true is -2.
- **orientation (boolean, default: false)**: Turn the orientation sensor on (if supported).
- **showZoom (boolean, default: false)**: Show the zoom-in and zoom-out button.
- **showFullscreen (boolean, default: false)**: Show the fullscreen button.
- **compass (boolean, default: false)**: Show the compass indicator.
- **hfov (number, default: 75)**: The initial horizontal field of view in degrees.
- **yaw (number, default: 0)**: The initial yaw position in degrees.
- **pitch (number, default: 0)**: The initial pitch position in degrees.
- **minHfov (number, default: 30)**: The minimum limit of hfov in degrees.
- **maxHfov (number, default: 120)**: The maximum limit of hfov in degrees.

## Features
- type
- autoLoad
- autoRotate
- compass
- show/hide control button
- preview
- initial view: hfov/yaw/pitch
- slot
- watch url changing
- max/minHfov
- orientation

## Licence

MIT
