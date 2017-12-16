# bignumber

Clojurescript wrapper library around [bignumber.js](https://github.com/MikeMcl/bignumber.js/). 

On contrary to the original library, if you pass non-bignumber value into a function, it doesn't throw an error, but fallbacks into `cljs.core` or `js/Math` equivalent. 

This library doesn't come with `cljsjs/bignumber`, because you might have bignumber.js included by other library, such as [web3.js](https://github.com/ethereum/web3.js/).

## Installation
Add `[district0x/bignumber "1.0.0"]` into your project.clj  
Include `[bignumber.core]` in your CLJS file.

## bignumber.core
**bignumber? [x]**  
True if number is BigNumber  

**number [x]**  
toNumber  

**abs [x]**    
abs  

### ceil [x]
ceil
### cmp [x & [base]]
cmp (comparedTo)
### dp [x]
dp (decimalPlaces)
### / [x y & [base]]
div
### div-to-int [x y & [base]]
divToInt
### = [x y & [base]]
equals
### floor [x]
floor
### > [x y & [base]]
greaterThan
BigNumbers are comparable event with native operators, so you don't need to use this one.
### >= [x y & [base]]
greaterThanOrEqualTo
BigNumbers are comparable event with native operators, so you don't need to use this one.
### finite? [x]
isFinite
### int? [x]
isInt
### nan? [x]
isNaN
### neg? [x]
isNeg
### zero? [x]
isZero
### < [x y & [base]]
lessThan
BigNumbers are comparable event with native operators, so you don't need to use this one.
### <= [x y & [base]]
lessThanOrEqualTo
BigNumbers are comparable event with native operators, so you don't need to use this one.
### - [x y & [base]]
minus
### mod [x y & [base]]
mod
### neg [x]
negated
### + [x y & [base]]
plus
### sd [x & [z]]
significantDecimals
### round [x & [dp rm]]
round
### shift [x z]
shift
### sqrt [x]
sqrt
### * [x y & [base]]
times
### digits [x & [sd rm]]
toDigits
### exponential [x & [dp rm]]
toExponential
### fixed [x & [dp rm]]
toFixed
### format [x & [dp rm]]
toFormat
### fraction [x & [max]]
toFraction
### json [x]
toJSON
### pow [x n & [m]]
pow
### precision [x & [sd rm]]
toPrecision
### trunc [x]
trunc
### value-of [x]
valueOf


