# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.10.1] - 2019.05.08
- Added import of magento 2 cms pages and blocks to the full import - @toh82 (#235)
- Added information about magento 2 cms pages and blocks import to the readme - @toh82 (#235)

## [1.10.0-rc.1] - UNRELEASED

### Added
- Typescript support - @ResuBaka (#210, #242)
- Multi Stock Inventory (Magento MSI) support - @aleron75, @dimasch (#226)

### Fixed
- Missing `res` and `req` parameters are now passed to ProductProcessor - @jahvi (#218)
- fixed moving of graphql files to the dist folder @ResuBaka (#242)
- fixed moving of schema files to the dist folder @ResuBaka (#244)
- fixed missing assetPath config for magento1  @ResuBaka (#245)

## [1.9.2] - 2019.05.20
- Fix failing o2m when parsing order schema - @lukeromanowicz (#248)

## [1.9.1] - 2019.05.10
- Mount ElasticSearch data to `docker/elasticsearch/data` directory - @dimasch, @lukeromanowicz (#237, #241)
- Fix product schema and importer in migration process - @lukeromanowicz (#239)

## [1.9.0] - 2019.05.06
- Changed location of magento1 platform js client. Moved from `src/platform/magento1/module` to [magento1-vsbridge-client](https://github.com/DivanteLtd/magento1-vsbridge-client) - @mtarld (#195)
- Update Babel from 6 to 7 - @lukeromanowicz (#202)
- Support unicode characters in order requests - @lukeromanowicz (#201)
- TravisCI configured for building and linting - @lukeromanowicz (#204)
- Use Redis database from configuration in mage2vs - @Cyclonecode (#211)
- Requests with invalid body result in HTTP code 400 instead of 500 - @AndreiBelokopytov (#220) 
- `src/models/order.schema.json` was moved to `src/models/order.schema.js` to support regex transformation - @lukeromanowicz (#201)

## [1.8.4] - 2019.04.17
- Use encrypted token for user authentication - @pkarw (#215)

## [1.8.3] - 2019.03.05
- Use store id from configuration in `mage2vs import` - @boehsermoe (#179)

## [1.8.2] - 2019.03.04
- Magento 1 bridge client - @afirlejczyk (#190)
- configurable ElasticSearch `apiVersion` - @Resubaka (#192)

## [1.8.1] - 2019.02.11
- Fixed `apiVersion` property for ElasticSearch driver - now it's available thru `config/*.json` - @mdanilowicz (#185)