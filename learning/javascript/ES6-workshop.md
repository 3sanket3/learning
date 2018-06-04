* ES6 to improve the redability
* declarative vs imparative

#### Arrow Function

* don't have `this`, so really helpful to handle `this`
* being anonymouse in most of the places, makes harder to ready, instead a function name itself would give more idea
* when to have () , {}, cleared

#### var

* a generalized variable avaialble in the IIFI
* even if redeclared, no new space will be allocated (will be the same variable even in for(var i))

#### let

* limitted to the current block scope
* can't be re declatred

#### const

* variable can't be re-assigned, but it is not the constant by value

#### default value

* `function (x=2){ }`
* `function (x= foo())`, foo will only be eveluated if no data is passed
