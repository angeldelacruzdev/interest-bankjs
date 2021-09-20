[![Package Quality](https://packagequality.com/badge/interest-bankjs.png)](https://packagequality.com/#?package=interest-bankjs)

# LoanJS on TypeScript

 
Calculating loan in equal or diminishing installments - Loan TypeScript

You can use on NestJS Framwework, work nice.

- TypeScript: https://github.com/angeldelacruzdev/interest-bankjs 
- Javascript: https://github.com/kfiku/LoanJS 
 
## Getting Started

Install the module with: 
```
npm i interest-bankjs
```
 

#### Calculating Loan:
```js
import { Loan } from 'interest-bankjs';
var loan =  Loan(
  1000, // amount
  12,   // installments number
  5,    // interest rate
  true  // diminishing
);
/** returns
{ 
  installments  : [
    {
      capital     : number,
      interest    : number,
      installment : number,
      remain      : number
    }
  ],
  amount        : number,
  interestSum   : number,
  capitalSum    : number,
  sum           : number
}
*/
```

## Documentation

### Loan
Loan(amount, installmentsNumber, interestRate, diminishing)

### Arguments
| Argument           | type   | default   | Description
| ------------------ | ------ | --------- | ------------------
| amount             | number | *required | full amount of Loan
| installmentsNumber | number | *required | how many installments will be (in months)
| interestRate       | number | *required | interest rate in percent (ex. 3.5)
| diminishing        | bool   | false     | if installments will be - true: diminishing; false: equal/annuity

### Returns
```js
{ 
  installments  : [
    {
      capital     : number,
      interest    : number,
      installment : number,
      remain      : number
    }
  ],
  amount        : number,
  interestSum   : number,
  capitalSum    : number,
  sum           : number
}
```
 
## License

Copyright (c) 2014 Grzegorz Klimek   
Copyright (c) 2021 Angel De La Cruz  
Licensed under the MIT license.
