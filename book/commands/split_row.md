---
title: split row
version: 0.63.0
usage: |
  Split a string into multiple rows using a separator
---

<script>
  import { usePageFrontmatter } from '@vuepress/client';
  export default { computed: { frontmatter() { return usePageFrontmatter().value; } } }
</script>

# <code>{{ frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ frontmatter.usage }}</div>

## Signature

```> split row (separator) --number```

## Parameters

 -  `separator`: the character that denotes what separates rows
 -  `--number {int}`: Split into maximum number of items

## Examples

Split a string into rows of char
```shell
> echo 'abc' | split row ''
```

Split a string into rows by the specified separator
```shell
> echo 'a--b--c' | split row '--'
```
