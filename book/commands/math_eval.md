---
title: math eval
version: 0.63.0
usage: |
  Evaluate a math expression into a number
---

<script>
  import { usePageFrontmatter } from '@vuepress/client';
  export default { computed: { frontmatter() { return usePageFrontmatter().value; } } }
</script>

# <code>{{ frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ frontmatter.usage }}</div>

## Signature

```> math eval (math expression)```

## Parameters

 -  `math expression`: the math expression to evaluate

## Examples

Evaluate math in the pipeline
```shell
> '10 / 4' | math eval
```
