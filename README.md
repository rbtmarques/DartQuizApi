
# Quiz API Dart

An application built with [aqueduct](https://github.com/stablekernel/aqueduct).

# Topics Covered
* [x] [How to Setup Aqueduct ?](https://youtu.be/rf6uAcAglzc)
* [x] [How to write your first REST API ?](https://youtu.be/rf6uAcAglzc)
* [x] [How to make controllers ?](https://youtu.be/XCOYxjoJDb8)
* [x] [Indexing And Routing ?](https://youtu.be/zG1kUp1bcQY)
* [x] [How to write tests ?](https://youtu.be/Q2I4wDET4Os)
* [x] [How to setup PostgreSQL ?](https://youtu.be/WrqUOZw1E7w)
* [x] [How to write tests with test db ?](https://youtu.be/JsPFOh3SPm0)
* [x] [What is ORM ?](https://youtu.be/JsPFOh3SPm0)
* [x] [How to make DataModels ?](https://youtu.be/JsPFOh3SPm0)
* [x] [What are Relationships and Joins ?](https://youtu.be/TWhCHoGds0c)
* [x] [How to deploy to real database ?](https://youtu.be/6H3XwY_G8JA)

# YouTube Tutorial Playlist 
[Dart Aqueduct Backend Series For Beginners Tutorial](https://www.youtube.com/playlist?list=PLR2qQy0Zxs_U3RMzoAXeC6_c5Dv43t8P-)

## Running the Application in Development

Run `aqueduct serve` from this directory to run the application.

If you wish to use the debugger in your IDE, run the `bin/main.dart` script from your IDE.

## Running Application Tests

To run all tests for this application, run the following in this directory:

```
pub run test
```

You may also run tests from an IntelliJ IDE by right-clicking on a test file or test case and selected 'Run tests'.

Tests will be run using the configuration file `config.src.yaml`. This file should contain  test configuration values and remain in source control. This file is the template for `config.yaml` files, which live on deployed server instances.

See the application test harness, `test/app/harness.dart`, for more details. This file contains a `TestApplication` class that can be set up and torn down for tests.

For more information, see [Getting Started](https://aqueduct.io/docs/) and [Testing](https://aqueduct.io/docs/testing/overview).

## Application Structure

Routes and other initialization are configured in `lib/quiz_api_sink.dart`. Endpoint controller files are in `lib/controller/`.

## Configuration

The file `config.src.yaml` is used for testing: it should be checked into source control and contain values for testing purposes. It should maintain the same keys as `config.yaml`.

## Creating API Documentation

In the project directory, run:

```bash
aqueduct document
```

This will print a JSON OpenAPI specification to stdout.

## Deploying an Application

See the documentation for [Deployment](https://aqueduct.io/docs/deploy/overview/).
