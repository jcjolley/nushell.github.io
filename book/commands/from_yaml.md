---
title: from yaml
version: 0.63.0
usage: |
  Parse text as .yaml/.yml and create table.
---

<script>
  import { usePageFrontmatter } from '@vuepress/client';
  export default { computed: { frontmatter() { return usePageFrontmatter().value; } } }
</script>

# <code>{{ frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ frontmatter.usage }}</div>

## Signature

```> from yaml ```

## Examples

Converts yaml formatted string to table
```shell
> 'a: 1' | from yaml
```

Converts yaml formatted string to table
```shell
> '[ a: 1, b: [1, 2] ]' | from yaml
```
