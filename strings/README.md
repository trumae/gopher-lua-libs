# strings [![GoDoc](https://godoc.org/github.com/vadv/gopher-lua-libs/strings?status.svg)](https://godoc.org/github.com/vadv/gopher-lua-libs/strings)

## Usage

```lua
local inspect = require("inspect")
local strings = require("strings")

-- strings.split(string, sep)
local result = strings.split("a b c d", " ")
print(inspect(result, {newline="", indent=""}))
-- Output: { "a", "b", "c", "d" }

-- strings.has_prefix(string, prefix)
local result = strings.has_prefix("abcd", "a")
-- Output: true

-- strings.has_suffix(string, suffix)
local result = strings.has_suffix("abcd", "d")
-- Output: true

-- strings.trim(string, cutset)
local result = strings.trim("abcd", "d")
-- Output: abc
```
