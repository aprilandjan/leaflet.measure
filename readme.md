# leaflet.measure

> A [`Leaflet`](https://github.com/Leaflet/Leaflet) plugin to measure distance on map. This repository is based on [`jtreml/leaflet.measure`](https://github.com/jtreml/leaflet.measure), the origin repo seems not to be maintained anymore.

> Supported with current latest `leaflet` `v1.0.3`.

## Example

You can check the [example](http://aprilandjan.github.com/leaflet.measure/example.html) here.

## Usage

Assume that you have already installed `Leaflet`:

Enable plugin in map constructor:

```javascript
var map = L.map(elMap, {
  center: [22.536836, 113.951513],
  zoom: 5,
  measureControl: true
})
```

Or, add it anytime you wish, with specific options:

```javascript
L.control.measure({
  position: 'topleft'
}).addTo(map)
```

## Options

The available options are listed below: 

| option | default | description |
| ------| ------ | ------ |
| position | 'topleft' | Option from L.Control |
| keyboard | true | Weather to use keyboard control for this plugin. If set to true, you can use the defined key to toggle measuring |
| activeKeyCode | 77 | The key code to active measuring. 77 is the keyCode of 'M' |
| cancelKeyCode | 27 | The key code to cancel measuring. 27 is the keyCode of 'ESC' |
| lineColor | 'black' | The color of measuring line. Option from L.Polyline |
| lineWeight | 2 | The weight(width) of measuring line. Option from L.Polyline |
| lineDashArray | '6, 6' | The dash array of measuring line. Option from L.Polyline |
| lineOpacity | 1 | The opacity of measuring line. Option from L.Polyline |

## Todo
- control tooltip text customize
- measure data
- measure event
- add start point indicator