## [6.2.0](https://github.com/gparasyris/versioning-demo/compare/v6.1.0...v6.2.0) (2022-01-07)


### Bug Fixes

* **library:** remove codeship-related files ([c4d3d27](https://github.com/gparasyris/versioning-demo/commit/c4d3d27af025ebc5646b3efde86c0a2c13b8019b))
* **library:** testing steps on master only ([229bb6e](https://github.com/gparasyris/versioning-demo/commit/229bb6eb1e149e7f5127635abeb7b6ed9fba40f4))

## [6.1.0](https://github.com/gparasyris/versioning-demo/compare/v6.0.1...v6.1.0) (2022-01-07)

## [6.0.0](https://github.com/gparasyris/versioning-demo/compare/v5.3.0...v6.0.0) (2022-01-07)


### Bug Fixes

* **refactor:** dummy fix ([5f9fce5](https://github.com/gparasyris/versioning-demo/commit/5f9fce57314f01de4b0ef9c3feb75b1e5980ef08))


### Breaking

* codehsip steps added ([56eb878](https://github.com/gparasyris/versioning-demo/commit/56eb878e5da39cd4318948ff1562ecc259504ded))


### Chores

* **release:** [skip ci] 6.0.0 ([ad5910e](https://github.com/gparasyris/versioning-demo/commit/ad5910e28c774ebc59c6175280a3e5670f21027d))

## [6.0.0](https://github.com/gparasyris/versioning-demo/compare/v5.3.0...v6.0.0) (2022-01-07)


### Breaking

* codehsip steps added ([56eb878](https://github.com/gparasyris/versioning-demo/commit/56eb878e5da39cd4318948ff1562ecc259504ded))

## [5.3.0](https://github.com/gparasyris/versioning-demo/compare/v5.2.1...v5.3.0) (2021-11-25)


### Features

* **page:** home page now has category filtering ([50889dc](https://github.com/gparasyris/versioning-demo/commit/50889dcb8cfadc9c9356b1013e8b7e2304c090e7))

### [5.2.1](https://github.com/gparasyris/versioning-demo/compare/v5.2.0...v5.2.1) (2021-11-25)


### Bug Fixes

* **services:** fixed subject initial state ([da86751](https://github.com/gparasyris/versioning-demo/commit/da8675137794cde98de62d3570c831d21dfc9ef3))
* **services:** solved data issue in userservice ([0af11b6](https://github.com/gparasyris/versioning-demo/commit/0af11b6de90691b0866c8d1a987e625dd10177e1))

## [5.2.0](https://github.com/gparasyris/versioning-demo/compare/v5.1.0...v5.2.0) (2021-11-25)


### Updates

* **other:** releaserc update ([ab98ced](https://github.com/gparasyris/versioning-demo/commit/ab98ceda9779474379efbc853db9c28b387e149a))

## [5.1.0](https://github.com/gparasyris/versioning-demo/compare/v5.0.1...v5.1.0) (2021-11-25)


### New

* **component:** third component added ([01377cd](https://github.com/gparasyris/versioning-demo/commit/01377cd030c9f1dd8c5d9e54a10620950cb04be4))

# Changelog

All notable changes to this project will be documented in this file.



## Added

### Boost subscriptions can be migrated 
- When a user owns multiple homes and one of them has a boost subscription, this subscription can be migrated to a different home

### Angular 12 upgrade - Major Update
- Upgraded Angularjs to Angular 12 version, this is a major change that requires to clean and reinstall node_modules in local environments:
`$ rm -rf node_modules && npm i`, this has been tested with the pre-existing node version recommendation in the dockerfile (node v12).

### Home flags utilize dedicated endpoints 
- We no longer add/remove flags by updating the home entity in favour of the (pre-existing) dedicated endpoints.
- Related code has been added in `home.service.js`.

### Home flags utilize dedicated endpoints 
- We no longer add/remove flags by updating the home entity in favour of the (pre-existing) dedicated endpoints.
- Related code has been added in `home.service.js`.

### Minimize usage of `home.address` property
- Use `home.address` only as a fallback for cases when backend fails to provide separate address components;
- otherwise combine address on client side; including `state` for US addresses;
- affected addresses of home, user, home list, fullfilments.
### CD pipeline support 
- Add `push_image` with sha to codeship-steps for every branch


## [Unreleased]
