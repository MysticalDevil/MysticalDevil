### Hi there 👋

I'm MysticalDevil, a new programmer.

### GitHub Analytics

```zig
const std = @import("std");

pub const User = struct {
    name: []const u8,
};

pub fn main() !void {
    const me = User{
        .name = "MysticalDevil",
    };
    std.debug.print("{s}\n", .{me.name});
    std.debug.print("A Zig learner.\n", .{});
}
```

### Pinned repository

- [`nvim`](https://github.com/MysticalDevil/nvim) The configuration file of Neovim is mainly configured by TypeScript and Rust.
- [`nvim-lite`](https://github.com/MysticalDevil/nvim-lite) A simplified version of my Neovim config.
- [`zite`](https://github.com/MysticalDevil/zite) A SQLite-based Data Mapper-style ORM library (for learning purposes only, not suitable for production use).
