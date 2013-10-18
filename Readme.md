# Fungible

A collection of base CSS classes that let you write styled HTML without writing any CSS. Fungible originated out of the need to scaffold HTML quickly without having to slow down and write CSS for each element. Its declarative usage is inspired by AngularJS. 

## Basics

This is what HTML might look like if you're using Fungible.

```html
<div class="mfb pk bad">
  <span class="se fwb"></span>
</div>

<!--
mfb - m (margin), f (1.0em), b (bottom)
pk - p (padding), k (2.0em)
bad - b (border), a (1px), d (#ddd)
fwb - fw (font-weight), b (bold)
-->
```

Here's a rundown of what's available to you:

### background-color

```css
.bg-[color]
```

**color**
- white - white `.bg-white`

### border

```css
.b[size][color][direction]
```

**size**
- a - 1px `.bad`
- b - 2px `.bbd`

**color**
- d - #ddd `.bad`

**direction**
- _ - all `.bad`
- r - right `.badr`
- t - top `.badt`
- b - bottom `.badb`
- l - left `.badl`

### font-size

```css
.s[size]
```

**size**
- a - 8px `.sa`
- b - 10px
- c - 12px
- d - 14px
- e - 16px
- f - 18px
- g - 20px
- h - 22px
- i - 24px
- j - 26px
- k - 28px
- m - 32px
- o - 36px
- r - 42px
- v - 48px

### float

```css
.left
.right
```

### text-align

```css
.ta[direction]
```

**direction**
- l - left `.tal`
- c - center `.tac`
- r - right `.tar`

### font-weight

.fw[weight]

- n - normal `.fwn`
- b - bold `.fwb`

### display

```css
.d[value]
```

**value**
- ib - inline-block `.dib`
- i - inline `.di`
- b - block `.db`

### color

```css
.white /* white */
.grey /* #888 */
.dagrey /* #666 */
```

### margin & padding

```css
.[p|m][size][direction]
```

**size**
- a - 0em `.ma, .pa`
- b - 0.2em `.mb, .pb`
- c - 0.4em `.mc, .pc`
- d - 0.6em `.md, .pd`
- e - 0.8em `.me, .pe`
- f - 1em `.mf, .pf`
- k - 2em `.mk, .pk`
- p - 3em `.mp, .pp`
- u - 4em `.mu, .pu`
- z - 5em `.mz, .pz`

**direction**
- _ - all `.mf, .pf`
- l - left `.mfl, .pfl`
- r - right `.mfr, .pfr`
- t - top `.mft, .pft`
- b - bottom `.mfb, .pfb`
- x - left and right `.mfx, .pfx`
- y - top and bottom `.mfy, .pfy`

### miscellaneous

```css
.hidden /* display: none; */
.full /* width: 100%; */
.uppercase /* text-transform: uppercase; */
.italic /* font-style: italic; */
```

## Installation

Install with [component(1)](http://component.io):

```bash
$ component install jeffcarp/fungible
```

Also available as a Rails gem (if you're using the asset pipeline): [fungible-rails](https://github.com/jeffcarp/fungible-rails)

## Wish list

- Search through files and only include classes that are mentioned in the template. (this might be better as an add-on)

## License

MIT
