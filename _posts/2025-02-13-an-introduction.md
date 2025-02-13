---
layout: post
title: An Introduction
date: 2025-02-13 23:45 +0100
categories: [Article]
tags: [intro, writing]
author: felix
math: true
---

{% include embed/{bilibili}.html id='{BV1Q44y1B7Wf}' %}

> Example line for prompt.
{: .prompt-info }

> Example line for prompt.
{: .prompt-tip }

> Example line for prompt.
{: .prompt-warning }

> Example line for prompt.
{: .prompt-danger }

`inline code part`

`/path/to/a/file.extend`{: .filepath}

```
This is a plaintext code snippet.
```

```yaml
key: value
```

```shell
echo 'No more line numbers!'
```
{: .nolineno }

```shell
# content
```
{: file="path/to/file" }

{% raw %}
```liquid
{% if product.title contains 'Pack' %}
  This product's title contains the word Pack.
{% endif %}
```
{% endraw %}

<!-- Block math, keep all blank lines -->

$$
LaTeX_math_expression
$$

<!-- Equation numbering, keep all blank lines  -->

$$
\begin{equation}
  LaTeX_math_expression
  \label{eq:label_name}
\end{equation}
$$

Can be referenced as \eqref{eq:label_name}.

<!-- Inline math in lines, NO blank lines -->

"Lorem ipsum dolor sit amet, $$ LaTeX_math_expression $$ consectetur adipiscing elit."

<!-- Inline math in lists, escape the first `$` -->

1. \$$ LaTeX_math_expression $$
2. \$$ LaTeX_math_expression $$
3. \$$ LaTeX_math_expression $$

