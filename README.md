# veloheroup

Upload FIT, TCX, GPX, SRM, HRM, PWX, SLF and SLM files to [Velo Hero](https://www.velohero.com/) from the command line.

![Velo Hero Logo](https://www.velohero.com/static/touchicon.png)

## Prerequisites

* Bash shell
* curl

Most Linux distributions and macOS meet the requirements.

## Setup

1. Sign up at https://app.velohero.com/sso
2. Get yourself a private single sign-on key. That's the long string.
3. Create a `.veloherorc` file in your home directory. Save the SSO key in this file:
~~~
VELOHERO_SSO_KEY=[insert your own]
~~~

## Usage

Upload a single file:

    veloheroup file.fit

Use find and xargs to upload everything:

    find -iname \*.fit | xargs veloheroup

## More info

Inspired by stravaup https://github.com/mpolla/stravaup