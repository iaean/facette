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

* check against KairosDB version during init to avoid API malfunction
* make the source tags list configurable  
  hard coded to `{"host", "name"}` at the moment
* make the interval for metrics population configurable  
  hard coded to 3600sec (1h) from now at the moment
* make metric aggregation function configurable by metric pattern  
  hard coded to the "max" of each 5min at the moment  
  each metric is aggregated at the moment, would be nice to graph raw data, too
* (Review) remove code for source/metric pattern matching?  
  KairosDB doesn't need it and the filter capability allows  
  to skip/modify source/metric names
* what's about different timezones between facette and the backend?

### Contribution
-----------------

All your contributions are welcome.


[0]: https://github.com/facette/facette
[1]: https://github.com/kairosdb/kairosdb
