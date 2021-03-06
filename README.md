# Collection-Strawman

[![Join the chat at https://gitter.im/scala/collection-strawman](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/scala/collection-strawman?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Prototype improvements for Scala collections.

- [Gitter Discussion](https://gitter.im/scala/collection-strawman)
- [Dotty Issue](https://github.com/lampepfl/dotty/issues/818)
- [Scala Center Proposal](https://github.com/scalacenter/advisoryboard/blob/master/proposals/007-collections.md)

## Build

- Compile the collections and run the
  tests:
  
  ~~~
  >; compile; test
  ~~~
- Run the memory benchmark:
  
  ~~~
  > memoryBenchmark/charts
  ~~~
- Run the execution time benchmark:
  
  ~~~
  > timeBenchmark/charts
  ~~~

## Use it in your project

We published a 0.1.0 version so that you can experiment with the new design.
Note that most of the collection implementations are incomplete!

~~~ scala
libraryDependencies += "ch.epfl.scala" %% "collection-strawman" % "0.1.0"
~~~

Only Scala 2.12 is supported so far.

We also automatically publish snapshots on Sonatype:

~~~ scala
resolvers += Resolver.sonatypeRepo("snapshots")

libraryDependencies += "ch.epfl.scala" %% "collection-strawman" % "0.2.0-SNAPSHOT"
~~~