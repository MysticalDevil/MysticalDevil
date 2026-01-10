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

### Pinned responsitory

- [`nvim`](https://github.com/MysticalDevil/nvim) The configuration file of Neovim is mainly configured by TypeScript ans Rust.
- [`nvim-lite`](https://github.com/MysticalDevil/nvim-lite) My nvim config simplifily version.
- [`zig_orm_sqlite`](https://github.com/MysticalDevil/zig_orm_sqlite) A SQLite-based Data Mapper-style ORM library (for leanring purposes only, not suitable for production use).
