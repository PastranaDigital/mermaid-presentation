Short story of where it all started

Pictures & Charts are powerful, give example (maybe words describing a chart)

Demo of coding a hand drawn chart in VSCode with preview tools

Show how to do it with Live Editor

Review what & why we learned it

Discuss further learning, resources & documentation

Questions

---

Where it started: https://github.community/t/feature-request-support-mermaid-markdown-graph-diagrams-in-md-files/1922

### _Pre-work if you would like to follow along_

1. Download and install the VSCode Extensions listed below

    1. [Markdown Preview GitHub Styling](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles)

    1. [Markdown Preview Mermaid Support](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid)

1. Create a DEMO.md file in VSCode

---

GitHub Blog: https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/

Mermaid GitHub Website Documentation: https://mermaid-js.github.io/mermaid/#/

Mermaid Live Editor: https://mermaid-js.github.io/mermaid-live-editor/

Mermaid Cheat Sheet: https://jojozhuang.github.io/tutorial/mermaid-cheat-sheet/

Article discussing the advantages of using Mermaid: https://ardalis.com/github-diagrams-with-mermaid/

In the Future: Font Awesome? https://github.com/mermaid-js/mermaid/issues/1435

VSCode Extensions

Markdown Preview GitHub Styling: https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles

Markdown Preview Mermaid Support: https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid

---

### _Extra Learning_

Free Markdown Course: https://wesbos.com/mastering-markdown

▶️ Learning GitHub Markdown: https://www.youtube.com/watch?v=eJojC3lSkwg

---

```mermaid
graph TD

    Name_of_A[Rectangle] -->|Text in Path| Name_of_B(Rounded Rectangle)

    Name_of_B --> Name_of_C{Diamond}

    Name_of_C -->|Text in Path| Name_of_D[Rectangle]

    Name_of_C -->|Text in Path| Name_of_E[\<br>Trapezoid<br><br>/]

    Name_of_C -->|Text in Path| Name_of_F((Circle))
```

---

## Guide To Using The Office Microwave

-   Is it Seafood?

    -   If yes, then stop

    -   If no, then proceed to next question

-   Is it Popcorn?

    -   If no, then carry on

    -   If yes, then

        -   Did you bring enough to share?

            -   If yes, then carry on

            -   If no, then stop

---

-   Is it Seafood?

    -   Yes -> Stop

    -   No -> Is it Popcorn?

        -   No -> Carry On

        -   Yes -> Did you bring enough to share?

            -   Yes -> Carry On

            -   No -> Stop

How many scenarios end in “Stop”? “Carry on”?

---

```mermaid
graph TD
A[Where it started] --> B[What you need]
B --> C[Why pictures are better]
C --> F[Resources]
C --> E((Questions))
```


```mermaid
graph TD 
              st{HI!}
              good((Great))
              bad((Mizzz))
              en>Goodbye!]
              A((HI))
              style st fill:blue,fill-opacity:0.35,color:#FFFFFF,stroke-opacity:0.2
              style en fill:red,fill-opacity:0.35,color:#FFFFFF,stroke-opacity:0.2
              classDef eco fill:green;
              class A eco
```

```mermaid
graph TB
         A[13,032] --> |Accept John's Offer| B[12,000]
         A ==> |Reject John's Offer |C(($13,032))
         C --> |Offer from Vanessa 0.6| D[$14,000]
         D ==> |Accept Vanessa's Offer| E[$14,000]
         D --> |Reject Vanessa's Offer| F(($11,580))
         C --> |No Offer from Vanessa 0.4| G(($11,580))
         G --> |Salary 1 0.05| H[$21,600]
         G --> |Salary 2 0.25| I[$16,800]
         G --> |Salary 3 0.40| J[$12,800]
         G --> |Salary 4 0.25| K[$6,000]
         G --> |Salary 5 0.05| L[$0]
         F --> |Salary 1 0.05| M[$21,600]
         F --> |Salary 2 0.25| N[$16,800]
         F --> |Salary 3 0.40| O[$12,800]
         F --> |Salary 4 0.25| P[$6,000]
         F --> |Salary 5 0.05| Q[$0]

```

```mermaid
graph TB
    sq[Square shape] --> ci((Circle shape))

    subgraph A subgraph
        od>Odd shape]-- Two line<br>edge comment --> ro
        di{Diamond with <br/> line break} -.-> ro(Rounded<br>square<br>shape)
        di==>ro2(Rounded square shape)
    end

    %% Notice that no text in shape are added here instead that is appended further down
    e --> od3>Really long text with linebreak<br>in an Odd shape]

    %% Comments after double percent signs
    e((Inner / circle<br>and some odd <br>special characters)) --> f(,.?!+-*ز)

    cyr[Cyrillic]-->cyr2((Circle shape Начало));

     classDef green fill:#9f6,stroke:#333,stroke-width:2px,color:#00F;
     classDef orange fill:#f96,stroke:#333,stroke-width:4px;
     class sq,e green
     class di orange
```
