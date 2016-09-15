# veloheroup
Upload FIT, TCX, GPX, SRM, HRM, PWX, SLF and SLM files to [Velo Hero](http://www.velohero.com/) from the command line.

## Prerequisites
* POSIX shell
* cURL

## Setup
1. Sign up at https://app.velohero.com/sso
2. Get yourself a private single sign-on key. That's the long string after private_key=.
3. Create a .veloherouprc file in your home directory:
~~~
VELOHEROUP_SSO_KEY=FIXME
~~~

## Usage
Upload a single file:

    veloheroup file.fit

Use find and xargs to upload everything:

    find -iname \*.fit | xargs veloheroup

## More info

Inspired by stravaup from inspired by mpolla https://github.com/mpolla/stravaup