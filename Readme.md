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
.bg-white
```

### border

```css
.b[size][color][direction]

  _
.bad  /* a - 1px */
.bbd  /* b - 2px */

   _
.bad  /* d - #ddd */

    _
.bad  /* all */
.badr /* right */
.badl /* left */
.badt /* top */
.badb /* bottom */
```

### font-size

```css
.s[size]

  _
.sa   /* 8px */
.sb   /* 10px */
.sc   /* 12px */
.sd   /* 14px */
.se   /* 16px */
.sf   /* 18px */
.sg   /* 20px */
.sh   /* 22px */
.si   /* 24px */
.sj   /* 26px */
.sk   /* 28px */
.sm   /* 32px */
.so   /* 36px */
.sr   /* 42px */
.sv   /* 48px */
```

### float

```css
.left
.right
```

### text-align

```css
.ta[direction]

   _
.tal /* left */
.tac /* center */
.tar /* right */
```

### font-weight

```css
.fw[weight]

   _
.fwn  /* normal */
.fwb  /* bold */
```

### display

```css
.d[value]

  _
.di   /* inline */
.dib  /* inline-block */
.db   /* block */
```

### color

```css
.white  /* white */
.grey   /* #888 */
.dagrey /* #666 */
```

### margin & padding

```css
.[p|m][size][direction]

 _
.pbb  /* padding *.
.mbb  /* margin */

  _
.pax  /* 0em */
.pby  /* 0.2em */
.pcy  /* 0.4em */
.pdy  /* 0.6em */
.pey  /* 0.8em */
.mfy  /* 1em */
.mky  /* 2em */
.mpy  /* 3em */
.muy  /* 4em */
.mzy  /* 5em */

.mf   /* all directions */
.mfl  /* left */
.mfr  /* right */
.mft  /* top */
.mfb  /* bottom */
.mfy  /* top and bottom */
.mfx  /* left and right */
```

### miscellaneous

```css
.hidden     /* display: none; */
.full       /* width: 100%; */
.uppercase  /* text-transform: uppercase; */
.italic     /* font-style: italic; */
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
