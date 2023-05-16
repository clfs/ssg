# ssg

A zero-config static site generator.

## Installation

Install or update `ssg`:

```text
go install github.com/clfs/ssg@latest
```

Uninstall `ssg`:

```text
rm -i $(which ssg)
```

## An example

### Input

`posts/index.md` (special case):

```markdown
Hey! I'm Jim.

Email me at [my@name.is.jim].

[my@name.is.jim]: mailto:my@name.is.jim
```

`posts/gangkhar-puensum.md`:

```markdown
Date: 2023-05-15

# Gangkhar Puensum

Gangkhar Peunsum is the [highest] unclimbed mountain in the world.

[highest]: https://en.wikipedia.org/wiki/Highest_unclimbed_mountain
```

### Usage

Read Markdown files from `posts/`, then output site content to `public/`.

```text
ssg -in posts -out public -author "Jim J. Jim"
```

### Output

`public/index.html`:

```html
```

`public/css.css`:

```css
```

`public/gangkhar-puensum.html`:

```html
```