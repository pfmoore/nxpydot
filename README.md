A pydot compatibility wrapper for pydotplus
===========================================

NetworkX can use ```pydot``` for GraphViz support, but ```pydot``` doesn't
support Python 3. On the other hand, ```pydotplus``` supports Python 3,
but doesn't have an API that is compatible with pydot.

This package creates a wrapper around pydotplus that simply re-exports the
```pydotplus``` API under the name ```pydot``` and exposes an empty top-level
module ```dot_parser```. This is minimally sufficient to allow NetworkX to
work, at least to the extent of passing its ```pydot``` tests.

This project should *not* be installed if you have a working version of
```pydot```. It should also not be used for any purpose other than using
```pydotplus``` as the ```pydot``` back-end for NetworkX.
