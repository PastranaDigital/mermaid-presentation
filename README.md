<img alt="Mermaid Banner" src="images\Mermaid_Banner.png"/>

# GitHub Charts Using Mermaid

Presentation content for Mermaid, the clever chart visualization for Markdown syntax, for specific use in GitHub

```mermaid
graph TD

    Name_of_A[Rectangle] -->|Text in Path| Name_of_B(Rounded Rectangle)

    Name_of_B --> Name_of_C{Diamond}

    Name_of_C -->|Text in Path| Name_of_D[Rectangle]

    Name_of_C -->|Text in <br> 2 lines| Name_of_E[\<br>Trapezoid<br><br>/]

    Name_of_C -->|Text in Path| Name_of_F((Circle))
```

```mermaid
graph TD
title(Outline)
title-->A[Where It All Started]
style title fill:#A6EDBE,stroke:#FFF,color:#003F5F,stroke-width:0
linkStyle 0 stroke:#FFF,stroke-width:0;

A --> B(Pictures & Charts are Powerful)
B --> C{Are pictures<br>better?}
C -. Yes .-> E
C -. No .-> D

style C fill:#1c1c1c

classDef orange fill:#f96,stroke:#d1d1d1,stroke-width:4px,color:#333
class C orange

```

<br><br>

## Where It All Started

-   For over 6 years, Mermaid has been around as a Javascript library for charting
-   Plant UML, a great tool but...
-   GitHub's 2022 Valentine's Day gift

<br><br>

## Pictures & Charts are Powerful

<img src="images/pictionary_steps.png" alt="Pictionary Chart Example" width="800"/>

Demo of coding a hand drawn chart in VSCode with preview tools

Show how to do it with Live Editor

Review what & why we learned it

Discuss further learning, resources & documentation

Questions

<br><br>

## Helpful Tips

### _Color Carefully_

This example uses stylized coloring of the components, This should be tested in both **light** and **dark** mode. When you change the backgorund color of a node, for example, the text color may need to be set also.

```mermaid
graph TB
    sq[Square shape] ==> ci((Circle shape))

    %% Notice that no text in shape are added here instead that is appended further down
    e --> od3>Really long text with linebreak<br>in an Odd shape]

    %% Comments after double percent signs
    e((Inner / circle<br>and some odd <br>special characters)) -.-> f(Example Text)

    cyr[Cyrillic]-->cyr2((Hard to read in <br> Dark mode));
    linkStyle 3 stroke:#F0F,stroke-width:5;

     classDef green fill:#9f6,stroke:#6c3,stroke-width:5px,color:#333
     classDef orange fill:#f96,stroke:#d63,stroke-width:4px
     class sq,e green
     class cyr2 orange
```

<br><br>

### _Two Ways to Add a Chart Title_

from https://github.com/mermaid-js/mermaid/issues/177

```mermaid
graph LR

title[<i>This is My Example Title</i>]
title --> FirstStep

%% this styling hides the connection arrow for link index 0
style title fill:#FFF,stroke:#FFF,color:#000
linkStyle 0 stroke:#FFF,stroke-width:0;

FirstStep --> SecondStep

```

```js
graph LR

title[<i>This is My Example Title</i>]
title --> FirstStep

%% this styling hides the connection arrow for link index 0
style title fill:#FFF,stroke:#FFF,color:#000
linkStyle 0 stroke:#FFF,stroke-width:0;

FirstStep --> SecondStep
```

<br>

```mermaid
graph LR

  subgraph This is my example title
    A[First node] --> B{Second Node}
  end

```

```js
graph LR

  subgraph This is my example title
    A[First node] --> B{Second Node}
  end
```

<br><br>

### _Places to Use it in GitHub_

-   README.md documentation
-   Comments in Pull Requests
-   GitHub Actions for visualization

```mermaid
pie
  title Test Coverage
  "Passing" : 14
  "Failing" : 3

```

<br><br>

## Resources

<a href="https://mermaid-js.github.io/mermaid/"><img alt="Mermaid GitHub Website" src="images\resource01.png"/></a>
<a href="https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/"><img alt="GitHub Blog about Mermaid" src="images\resource02.png"/></a>
<a href="https://mermaid-js.github.io/mermaid-live-editor/"><img alt="Mermaid Live Editor" src="images\resource03.png"/></a>
<a href="https://jojozhuang.github.io/tutorial/mermaid-cheat-sheet/"><img alt="Mermaid Cheat Sheet" src="images\resource04.png"/></a>

<br><br>

## Further Learning (100% Free)

<a href="https://www.youtube.com/watch?v=eJojC3lSkwg"><img alt="Learning GitHub Writing Markdown" src="images\video_resource01.png"/></a>
<a href="https://wesbos.com/mastering-markdown"><img alt="Mastering Markdown Course" src="images\video_resource02.png"/></a>
<a href="https://www.youtube.com/playlist?list=PLUoebdZqEHTxNC7hWPPwLsBmWI0KEhZOd"><img alt="Lucid Chart Diagram Playlist" src="images\video_resource03.png"/></a>

<br><br>

## VSCode Extensions

<img src="images/VSCode_Extension01.png" alt="Markdown Preview Icon" width="40"/> Markdown Preview GitHub Styling https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles

<img src="images/VSCode_Extension02.png" alt="Markdown Preview Mermaid Icon" width="40"/> Markdown Preview Mermaid Support https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid
