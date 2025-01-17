# `freetype_render_target = "Normal"`

*Since: nightly builds only*

Configures the *rendering* mode used with the freetype rasterizer.

The default is to use the value of [freetype_load_target](freetype_load_target.md).

You may wish to override that value if you want very fine control over
how freetype hints and then renders glyphs.

For example, this configuration uses light hinting but produces
subpixel-antialiased glyph bitmaps:

```lua
return {
  freetype_load_target = "Light",
  freetype_render_target = "HorizontalLcd",
}
```

