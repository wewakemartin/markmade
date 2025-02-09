# Obsidian Sketchpen

A tool to draw in Obsidian markdown notes.

![](SketchPen_Test.gif)

![](Screenshot.png)

---

## Instructions:

Tag your code block with `sketch-pen` like the screenshot and copy paste the code below into the code block.
Move the mouse over the canvas to draw in live preview or reading mode.



````

```sketch-pen

cnv.width  = cnv.parentNode.scrollWidth
cnv.height = cnv.width * 9/16

const ctx = cnv.getContext (`2d`)

ctx.fillStyle = `white`
ctx.fillRect (0, 0, cnv.width, cnv.height)

cnv.addEventListener("mousemove", logKey);

function logKey(e) {

cnv_X = cnv.getBoundingClientRect().left
cnv_Y = cnv.getBoundingClientRect().top


    a = e.pageX - cnv_X
    b = e.pageY - cnv_Y


ctx.fillRect (a, b, 5, 5);

ctx.fillStyle = `white`
ctx.fillRect (0, 0, 50, 230)

ctx.fillStyle = `black`
ctx.font = "18px serif";


}


```

````


## Credits:

Many thanks to [obsidian-canvas-api](https://github.com/capogreco/obsidian-canvas-api) for showing how to run p5js sketches inside Obsidian notes. 

## Further

https://developer.mozilla.org/en-US/docs/Web/API/Touch

https://developer.mozilla.org/en-US/docs/Web/API/Touch_events

https://developer.mozilla.org/en-US/docs/Web/API/TouchList

https://developer.mozilla.org/en-US/docs/Web/API/Ink_API

https://developer.mozilla.org/en-US/docs/Web/API/Pointer_events/Multi-touch_interaction

https://developer.mozilla.org/en-US/docs/Web/API/Pointer_events













