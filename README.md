# dependency-sanity-test

Throwaway repo to smoke-test [lhein/dependency-sanity-action](https://github.com/lhein/dependency-sanity-action).

Layout:

- `module-a/pom.xml`, `module-b/pom.xml` — Maven multi-module reactor
- `gradle-module-a/build.gradle` — Gradle project with Groovy DSL
- `gradle-module-kts/build.gradle.kts` — Gradle project with Kotlin DSL

Open a PR that bumps a dependency in any of those build files and the action
posts a diff report as a comment.
