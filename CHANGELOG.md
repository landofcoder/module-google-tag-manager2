# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [3.0.6] - 31 December 2022
### Fixed
- Prevent reloading order per order-item

## [3.0.5] - 21 December 2022
### Fixed
- Render debugging block only if available

## [3.0.4] - 17 December 2022
### Fixed
- Finalize product clicks for Hyva
- Fix typo in payment validator

## [3.0.3] - 13 December 2022
### Fixed
- Hyva event handling

## [3.0.2] - 13 December 2022
### Fixed
- Basic compatibility with Hyva

## [3.0.1] - 13 December 2022
### Fixed
- Backend model prevents saving container ID

## [3.0.0] - 12 December 2022
### Added
- GA4 support
- Removed GA4/UA/EE support
- Extensibility via XML layout
- Support for EAV attributes of products and categories
- Click events
- Cart & checkout events 
- Integration Tests

## [2.1.8] - 1 July 2022
### Fixed
- Update ecommerce attributes #95 (@BorisovskiP)

## [2.1.7] - 31 March 2022
### Fixed
- Prevent adding quote data to success page #91
- Add additional field for ecommerce push #93 (@sprankhub)

### Fixed
- Prevent adding quote data to success page #91
- Add additional field for ecommerce push #93 (@sprankhub)

## [2.1.7] - 31 March 2022
### Fixed
- Prevent adding quote data to success page #91
- Add additional field for ecommerce push #93 (@sprankhub)

## [2.1.6] - 23 March 2022
### Fixed
- Add ecommerce push on checkout success #90 (@sprankhub)

## [2.1.5] - 21 March 2022
### Fixed
- Fix Duplicate Product Tracking #88 (@sprankhub)
- Add parent SKU #89 (@sprankhub)

## [2.1.4] - 17 February 2022
### Fixed
Fix duplicate product loading #85 (@sprankhub)


## [2.1.3] - 23 September 2021
### Fixed
- Prevent Fatal Error with `Amasty_Xlanding`

## [2.1.2] - 29 July 2021
### Fixed
- Fix error on cart configure page (@Irinina)

## [2.1.1] - 10 July 2021
### Fixed
- Make sure \Yireo\GoogleTagManager2\ViewModel\Product::getProductPrice() always returns float

## [2.1.0] - 10 July 2021
### Fixed
- Various styling issues (PHPCS, PHPStan)
- Increase framework requirement to 101.2 because of ViewModel bug

### Added
- Enabled debugging in JS (dumping attributes and config)
- New Attributes ViewModel to collect data after initialize output
- Add API interfaces to guarantee backwards compatibility in future
- Added XML layout container `gooogletagmanager_container` for most datalayer blocks
- Added debug utility class
- Renamed existing plugin interceptors

### Removed
- Rewrite x-magento-init into simple require() for performance
- Refactored `Category` block to no longer depend on `onLoadedProductCollection`
- Removed all block classes (`Script`, `Category`, `Product`, `Generic`, `Custom`)
- Remove `\Yireo\GoogleTagManager2\Util\GetCurrentProduct`
- Remove `\Yireo\GoogleTagManager2\Util\GetCurrentCategory`
- Remove helper
- Remove container model
- Remove entire observer-based input method
- Remove ViewModelFactory

## [2.0.5] - 5 May 2021
### Fixed
Re-add CSP whitelisting

## [2.0.4] - 30 April 2021
### Fixed
- Fix block retrieval with Layout instead LayoutFactory (@sprankhub)
- Make sure view model is set correctly (@sprankhub)

## [2.0.3] - 29 October 2020
### Fixed
- Fix error when block is not present

## [2.0.2] - 28 October 2020
### Fixed
- Category Sort By not working properly with 2.4.X because of weird product loading (70)
- Refactored legacy Registry into request
- Move Config class to new namespace
- PHPCS fixes for Magento Marketplace compliance

## [2.0.1] - 29 July 2020
### Added
- Magento 2.4 support

## [2.0.0] - 2020-07-21
### Removed
- Legacy CustomerData class
- Dev dependency with Mockery

### Fixed
- Upgrade PHPUnit to be 2.4 compatible
- Bumped minimum PHP to 7.2

## [1.1.3] - 2020-05-30
### Fixed
- Add a new CSP whitelist for M2.3.5+

## [1.1.2] - 2020-03-31
### Fixed
- Some small code quality things

## [1.1.1] - 2020-02-10
### Added
- Add ACL file for configuring access to config

## [1.1.0] - 2019-11-23
### Added
- Major rewrite to remove custom sections in favor of DI plugin
- No more reloading of sections

## [1.0.3] - 2019-08-07
### Fixed
- Use currency code instead of currency symbol (@nicolas-medina)

## [1.0.2] - 2019-06-15
### Fixed
- Move cookie-restriction-mode to JS to work with FPC

## [1.0.1] - 2019-03-13
### Fixed
- Fix duplicate code
- Add compatibility with Magento 2.2 again (2.1 is dropped permanently)
- Fix invalid template path
- Fix reloading issues with quote

## [1.0.0] - 2019-02-26
### Fixed
- First release with Changelog
- See GitHub commits for earlier messages
