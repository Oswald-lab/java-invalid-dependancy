# 03-java-invalid-dependencies
Java source is valid; ONLY the dependency coordinates are broken, in both `pom.xml` and `build.gradle`.
Expected: resolution fails with "Could not resolve dependencies" / "Could not find ..." naming
`com.nonexistent.fakegroup:fake-artifact-does-not-exist:1.0.0` and `commons-lang3:99.99.99`.
Gradle plugin failure: uncomment the `com.nonexistent.fake-plugin` line in build.gradle.
