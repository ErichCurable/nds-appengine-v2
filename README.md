nds
===

This is a datastore library for Google App Engine.

You can find API documentation at [http://godoc.org/github.com/qedus/nds](http://godoc.org/github.com/qedus/nds).

Its aim is to follow some of the feature set of Python ndb but still conforming to the App Engine datastore API.

The most compelling feature would be to properly implement local caching and memcaching of datastore calls. To do this properly is tricker than it might first seem. I have not come across a single Go implementation that does this correctly.

Right now only the GetMulti function does anything - which is to overcome the entity retrieval maximum of 1000 entities.

TODO
===
- Implement the NDB strategy for keeping caches in sync with the datastore.
