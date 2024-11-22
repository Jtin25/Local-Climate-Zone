<div align="center">
  <p>
        <img src="images/LCZprocess.png" width="600">
</p>
</div>

# Introduction
A GIS-based Local Climate Zone mappong
| Band Value | LCZ | Label |
|----------|----------|----------|
| 1 | B | Scattered trees |
| 2 | D | Low plants |
| 3 | 8 | Large lowrise |
| 4 | 9 | Sparsely built |
| 5 | G | Water |
| 6 | A | Dense trees |
| 7 | F | Bare soil or sand |
| 8 | E | Bare rock or paved |
| 9 | 6 | open lowrise |
| 10 | 5 | open midrise |

# Evaluation
| LCZ | B | D | 8 | 9 | G | A | F | E | 6 | 5 | Total | User Accuracy |
|-----|---|---|---|---|---|---|---|---|---|---|-------|---------------|
|  B  | 7 | 1 | 0 | 0 | 1 | 0 | 0 | 0 | 1 | 0 |  10   |     0.7       |
|  D  | 4 | 46| 1 | 2 | 0 | 2 | 0 | 0 | 0 | 0 |  55   |     0.84      |
|  8  | 0 | 0 | 9 | 0 | 0 | 0 | 0 | 0 | 1 | 0 |  10   |     0.9       |
|  9  | 1 | 0 | 0 | 9 | 0 | 0 | 0 | 0 | 0 | 0 |  10   |     0.9       | 
|  G  | 0 | 0 | 0 | 0 | 10| 0 | 0 | 0 | 0 | 0 |  55   |     1         |
|  A  | 1 | 0 | 0 | 0 | 0 | 9 | 0 | 0 | 0 | 0 |  10   |     0.9       |
|  F  | 0 | 1 | 2 | 1 | 0 | 0 | 3 | 0 | 3 | 0 |  10   |     0.3       | 
|  E  | 0 | 1 | 0 | 0 | 0 | 0 | 0 | 9 | 0 | 0 |  10   |     0.9       |
|  6  | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 15| 0 |  15   |     1         |
|  5  | 0 | 1 | 3 | 0 | 0 | 0 | 0 | 0 | 0 | 6 |  10   |     0.6       |
|Total| 13| 50| 15| 12| 11| 11| 3 | 9 | 20| 6 |  150  |               |
|Producer Accuracy| 0.54 | 0.92 | 0.6 | 0.75 | 0.91 | 0.82 | 1 | 1 | 0.75 | 1 |     |     0.82       |
