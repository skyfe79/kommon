#### Kommon Overview

Kommon is a "commons" library for Kotlin.

It fills in a few gaps in Kotlin's current standard library and will hopefully cease to exist
as the standard library matures.

##### Status

Unstable and not for production use.

##### Features

Current functionality is largely to support scripting use cases such as executing shell commands. e.g.

```kotlin
import com.github.andrewoma.kommon.script.*

val out = shell("ls -lah").out
val out = shell("echo \$HELLO \$WORLD", environment = mapOf("HELLO" to "foo", "WORLD" to "bar")).out
```

See the [tests](/src/test/kotlin/com/github/andrewoma/kommon) for more examples.

#### License
This project is licensed under a MIT license.

[![Build Status](https://travis-ci.org/andrewoma/kommon.svg?branch=master)](https://travis-ci.org/andrewoma/kommon)