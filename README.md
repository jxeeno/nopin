# nopin

Tool that automatically compiles, patches and resigns an Android Application Package (.apk) to bypass Certificate Pinning functionality implemented using OkHttp3.

## Dependents

This docker image uses:

* apktool 2.3.1
* zipalign
* jarsigner
* keytool

## Usage

1. Clone this repo
2. Build: `docker build -t <username>/nopin .`
3. Run: `docker run -v $(pwd):/app <username>/nopin lolapp.apk`

Outputs `SIGNED_lolapp.apk`