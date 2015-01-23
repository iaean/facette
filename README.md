![logo](https://cloud.githubusercontent.com/assets/1122379/3501756/07726d40-061a-11e4-8ffa-bbaa6cf3adfb.png)

This is a fork of [Facette][0], to provide a [KairosDB][1] connector for it.
C*/KairosDB is a fast scalable time series sink, but it seems to lack an
user friendly ad-hoc instant graphing capability. Hoping by providing a connector,
facette can deal with this.

### Status
----------

still functional with KairosDB 0.9.4 (< 0.9.4 untested)...

...but there is sufficient scope for reviews and enhancements

### TODO / Review
-----------------

* [x] check against KairosDB version during init  
API is stable between 0.9.4 and upcoming 0.9.5  
[see here](https://github.com/kairosdb/kairosdb/issues/141)
* [x] make the source tags list configurable
* [x] make the interval for metrics population configurable
* [x] make metric aggregation function configurable by metric pattern
* [ ] what's about different timezones between facette and the backend?

### Contribution
-----------------

All your contributions are welcome.


[0]: https://github.com/facette/facette
[1]: https://github.com/kairosdb/kairosdb
