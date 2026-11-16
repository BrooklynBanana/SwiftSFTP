# Fork notice

This is a fork of [RuiNelson/SwiftSFTP](https://github.com/RuiNelson/SwiftSFTP) (Apache-2.0) for the Swift Connection Manager.

Branch `connection-manager`, based on upstream `v3.22.0`. Changes:

- `Package.swift` (2026-11-16): the libssh2 target is built with the `LIBSSH2_*_ENABLE` defines, so the methods
  libssh2 disables by default since 1.11.2_DEV (SHA-1 key exchange, `ssh-rsa`/`ssh-dss` host keys, `hmac-sha1`,
  MD5, 3DES, RIPEMD-160, Blowfish, RC4, CAST) stay available for very old servers.

Nothing else differs from upstream.
