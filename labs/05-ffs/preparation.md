   **D-type FF**
   | **clk** | **d** | **q(n)** | **q(n+1)** | **Comments** |
   | :-: | :-: | :-: | :-: | :-- |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 0 | 0 | 0 | `q(n+1)` has the same level as `d` |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 0 | 1 | 0 | q is set to low |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 1 | 0 | 1 | q is set to high |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 1 | 1 | 1 | q is the same as before |

   **JK-type FF**
   | **clk** | **j** | **k** | **q(n)** | **q(n+1)** | **Comments** |
   | :-: | :-: | :-: | :-: | :-: | :-- |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 0 | 0 | 0 | 0 | Output did not change |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 0 | 0 | 1 | 1 | Output did not change |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 0 | 1 | 0 | 0 | Output did not change |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 0 | 1 | 1 | 0 | Output is set to low |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 1 | 0 | 0 | 1 | Output is set to low |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 1 | 0 | 1 | 1 | Output did not change |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 1 | 1 | 0 | 1 | Output is set to other state |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 1 | 1 | 1 | 0 | Output is set to other state |

   **T-type FF**
   | **clk** | **t** | **q(n)** | **q(n+1)** | **Comments** |
   | :-: | :-: | :-: | :-: | :-- |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 0 | 0 | 0 | Output did not change |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 0 | 1 | 0 | set to L |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 1 | 0 | 1 | set to H |
   | ![rising](https://github.com/tomas-fryza/digital-electronics-1/blob/master/labs/05-ffs/images/eq_uparrow.png) | 1 | 1 | 1 | Output did not change |
