<img alt="Mermaid Banner" src="images\Mermaid_Banner.png"/>

# GitHub Charts Using Mermaid

Presentation content for Mermaid, the clever chart visualization for Markdown syntax, for specific use in GitHub

<br><br>

<img alt="Mermaid Banner" src="images\Mermaid_HR.png"/>

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
  subgraph This is my title
    A --> B
  end
```

<img src="images\microwave.png" alt="Multi Photo Frame to explain how components mesh together" width="200"/><img src="images\microwave.png" alt="Multi Photo Frame to explain how components mesh together" width="200"/><img src="images\microwave.png" alt="Multi Photo Frame to explain how components mesh together" width="200"/>

<a href="http://google.com"><img alt="Mermaid Banner" src="images\Mermaid_Banner.png"/></a>
