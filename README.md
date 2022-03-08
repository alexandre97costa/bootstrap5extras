
# Bootstrap 5 Extras

A few extra functionalities to add on top of the standard Bootstrap 5 template styling.


# Usage

## Using a CDN
You can copy this line into your html document, and place it *below* the Bootstrap's CSS 
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/alexandre97costa/bootstrap5extras/main.min.css" integrity="sha384-1AgpaGraxmZfUSv85Q1IoegydxJx90MTIkT3Bo6Lum0u8uE9EoJtQn/vCuHOOwfb" crossorigin="anonymous">
```
You might encounter some problems with this code's integrity attribute. My recommendation is to go to `https://www.srihash.org/` and paste `https://cdn.jsdelivr.net/gh/alexandre97costa/bootstrap5extras/main.min.css` there. It will generate the appropriate hash and link tag.

## Use it locally

You can also download the `main.css` file from this repo and place it in your project's files. Remember to rename it and place it after bootstrap's css and before your own.


# Documentation

Here is some basic documentation explaining how everything works. Bootstrap5extras adds the following functionalities (for now):
- More radius sizes;
- Separate radius size for each corner
- More focus colors for `.form-control`, `.form-select`, `.input-group` and `.btn-group`.

## Radius Sizes

Use the class `radius-` followed by a number from 0 to 5 to make the element have an increasingly bigger border radius. 
For consistency with Bootstrap's spacing utilities, the size of the radius is the same as the standard spacing for margin and padding:
- `radius-0` had a border radius of `0em`;
- `radius-1` had a border radius of `0.25em`;
- `radius-2` had a border radius of `0.5em`;
- `radius-3` had a border radius of `1em`;
- `radius-4` had a border radius of `1.5em`;
- `radius-5` had a border radius of `3em`;

## Individual Corner Radius

Bootstrap has a special nomenclature for each of an element's sides. This file uses those names in its' acronyms, and works just like the `margin` and `padding` utilities.
To recap: Top, Bottom, Start and End are the names of each side of an element. Therefore, the corners are named after a mix of the two sides they belong to. For example, the top left corner's name is `ts`, which stands for `top` and `start`.

Here are the different corners explicitly:
- `radius-ts-X`;
- `radius-te-X`;
- `radius-bs-X`;
- `radius-be-X`;

Where `X` is a number from 0 to 5.

## Focus Colors
While using Bootstrap I also noticed that you cant really change the focus color of an input by default. It always has that blue drop-shadow that might not fit well with your scheme, or any of the remaining colors in Bootstrap's default colors. Because of that, I made some basic classes that change that drop-shadow's color, using Bootstrap's nomenclature.
Here are the different variations:

- `focus-primary` (default);
- `focus-secondary`;
- `focus-success`;
- `focus-info`;
- `focus-warning`;
- `focus-danger`;

_Note that these only work on `.form-control`, `.form-select`, `.input-group` and `.btn-group`._


## To sum it up

I know this repo is nothing fancy, but the file has helped me, and so I thought it might help someone else too.
If you end up using it, please star it or just message me on Discord saying that my extras suck at Calimero#2948

Have fun and happy coding! ♥

