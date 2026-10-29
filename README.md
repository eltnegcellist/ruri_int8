# Ruri v3 70M — Mitsukotoba INT8 ONNX

This repository distributes the Mitsukotoba-specific INT8 ONNX conversion of [cl-nagoya/ruri-v3-70m](https://huggingface.co/cl-nagoya/ruri-v3-70m).

- Base revision: `07a8b0aba47d29d2ca21f89b915c1efe2c23d1cc`
- Model: `model.onnx` (71,248,404 bytes)
- SHA-256: `bd500193003fdeaba8c5422a47b974b40b49a5e0c91285c76f6bd949d2205264`
- License: Apache-2.0; see accompanying license, attribution and model card documents.
- This is **not an official cl-nagoya quantization**. The ONNX graph and embedding table were customized for Mitsukotoba.

The derived classification heads (Topic/Interaction/Intent/State) and tokenizer files are provided separately from the model weights and are required by Mitsukotoba's classifier. Verify hashes before use. The published release files are checked by the GitHub Actions import workflow. Model binaries are distributed by GitHub's raw file endpoint.

For model usage, please refer to the [Mitsukotoba Web app](https://github.com/eltnegcellist/Web_EmmaLocal_English_for_babies).

## Browser download

The application fetches the SHA-256-pinned model from an immutable Git commit:

https://raw.githubusercontent.com/eltnegcellist/ruri_int8/181a9f2a8b3706d430116ed8ae992866cb603b26/model.onnx

The [browser delivery check](https://github.com/eltnegcellist/ruri_int8/actions/runs/40809777833) verified HTTP 200, `Access-Control-Allow-Origin: *`, exactly 71,248,404 bytes and the SHA-256 above. The model URL is public; any user can obtain the exact weights without GitHub authentication. GitHub Pages/R2 is not required for this distribution.
