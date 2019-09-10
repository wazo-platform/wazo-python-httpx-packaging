# wazo-python-httpx-packaging

Debian packaging for [python3-httpx](https://github.com/encode/httpx/) used in Wazo.

## Upgrading

To upgrade python-httpx

* Update the version number in the `VERSION` file
* Update the changelog using `dch -i` to the matching version
* Refresh patches
* Push the changes

## Building Locally

To build on a test environment before submitting a change to production the following procedure can be used.

```sh
debian/rules get-orig-source
debuild -us -uc
```
The `.deb` will be located in the parent directory.
