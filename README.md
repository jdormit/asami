# asami [![Build Status](https://travis-ci.org/threatgrid/asami.svg?branch=master)](https://travis-ci.org/threatgrid/asami)

An implementation of the Naga storage protocol in memory.

[![Clojars Project](http://clojars.org/org.clojars.quoll/asami/latest-version.svg)](http://clojars.org/org.clojars.quoll/asami)

This has a query API that looks very similar to a simplified Datomic.

## Usage

Create a store with:

`(asami.core/create-store config)`

Where _config_ is a standard Naga config, but will be ignored.

Alternatively, just use the `asami.core/empty-store` object.

Add data with:
`naga.store/assert-data`

Query using:
`naga.store/query`

Look at the `naga.store/Storage` protocol (in [threatgrid/naga-store](https://github.com/threatgrid/naga-store) ) for the full suite of functions to apply to the storage.

## License

Copyright © 2018 Cisco

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
