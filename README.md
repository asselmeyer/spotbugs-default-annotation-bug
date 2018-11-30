# spotbugs-default-annotation-bug
A minimal example to illustrate [SpotBugs issue #805](https://github.com/spotbugs/spotbugs/issues/805), a problem concerning SpotBugs' null checks in combination with Eclipse JDT `@NonNullByDefault` and `@Nullable` annotations.

To observe the problem run SpotBugs, e.g. with `mvn clean verify`. SpotBugs reports a false-positive NP_NONNULL_RETURN_VIOLATION warning on `sample.withdefault.NullableSample.maybeNull()`.
