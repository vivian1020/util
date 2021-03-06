Overview
--------

`util-stats <https://github.com/twitter/util/tree/master/util-stats/src/main/scala/com/twitter/finagle/stats>`_
is Twitter’s library for instrumenting Scala and Java code so that you know
what your application is doing in production. The API surface is small, with
the `StatsReceiver interface <https://github.com/twitter/util/blob/develop/util-stats/src/main/scala/com/twitter/finagle/stats/StatsReceiver.scala>`_
you get counters, gauges (value at a point in time) and stats (histograms).

Three provided Stats implementations are `finagle-stats <https://github.com/twitter/finagle/tree/master/finagle-stats>`_,
`finagle-ostrich <https://github.com/twitter/finagle/tree/master/finagle-ostrich4>`_,
and `finagle-commons-stats <https://github.com/twitter/finagle/tree/master/finagle-commons-stats>`_.
Our preferred implementation is finagle-stats.

A StatsReceiver provides the metrics within each node in your deployment.
