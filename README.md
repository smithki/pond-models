# Pond's models

The files [Pond](https://pond.camera) downloads for searching its recordings by picture: Google's
[SigLIP 2](https://huggingface.co/google/siglip2-base-patch16-224), converted to Core ML. This repository holds no code,
only these files, as its releases: each version one release (`siglip2-v1`, …), one archive and its licence, never
changed once published.

Pond doesn't take a file from here on trust: it downloads the version pond.camera's manifest names, which is signed
with Pond's own key, and refuses any file whose SHA-256 isn't the one signed for. A new version is made by Pond's CI
(the converter is in Pond's repository), checked, and published here only when its maintainer approves it.

## Licence

SigLIP 2 is Google's, under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0); the archives are
converted to Core ML and quantized from it, and carry the licence and a notice saying so.

Questions and bug reports go to Pond's own repository, not here.
