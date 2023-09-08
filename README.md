To reproduce:

- Make sure you're running node 20.6.0
- Run `yarn`
- Run `node ./test.cjs`. This works fine
- Run `node ./test.js`. This throw the following error:

```
class MultiSamlStrategy extends strategy_1.AbstractStrategy {
                                           ^

TypeError: Class extends value undefined is not a constructor or null
    at Object.<anonymous> (~/saml/node_modules/@node-saml/passport-saml/lib/multiSamlStrategy.js:6:44)
    at Module._compile (node:internal/modules/cjs/loader:1241:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1295:10)
    at Module.load (node:internal/modules/cjs/loader:1091:32)
    at Module._load (node:internal/modules/cjs/loader:938:12)
    at Module.require (node:internal/modules/cjs/loader:1115:19)
    at require (node:internal/modules/helpers:130:18)
    at Object.<anonymous> (~/saml/node_modules/@node-saml/passport-saml/lib/index.js:21:29)
    at Module._compile (node:internal/modules/cjs/loader:1241:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1295:10)

Node.js v20.6.0
```
