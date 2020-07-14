[![View Unit-Commitment-and-Economic-Dispatch on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://www.mathworks.com/matlabcentral/fileexchange/78125-unit-commitment-and-economic-dispatch)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

# Unit-Commitment-and-Economic-Dispatch
Matlab toolbox for the UC &amp; ED Calculation

## Installation

To run: double click on the .mlapp file.

![Image of package](https://github.com/AhmetTavli/Unit-Commitment-and-Economic-Dispatch/blob/master/install_pack.png)

## Demonstration

Open example [excel](https://github.com/AhmetTavli/Unit-Commitment-and-Economic-Dispatch/blob/master/project.xlsx)

![main_screen_excel](https://github.com/AhmetTavli/Unit-Commitment-and-Economic-Dispatch/blob/master/main_screen_excel.png)

Click Unit commitment

![uc](https://github.com/AhmetTavli/Unit-Commitment-and-Economic-Dispatch/blob/master/uc.png)

Click Economic dispatch

![ed](https://github.com/AhmetTavli/Unit-Commitment-and-Economic-Dispatch/blob/master/ed.png)

To see the summary:

![summary](https://github.com/AhmetTavli/Unit-Commitment-and-Economic-Dispatch/blob/master/uc_and_ed.png)

## Theory

Economic Dispatch Model:

<img src="https://i.upmath.me/svg/%C2%A0%5Ctext%7Bminimize%7D%5Csum_%7Bg%2Ct%7D%5E%7B%7D%20B_%7Bg%7DP_%7Bg%2Ct%7D%20" alt=" \text{minimize}\sum_{g,t}^{} B_{g}P_{g,t} " />

subject to

<img src="https://i.upmath.me/svg/%20%5Cunderline%7BP_%7Bg%7D%7D%20%5Cleq%20P_%7Bg%2Ct%7D%20%5Cleq%20%5Coverline%7BP_%7Bg%7D%7D%20%5Cquad%5Cforall%20g%5C%20%5Cforall%20t%C2%A0" alt=" \underline{P_{g}} \leq P_{g,t} \leq \overline{P_{g}} \quad\forall g\ \forall t " />

<img src="https://i.upmath.me/svg/%20%5Csum_%7Bg%7D%5E%7B%7D%20P_%7Bg%2Ct%7D%20%3D%20D_%7Bt%7D%20%5Cquad%20%5Cforall%20t%20" alt=" \sum_{g}^{} P_{g,t} = D_{t} \quad \forall t " />
