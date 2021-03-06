# Release Notes

## June 1, 2020

### iOS Analytics 2.2.4

* Fixed incorrect timezone offset calculation
* Fixed a crash which happened in Analytics::TrackLifecycle

## March 2, 2020

The following updates were made in this release:

### iOS Analytics 2.2.3

* `AnalyticsResponse` events are now always dispatched regardless if the debugApi is enabled or if AAM forwarding is enabled.
* Report extension details to ACPCore for improved logging and Griffon support.
* Improved existing log messages and added additional logging to assist with debugging.

## February 13, 2020

The following updates were made in this release:

### Android Analytics 1.2.4

* Fixed an issue which, was causing some hits to be delayed.
* Fixed an issue where `AnalyticsResponse` events were not being dispatched even when the debug API was enabled.
* Report extension details to Mobile Core for improved logging and Griffon support.
* Improved existing log messages and added additional logging to assist with debugging.

## January 25, 2020

The following updates were made in this release:

### Android Analytics 1.2.3 and iOS Analytics 2.2.2

* `requestEventIdentifier` is now appended to all non-track events so that Lifecycle \(or other extension events that are sent to Analytics\) can be viewed with rich detail in Project Griffon.

## October 28, 2019

The following change was made in this release:

### iOS Analytics 2.2.1

* Analytics response content events now contain two new fields:
  * `hitHost`
  * `hitUrl`

These fields contain the host and URL of the of the hit responsible for dispatching the response event.

### Android Analytics 1.2.2

* Analytics response content events now contain two new fields:
  * `hitHost`
  * `hitUrl`

These fields contain the host and URL of the of the hit responsible for dispatching the response event.

## October 7, 2019

The following updates were made in this release:

### Android Analytics 1.2.1

* Fixed a bug where, on start up, the Analytics database was being modified by multiple threads.

## September 10, 2019

The following updates were made in this release:

### Android Analytics 1.2.0

* Added the following new pieces of data when reporting a crash:
  * `previousosversion`
  * `previousappid`
* Added support for the Griffon debug API.
* The `global.ssl` configuration settings are ignored, and SSL is enabled by default.

### iOS Analytics 2.2.0

* Added support for Griffon debug API.
* The `global.ssl` configuration settings are ignored, and SSL is enabled by default.

## July 9, 2019

The following updates were made in this release:

### iOS Analytics 2.1.2

* ACPAnalytics now correctly identifies Acquisition link event types.
* Fixes a compile-time error when using the “-all\_load” linker flag.

