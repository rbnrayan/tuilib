# TUI-lib

## Purpose of the lib

Provide an abstract way to create <b>T</B>ext-Based <b>U</b>ser <b>I</b>nterface.
The library is build on top of (termion)[https://docs.rs/termion/latest/termion/index.html].

### Example

```rust
use tui::*;

fn main() {
  let content = Content::new("text block", Position::Center, Position::Center);
  let text_block = TextBlock::new((1, 1), 10, 1, content);

  App::new().attach(&[&text_block]).run().unwrap();
}
```
