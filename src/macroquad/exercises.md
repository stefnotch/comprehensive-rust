---
minutes: 100
---


# Macroquad Exercises

- [GLSL Post-processing](https://github.com/not-fl3/macroquad/blob/master/examples/post_processing.rs)
  - Use `is_key_down` to react to user input, and change the strength of the post-processing effects. 
- [First person camera](https://github.com/not-fl3/macroquad/blob/master/examples/first_person.rs)
- [Game of life](https://github.com/not-fl3/macroquad/blob/master/examples/life.rs)
  - Load a "scene" from a file.
    This can either be [a simple text file](https://conwaylife.com/patterns/gosperglidergun.cells), or [use a JSON file](https://github.com/stefnotch/rust-tutorial/blob/cee3a6205fdbe314e4f17a74d5e9e820ba36cdb7/glider-gun.json#L1). This is a nice opportunity to practice reading files and parsing them. For the JSON file, we recommend using [`serde` and `serde_json`](https://serde.rs/derive.html).
- [Snake!](https://github.com/not-fl3/macroquad/blob/master/examples/snake.rs)
  - Extend the game to have a second snake. There are multiple variations, it is up to you to choose the most fun one. This is a good opportunity to practice more with building abstractions (like extending the `Snake` struct).

<details>

We will go through 2 more chapters, and then we'll use what we've learned to create simple games!

The missing chapters can be covered on demand, or by the students themselves.

<!--The JSON file was generated using the following code:
```js
`put the cells text here`.split('\n').flatMap((v, y) => v.split("").flatMap((c, x) => c == 'O' ? [{x,y}]:[]));
```
-->

</details>