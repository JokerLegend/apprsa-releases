# AppRSA — engine payloads

This repository holds the encrypted engine payloads for AppRSA.

Every file published here is **AES-256-GCM encrypted**. The decryption key is
issued by the licence server only after a valid activation, so these files
contain no readable code and are of no use on their own.

The application source is **not** in this repository.

Each release also carries an Ed25519 signature over the payload's SHA-256, which
the app verifies before installing — so a file published here cannot be swapped
for another without the app rejecting it.
