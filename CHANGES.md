0.2.1
====

* Exposes `throwE` and `catchE`.
* Add `transformers-compat` for old versions of transformers that require
  `throwE`, `catchE`.
* Fix `safe` version bounds for new versions.
* Add `mapExceptT and `withExceptT`.
* Export `scanl'` and provide shim for backwards compatability.
* Add `putErrLn`.
* Expose `RealFloat`.
* Expose `GHC.Records` exports for GHC 8.2 and above.

0.2
====

* Expose `Symbol` and `Nat` types from `GHC.TypeLits` by default.
* Switch exported `(<>)` to be from `Data.Monoid` instead of Semigroup.
* Expose `putByteString` and `putLByteString` monomorphic versions of `putStrLn` functions
* Export `genericLength` and other generic list return functions.
* Rename `msg` to `fatalErrorMessage`.
* Export `ExceptT`, `ReaderT`, and `StateT` constructors.
* Mask `displayException` from default exports.
* Mask `stToIO` from default exports.
* Export `NonEmpty` type and constructor for Base 4.9 only.
* Export `Data.Semigroup` type and functions for Base 4.9 only.
* Restrict exported symbols from ``async`` to set available in 2.0.
* Add `(&&^)`, `(||^)`, `(<&&>)`, `(<||>)`
* Expose `unzip`.
* Export `maximumMay` and `minimumMay`.
* Mask `Type` export from `Data.Kind`.
* Wrap `die` to take `Text` argument instead of `[Char]`.
* Export constructors `GHC.Generics`: `(:+:)`, `(:*:)`, and `(:.:)`.
* Expose `StablePtr`, `IntPtr` and `WordPtr` types.

0.1.9
====

* Make `sum` and `product` strict

0.1.8
=====

* ``foreach`` for applicative traversals.
* ``hush`` function for error handling.
* ``tryIO`` function for error handling.
* ``pass`` function for noop applicative branches.
* Mask ``Handler`` typeclass export.
* Mask ``yield`` function export.

0.1.7
=====

* Exports monadic ``(>>)`` operator by default.
* Adds ``traceId`` and ``traceShowId`` functions.
* Exports``reader`` and ``state``  functions by default.
* Export lifted ``throwIO`` and ``throwTo`` functions.

0.1.6
=====

* Adds uncatchable panic exception throwing using Text message.
* Removes ``printf``
* Removes ``string-conv`` dependency so Stack build works without ``extra-deps``.
* Brings ``Callstack`` machinery in for GHC 8.x.
* Removes ``throw`` and ``assert`` from ``Control.Exception`` exports.
* Removes ``unsafeShiftL`` and ``unsafeShiftR`` from ``Data.Bits`` exports.
* Reexport ``throw`` as ``unsafeThrow`` via Unsafe module.
* Hides all Show class functions. Only the Class itself is exported. Forbids custom instances that are not GHC derived.
* Export`` encodeUtf8`` and ``decodeUtf8`` functions by default.
* Adds ``unsnoc`` function.

0.1.5
=====

* Initial release.
