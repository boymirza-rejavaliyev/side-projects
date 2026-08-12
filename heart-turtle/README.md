# Heart (Python Turtle)

Draws an animated heart shape made entirely of repeated "I love you" text, using Python's built-in `turtle` module and a parametric heart curve.

## Preview

![Heart demo](demo.png)

## How it works

The heart outline is generated with a parametric equation:

```
x = 16 * sin(angle)^3
y = 13*cos(angle) - 5*cos(2*angle) - 2*cos(3*angle) - cos(4*angle)
```

The curve is traced multiple times at increasing scale (`range(11, 17)`), and at each point along the curve the turtle writes the text `"I love you"` instead of drawing a line — building up a dense, text-filled heart shape.

## Run

```bash
python3 heart.py
```

Requires Python 3 with `turtle` (included in the standard library on most systems; on Linux you may need `sudo apt install python3-tk`).
