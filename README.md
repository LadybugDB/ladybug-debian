# LadybugDB Debian Packaging

Packaging follows Debian source format 3.0 (quilt).

To build from upstream source:
  1. Download the Ladybug release tarball.
  2. Rename it to ladybug_<version>.orig.tar.gz.
  3. Extract the tarball to a new directory. Don't delete the tarball after extraction, we need it for the build process
  4. Copy the `debian/` directory from this repository into the extracted directory and `cd` into it.
  5. Run `export DH_BUILD_SYSTEM=cmake_ninja && dpkg-buildpackage -us -uc`

## References
- https://arnaudr.io/2016/01/14/first-debian-package/
- https://arnaudr.io/2016/10/01/publishing-a-debian-package-mentors-sponsorship/
