---
title: math ceil
version: 0.63.0
usage: |
  Applies the ceil function to a list of numbers
---

<script>
  import { usePageFrontmatter } from '@vuepress/client';
  export default { computed: { frontmatter() { return usePageFrontmatter().value; } } }
</script>

# <code>{{ frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ frontmatter.usage }}</div>

## Signature

```> math ceil ```

## Examples

Apply the ceil function to a list of numbers
```shell
> [1.5 2.3 -3.1] | math ceil
```
