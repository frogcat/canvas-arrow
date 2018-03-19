# canvas-arrow
Simple javascript lib to add CanvasRederingContext2D#arrow method

![image](https://user-images.githubusercontent.com/12029629/37581449-05217af4-2b8c-11e8-9d3b-a024d7a2ccc4.png)

## Demo

- <https://frogcat.github.io/canvas-arrow/>

## Usage

```
// include canvas-arrow.js to extend CanvasRenderingContext2D
<script src="https://frogcat.github.io/canvas-arrow/canvas-arrow.js"></script>`
...
// draw
<script>
var context = canvas.getContext("2d");
context.beginPath();
context.arrow(0, 0, 200, 100, [0, 1, -10, 1, -10, 5]);
context.fill();
</script>
...
```

## API


`CanvasRederingContext2D#arrow(startX, startY, endX, endY, controlPoints);`


### Parameters

Option   | Type              | Description
-------- | ----------------- | ---------------------------------
startX   | number            | The x axis of the coordinate for the begin of the arrow
startY   | number            | The y axis of the coordinate for the begin of the arrow
endX     | number            | The x axis of the coordinate for the end of the arrow
endY     | number            | The y axis of the coordinate for the end of the arrow
controlPoints | Array of numbers | controlPoints (#1)


(#1) controlPoints array is list of x,y to define shape of arrow, see below.

![image](https://user-images.githubusercontent.com/12029629/37581903-cb15520c-2b8d-11e8-8799-f827300408b8.png)


