# APK publishing contract

The stable download filename is `sifriat-harayah.apk`.

Every future release must upload the newest signed APK with that exact asset name and be marked as the latest non-prerelease. Keep the already-published compatibility asset `sifriat-harayah-0.4.96.apk` on release `v0.4.96`, updating its bytes to the newest APK too while old links remain in circulation. Never leave that URL serving a known-broken build.

After publishing, download both the latest-release stable URL and the legacy compatibility URL. Compare their complete SHA-256 digests with the signed local APK. Confirm Android versionCode/versionName in the downloaded file. Do not report either link ready from upload success alone.

The current workflow uploads both asset names. If creating a new release tag, update the workflow's target tag while retaining an extra upload to the legacy release for compatibility. Do not remove the stable asset name.
