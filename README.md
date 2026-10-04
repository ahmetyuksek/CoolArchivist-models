# CoolArchivist models

Model files for [CoolArchivist](https://ahmetyuksek.com), downloaded by the app's first-run
setup. Each release holds one model with its `LICENSE.txt`. The app pins every file's
SHA-256 and size, so it only installs exactly these bytes.

| Release | Model | Used for | License |
|---|---|---|---|
| `siglip2-so400m-patch14-384-r1` | [SigLIP 2 so400m, 384 px](https://huggingface.co/google/siglip2-so400m-patch14-384) by Google | Search by content (graphics card) | Apache 2.0 |
| `siglip2-base-patch16-224-r1` | [SigLIP 2 base, 224 px](https://huggingface.co/google/siglip2-base-patch16-224) by Google | Search by content (processor) | Apache 2.0 |
| `Florence-2-large-r1` | [Florence-2 large](https://huggingface.co/florence-community/Florence-2-large) by Microsoft | Captions | MIT |
| `faces-r1` | [YuNet 2023mar](https://github.com/opencv/opencv_zoo/tree/main/models/face_detection_yunet) and [SFace 2021dec](https://github.com/opencv/opencv_zoo/tree/main/models/face_recognition_sface), OpenCV Model Zoo | Faces and people | MIT, Apache 2.0 |

Changes: SigLIP 2 and Florence-2 are converted to ONNX (SigLIP 2 in float16), with tag
vectors computed from SigLIP 2 for CoolArchivist's vocabulary. The face models are unchanged.
The license texts are in `licenses/` and in each release.
