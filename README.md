# tw-hitbox

> 🖱️ Hitbox utility for Tailwind CSS

## Installation

```bash
pnpm install tw-hitbox
```

*Instead of `pnpm`, you can also use `npm`, `yarn`, or `bun`.*

Then, insert the following line near the top of your global `.css` file:

```diff
  @import "tailwindcss";
+ @import "tw-hitbox";
```

## Usage

The hitbox utility, works similarly to tailwind's built-in utilities for e.g. margin or padding, so classes like `hb-4`, `hb-y-[1px]` or `hb-t-2` are valid.

```html
<button class="hb-4">Hitbox extending to all sites</button>
<button class="hb-x-4">Hitbox extending to left and right</button>
<button class="hb-y-4">Hitbox extending to top and bottom</button>
<button class="hb-t-4">Hitbox extending to top</button>
```

### Debugging

Want to preview the hitbox area? Add the `hb-debug` class to the element.

```html
<button class="hb-4 hb-debug">Hitbox extending to all sites</button>
```

### Overriding through CSS variables

If you, for whatever reason, need to override the hitbox values through CSS variables, you can do so by setting the following variables:

```css
.element {
  --tw-hitbox-top: 10px;
  --tw-hitbox-right: 10px;
  --tw-hitbox-bottom: 10px;
  --tw-hitbox-left: 10px;
}
```

## Inspiration

The concept of this library is based on the [hit area utility by Kian Bazza](https://bazza.dev/craft/2026/hit-area).

Its purpose is to serve as an alternative that is available as a `npm` package instead of through a shadcn registry.
