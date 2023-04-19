heroku-buildpack-grpc
====

Add a GRPC PECL extencion to your build.

## Usage

1. Add the buildpack to your project.toml file in your app:

    ```
    ...
    [[build.buildpacks]]
    uri = "fagianijunior/grpc"

    [[build.buildpacks]]
    uri = "heroku/php"
    ```

    Keep in mind that the buildpack order is important. If you'll specify this buildpack after your default one (e.g. `heroku/php`) it'll not work. See [https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app) for details.

2. Done