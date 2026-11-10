# Pond's models

The model files [Pond](https://pond.camera) uses, published here so its builds and its copies download exactly
these, by hash. This repository holds no code, only these files, as its releases: each version one release, never
changed once published.

| Model | Releases | What Pond does with it | Licence |
| --- | --- | --- | --- |
| Google's [SigLIP 2](https://huggingface.co/google/siglip2-base-patch16-224), converted to Core ML | `siglip2-v1`, … | Search by picture | Apache 2.0 |
| Ultralytics [YOLO26](https://docs.ultralytics.com) small, exported to Core ML | `yolo26s-v1`, … | Detection, built into the app | AGPL 3.0 |

Each archive carries its model's licence and a notice saying how it was made, from what. A YOLO26 release carries
its source too (Ultralytics' weights, `yolo26s.pt`), as the AGPL asks.

Pond doesn't take a file from here on trust. Its builds check each archive against the SHA-256 Pond's repository
records for it, and Pond downloads a search model only when pond.camera's manifest names it, signed with Pond's
own key, and only a file whose SHA-256 is the one signed for. New search model versions are made by Pond's CI,
checked, and published here only when its maintainer approves them.

Questions and bug reports go to Pond's own repository, not here.
