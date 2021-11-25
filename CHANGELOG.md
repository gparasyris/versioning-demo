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
