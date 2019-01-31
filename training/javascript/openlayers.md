# OpenLayers

[OpenLayers](https://openlayers.org/)

## Tips and tricks

### Mes points ne sont pas visibles sur la carte

See default [ol.style](http://openlayers.org/en/latest/apidoc/ol.style.html) of ol.layer.Vector

Stroke needs some shape of feature such as circle, polygon, etc,. simple ol.geom.point doesn't have a shape. that's why nothing appears when you set style only with stroke

If you change your style like below, it will work as you expect:
```
var style = new ol.style.Style({
  image: new ol.style.Circle({ // add this
    stroke: new ol.style.Stroke({
      color: 'red'
    }),
    radius: 5
  }),
});
```

### Clear features in a vector layer
https://gis.stackexchange.com/questions/251770/how-can-i-clear-a-vector-layer-features-in-openlayers-4

### Rotate marker image
[Rotate marker Image](https://openlayers.org/en/latest/apidoc/module-ol_style_Icon.html)
