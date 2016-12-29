Heroku buildpack for Loklak: Java (uses Gradle)
===================================================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpack) made specifically for the [Loklak server](https://github.com/loklak/loklak_server). Forked from https://github.com/loklak/heroku_buildpack_gradle_loklak (Thanks!)
It uses the Gradle wrapper to build Loklak server and OpenJDK 1.8 (currently) to run it.

Usage
-----
This buildpack is meant to be used in conjuction with Loklak server only.

In your project directory:

1. Clone the Loklak server (if not already) : `git clone https://github.com/loklak/loklak_server.git`
2. Create a heroku app: `heroku create`
3. Set the buildpack: `heroku buildpacks:set https://github.com/loklak/heroku_buildpack_ant_loklak.git`
4. Push your app to heroku: `git push heroku master`
5. Confirm the loklak server is running: `heroku logs --tail`
6. Open the URL of your server in your browser: `heroku open`.
