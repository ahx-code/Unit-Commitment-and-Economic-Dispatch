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

### Economic Dispatch

<img src="https://i.upmath.me/svg/%C2%A0%5Ctext%7Bminimize%7D%5Csum_%7Bg%2Ct%7D%5E%7B%7D%20B_%7Bg%7DP_%7Bg%2Ct%7D%20" alt=" \text{minimize}\sum_{g,t}^{} B_{g}P_{g,t} " />

subject to

<img src="https://i.upmath.me/svg/%20%5Cunderline%7BP_%7Bg%7D%7D%20%5Cleq%20P_%7Bg%2Ct%7D%20%5Cleq%20%5Coverline%7BP_%7Bg%7D%7D%20%5Cquad%5Cforall%20g%5C%20%5Cforall%20t%C2%A0" alt=" \underline{P_{g}} \leq P_{g,t} \leq \overline{P_{g}} \quad\forall g\ \forall t " />

<img src="https://i.upmath.me/svg/%20%5Csum_%7Bg%7D%5E%7B%7D%20P_%7Bg%2Ct%7D%20%3D%20D_%7Bt%7D%20%5Cquad%20%5Cforall%20t%20" alt=" \sum_{g}^{} P_{g,t} = D_{t} \quad \forall t " />

### Unit Commitment

<img src="https://i.upmath.me/svg/%20%5Ctext%7Bminimize%7D%5Csum_%7Bt%2Cg%7D%5E%7B%7D%20B_%7Bg%7DP_%7Bg%2Ct%7D%5Cbeta%20%2B%20C_%7Bg%7Ds_%7Bg%2Ct%7D%20%2B%20E_%7Bg%7Dh_%7Bg%2Ct%7D%20%2B%20A_%7Bg%7Du_%7Bg%2Ct%7D%20" alt=" \text{minimize}\sum_{t,g}^{} B_{g}P_{g,t}\beta + C_{g}s_{g,t} + E_{g}h_{g,t} + A_{g}u_{g,t} " />

subject to

<img src="https://i.upmath.me/svg/%20u_%7Bg%2Ct%7D%5Cunderline%7BP_%7Bg%7D%7D%5Cleq%20P_%7Bg%2Ct%7D%5Cleq%5Coverline%7BP_%7Bg%7D%7Du_%7Bg%2Ct%7D%5Cquad%5Cforall%20g%5C%20%5Cforall%20t%5C%5C%5C%5C%0A-R_%7Bg%7D%5E%7BD%7D%5Cleq%20P_%7Bg%2Ct%7D%20-%20P_%7Bg%2C(t-1)%7D%5Cleq%20R_%7Bg%7D%5E%7BU%7D%5Cquad%5Cforall%20g%5C%20%5Cforall%20t%5C%5C%5C%5C%0A%5Csum_%7B%5Ctau%3D1-M_%7Bg%7D%5E%7BU%7D%2B1%7Ds_%7Bg%2Ct%7D%5Cleq%20u_%7Bg%2Ct%7D%5Cquad%5Cforall%20g%5C%20%5Cforall%20t%5C%5C%5C%5C%0A%5Csum_%7B%5Ctau%3D1-M_%7Bg%7D%5E%7BD%7D%2B1%7Dh_%7Bg%2Ct%7D%5Cleq%201-u_%7Bg%2Ct%7D%5Cquad%5Cforall%20g%5C%20%5Cforall%20t%5C%5C%5C%5C%0As_%7Bg%2Ct%7D-h_%7Bg%2Ct%7D%3Du_%7Bg%2Ct%7D-u_%7Bg%2Ct-1%7D%5Cquad%5Cforall%20g%5C%20%5Cforall%20t%5C%5C%5C%5C%0A%5Csum_%7Bg%7D%5Coverline%7BP_%7Bg%7D%7Du_%7Bg%2Ct%7D%5Cgeq%20D_%7Bt%7D%2BR_%7Bt%7D%5Cquad%5Cforall%20t" alt=" u_{g,t}\underline{P_{g}}\leq P_{g,t}\leq\overline{P_{g}}u_{g,t}\quad\forall g\ \forall t\\\\
-R_{g}^{D}\leq P_{g,t} - P_{g,(t-1)}\leq R_{g}^{U}\quad\forall g\ \forall t\\\\
\sum_{\tau=1-M_{g}^{U}+1}s_{g,t}\leq u_{g,t}\quad\forall g\ \forall t\\\\
\sum_{\tau=1-M_{g}^{D}+1}h_{g,t}\leq 1-u_{g,t}\quad\forall g\ \forall t\\\\
s_{g,t}-h_{g,t}=u_{g,t}-u_{g,t-1}\quad\forall g\ \forall t\\\\
\sum_{g}\overline{P_{g}}u_{g,t}\geq D_{t}+R_{t}\quad\forall t" />

## Contributing :thought_balloon:
Pull requests are welcome.

For major changes, please open an issue, then discuss what you would like to change.
