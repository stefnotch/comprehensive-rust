---
minutes: 10
---


# Getting started with Macroquad


We look up the library on [crates.io](https://crates.io/crates/macroquad) to find the latest version. We will use version `0.4.0` in this example.

Create a new project
```bash
cargo new --bin fun-game
```

And open it in your favorite editor.

We will add the following to our `Cargo.toml`:

```toml
[dependencies]
macroquad = "0.4.0"
```

And then we copy their example code into `src/main.rs`:

```rust
use macroquad::prelude::*;

#[macroquad::main("BasicShapes")]
async fn main() {
    loop {
        clear_background(RED);

        draw_line(40.0, 40.0, 100.0, 200.0, 15.0, BLUE);
        draw_rectangle(screen_width() / 2.0 - 60.0, 100.0, 120.0, 60.0, GREEN);
        draw_circle(screen_width() - 30.0, screen_height() - 30.0, 15.0, YELLOW);

        draw_text("IT WORKS!", 20.0, 20.0, 30.0, DARKGRAY);

        next_frame().await
    }
}
```

<details>

Go through the steps, and showcase crates.io.

Use `cargo add macroquad` to add the dependency. Note that git dependencies, and other registries, also exist.

And then showcase that we can look up what each function does on docs.rs. Go a bit into why docs.rs is useful and takes advantage of the fact that most code is open source.

Finally, show that the Readme includes a WASM guide.
</details>