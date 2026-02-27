### Hi there 👋

I'm MysticalDevil, a beginner programmer.

### GitHub Analytics

```zig
const std = @import("std");

const User = struct {
    name: []const u8,
    role: []const u8,
    editor: []const u8,
    languages: []const []const u8,
    building: []const []const u8,
};

pub fn main() !void {
    const me = User{
        .name = "MysticalDevil",
        .role = "beginner programmer",
        .editor = "Neovim",
        .languages = &.{ "Go", "Zig", "Lua" },
        .building = &.{ "gout", "zite", "nvim config" },
    };

    std.debug.print("== {s}'s Terminal Dashboard ==\n", .{me.name});
    std.debug.print("role      : {s}\n", .{me.role});
    std.debug.print("editor    : {s}\n", .{me.editor});

    std.debug.print("languages : ", .{});
    for (me.languages, 0..) |lang, i| {
        if (i != 0) std.debug.print(" | ", .{});
        std.debug.print("{s}", .{lang});
    }
    std.debug.print("\n", .{});

    std.debug.print("building  : ", .{});
    for (me.building, 0..) |project, i| {
        if (i != 0) std.debug.print(", ", .{});
        std.debug.print("{s}", .{project});
    }
    std.debug.print("\nstatus    : shipping small things, learning fast\n", .{});
}
```

### Tech Stack

[![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)](https://go.dev/) [![Zig](https://img.shields.io/badge/Zig-F7A41D?style=for-the-badge&logo=zig&logoColor=white)](https://ziglang.org/) [![Lua](https://img.shields.io/badge/Lua-2C2D72?style=for-the-badge&logo=lua&logoColor=white)](https://www.lua.org/)
[![Neovim](https://img.shields.io/badge/Editor-Neovim-57A143?style=for-the-badge&logo=neovim&logoColor=white)](https://neovim.io/)

Primary editor: **Neovim**

### Featured Projects

- [`nvim`](https://github.com/MysticalDevil/nvim): A Neovim setup for Go, Zig, and Rust development.
- [`nvim-lite`](https://github.com/MysticalDevil/nvim-lite) A simplified version of my Neovim configuration.
- [`zite`](https://github.com/MysticalDevil/zite) A SQLite-based Data Mapper-style ORM library for learning purposes only, and not suitable for production use.
- [`gout`](https://github.com/MysticalDevil/gout) A lightweight Go web framework inspired by Gin.
