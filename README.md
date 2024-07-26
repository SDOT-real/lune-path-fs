# lune-path-fs
luau-path + @lune/fs

## Note
This library is based on [luau-path](https://github.com/seaofvoices/luau-path) by seaofvoices

## Features
- `luau-path` utility
- fs library but supports path objects (`AsPath` objects which include string and `Path` objects)
- Does not require `node` & `npm` anymore.

## Installation
Use git submodules.
```sh
git submodule add
```

## Usage
```lua
pathfs.writeFile("something.json", "{ \"message\": \"Hello, world!\" }")

local path = pathfs.Path.from("something.json")

print(pathfs.readFile(path))

```
