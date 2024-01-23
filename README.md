# C/C++ (clangd) for Lapce

## Configuration

Use the settings UI or directly adjust `settings.toml`:

```toml
[lapce-cpp-clangd]
clangdVersion = "15.0.0"                       # git tag from https://github.com/clangd/clangd
volt.serverPath = "<path to custom clangd>"    # use custom clangd instead of downloading
volt.serverArgs = "--first-arg --second=arg=0" # flags passed to clangd (see clangd --help)
volt.cPattern = "h,c"                          # use these file extensions for C
volt.cppPattern = "H,hh,hpp,C,cc,cpp,c++"      # use these file extensions for C++
```

## Platforms

Plugin will automatically download `clangd` for below architectures

| Platform | x86_64 (amd64) | aarch64 (arm64) |
| -------- | -------------- | --------------- |
| Linux    | ✔️              | ❌               |
| Windows  | ✔️              | ❌               |
| macOS    | ✔️              | ❌               |
