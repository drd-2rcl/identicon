# Identicon

This tool generate images formed of a five by five grid thas is 300px wide 300px tall and each square in this grid is 50 by 50px. Composed of 25 smaller squares inside of it. Some of those squares in the grid are colored and the colored squares are mirrored about the center axis.

Each identicon on should it not be randomly generated. It generate based on a string input. So if i enter the same string twice I should always get back the same identical thing.

## How is done?
- Simple structure:
```elixir
string -> identicon generator -> image
```
- Detail structure:

```elixir
string -> compute MD5 hash of string -> list of numbers based on the string -> pick color -> build grid of squares -> convert grid into image -> save image
```
