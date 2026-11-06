# ORIZURU SEKISHO — signed release feed

This repository hosts **signed release artifacts and update metadata** for the
ORIZURU SEKISHO management server.

- Source code is kept in a separate private repository.
- Artifacts are signed with the ORIZURU WORKS Ed25519 release key.
- The signed feed is the source of truth. Do not use GitHub's `latest` release
  as an update source; use the feed below.

## Feed

- stable: `https://orizuru-works.github.io/sekisho-releases/feed/stable.json`
- security: `https://orizuru-works.github.io/sekisho-releases/feed/security.json`

Each feed is accompanied by a detached signature (`<name>.json.sig`).

## Verification key

Ed25519 public key (base64):

```
/3Km8mH1R31jeb5WWV+KAEm8j/KjLgJEApzRzmNzyws=
```

SHA-256 fingerprint of the raw public key:

```
9b89a4d07d86661df5257fe1861d04226ecd849d2532dfe358b86bce10355121
```

The update client refuses unsigned metadata and artifacts. A mirror may host
the same files; the signature, not the hostname, is the trust anchor.

## Security

Please report vulnerabilities through the security policy of the ORIZURU
WORKS repository. Do not open a public issue for an unpatched vulnerability.
