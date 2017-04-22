# veloheroup

Upload FIT, TCX, GPX, SRM, HRM, PWX, SLF and SLM files to [Velo Hero](http://www.velohero.com/) from the command line.

![Velo Hero Logo](https://www.velohero.com/static/touchicon.png)

## Prerequisites

* POSIX shell
* cURL

Most Linux distributions and macOS meet the requirements.

## Setup

1. Sign up at https://app.velohero.com/sso
2. Get yourself a private single sign-on key. That's the long string.
3. Create a `.veloherorc` file in your home directory:
~~~
VELOHERO_SSO_KEY=FIXME
~~~

## Usage

Upload a single file:

    veloheroup file.fit

Use find and xargs to upload everything:

    find -iname \*.fit | xargs veloheroup

## More info

Inspired by stravaup https://github.com/mpolla/stravaup