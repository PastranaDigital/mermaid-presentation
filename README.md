# GitHub Charts using Mermaid
Presentation content for Mermaid, the clever chart visualization for Markdown syntax, for specific use in GitHub

<br><br>
## Two Ways to Add a Chart Title
from https://github.com/mermaid-js/mermaid/issues/177
```mermaid
graph TD

title[<u>My Title</u>]
title-->FirstStep
style title fill:#FFF,stroke:#FFF,color:#000
linkStyle 0 stroke:#FFF,stroke-width:0;

FirstStep-->...
```

```mermaid
graph LR
  subgraph This is my caption
    A --> B
  end
```
