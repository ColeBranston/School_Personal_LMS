**Sacrificial (throw-away) candidate solutions** are several deliberately different [[Prototyping|prototypes]] of a solution, built to be discarded. One candidate isn't enough to open your mind to all the possibilities — generating many forces you (and stakeholders) to explore the problem space, and the comparison reveals the real requirements.

> [!quote] "If you want to have a good idea, have lots of ideas." — Linus Pauling

**Example:** college students must acquire the textbooks required for their courses. Five candidates:

*Five candidate solutions to the textbook problem (slide 8)*

```mermaid
flowchart LR
    subgraph c1["1"]
        a1["Buy the book at a bookstore / Amazon"]
    end
    subgraph c2["2"]
        b1["Student (reading list)"] --> b2["Searches second-hand booksellers"] --> b3["Pays"] --> b4["Waits for delivery"]
    end
    subgraph c3["3"]
        d1["Professor uploads the list"] --> d2["Student selects a book"] --> d3["Print-on-demand service"] --> d4["Mailed to student"]
    end
    subgraph c4["4"]
        e1["Student goes to campus bookstore and selects a book"] --> e2["Espresso printer prints the book in five minutes"]
    end
    subgraph c5["5"]
        f1["Reading list"] --> f2["Student downloads the book to her tablet"]
    end
```
