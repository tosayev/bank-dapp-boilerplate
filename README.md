# Cadena Bank DAPP
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

This is the completed code for the Bank DAPP.

## To Install

Clone the project and run:

### `npm install`
### `npm start`


## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://harlandlohora.com/"><img src="https://avatars.githubusercontent.com/u/26666489?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Harland Lohora</b></sub></a><br /><a href="https://github.com/CadenaDev/bank-dapp-boilerplate/issues?q=author%3AHarlandLohora" title="Bug reports">🐛</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

## Building a DApp
Next part of the lesson covered building a dapp which was incredibly exciting, especially for me after being a regular user of many dapps.

The section was tough, very dense but the structure was easy to follow.  Only issues I faced:
1. Forgot quotations around the contract address in App.js which made the app read the address as a number in hex.
2. Kept getting an error in `withDrawMoneyHandler` which turns out was due to a simple case error.  In BankContract.sol, the function is defined as `withdrawMoney(address payable _to, uint256 _total)` but I had forgotten about that and just followed the course instruction.  In the course instruction, in App.js, the used case is `withDrawMoney` so I just blindly typed that into App.js without looking back to what I had used in BankContract.sol.  Anyway, was pretty easy to find and resolve & I also made a pull request to correct the code in the course.

After following all the steps and deploying my first dapp ever (deployed locally), it was an incredible moment.  My end result exactly matched the [final product](https://cadena-bank-dapp.vercel.app/) demonstrated in the course.

I could deposit, withdraw, rename the bank.  Just like that - from zero knowledge of Solidity, dapps, Smart Contracts, etc. to deploying an app in 2 days with a very well designed course...for free!
