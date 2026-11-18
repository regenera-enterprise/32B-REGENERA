# Regenera 32B — Weight Distribution

> **Official weight manifest and distribution record for Regenera 32B**

This directory documents the official weight distribution of **Regenera 32B**, a language model with **32,118,447,104 declared parameters**.

The model weights are distributed as **7 SafeTensors shards** with a combined local size of:

**36,265,925,343 bytes (~36.27 GB decimal)**

The weight files are not stored directly in this GitHub repository because each shard exceeds the GitHub LFS per-object limit observed during publication.

The GitHub repository remains the **canonical technical and evidentiary repository** for configuration, manifests, hashes, signatures, provenance records and release metadata.

---

## Weight set

| Shard | SHA-256 |
|---|---|
| `model-00001-of-00007.safetensors` | `cf7d6d85f39129dac205d8a8610ce18f9c4bb325effbe071bf61fbe51a26a130` |
| `model-00002-of-00007.safetensors` | `f23c7b5aa5013feffecec0888bc8d5e7eb28ccd0b8384d84b52a2b695aefd737` |
| `model-00003-of-00007.safetensors` | `5a4a40ffc4e79239032b71433ace0de995481e5e0166a940179d6220b60f044b` |
| `model-00004-of-00007.safetensors` | `0c176364d2f32375592c2ac870d7889fc1ff61a66b5a54f7b9776192a2043bf0` |
| `model-00005-of-00007.safetensors` | `bcb76e3c1dc3c34c005aa51a5d28e3ea47c8534c52937fc6bd6a4911b430635b` |
| `model-00006-of-00007.safetensors` | `8329885b9d2381ceb79e6e33ad2660501f277e30e761425ab254b0dd11564b84` |
| `model-00007-of-00007.safetensors` | `b8415f31cbb3eeeb4843059920de794acd142a463b49533e3e2dae0d4b52c1d6` |

These identifiers were produced from the actual local weight files and were also observed by Git LFS during the attempted publication.

---

## Integrity

The local evidence package generated for this release includes:

- `evidencias/PESOS-REGENERA-32B-SHA256.txt`
- `evidencias/PESOS-REGENERA-32B-MANIFEST.json`
- `evidencias/MANIFEST-SHA256.txt`
- `evidencias/MANIFEST-SHA256.json`
- `evidencias/HASHES-CRITICOS.sha256`
- `evidencias/EVIDENCIAS-PRINCIPAIS.sha256`

The critical model files were checked with SHA-256 and reported **OK** during local verification.

---

## Cryptographic signature

The evidence manifest was signed with a dedicated **Ed25519 SSH signing key**.

**Signing key fingerprint**

```text
SHA256:OM4mUvOWjZILowERckms0ezssaFSujfN0SpbaeXIwhU
```

The local verification result was:

```text
Good "file" signature for regenera32b with ED25519 key SHA256:OM4mUvOWjZILowERckms0ezssaFSujfN0SpbaeXIwhU
```

Associated evidence files:

- `evidencias/github/regenera-32b-signing-public-key.pub`
- `evidencias/assinaturas/MANIFEST-SHA256.txt.sig`
- `evidencias/assinaturas/VERIFICACAO.txt`
- `evidencias/assinaturas/allowed_signers`

Only the **public key** belongs in the repository. The private signing key must remain outside version control.

---

## Canonical model metadata

The following files define the model package and should remain versioned in the canonical GitHub repository:

```text
config.json
generation_config.json
tokenizer_config.json
tokenizer.json
chat_template.jinja
model.safetensors.index.json
```

The index file `model.safetensors.index.json` maps tensors to the seven SafeTensors shards.

---

## Weight hosting

The weight binaries require external model storage because their individual sizes exceed the GitHub LFS object limit encountered during upload.

**Current distribution status**

- GitHub canonical repository: **active**
- Weight hashes: **generated**
- Weight manifest: **generated**
- Ed25519 signature: **verified locally**
- External binary hosting endpoint: **pending publication**

Once the official external weight repository is published, its canonical URL must be added here and tied to the same SHA-256 values listed above.

A valid external copy is considered identical to the canonical Regenera 32B weight set only when all seven files reproduce the SHA-256 values in this document.

---

## Verification

After downloading all seven shards, verify them on macOS or Linux with:

```bash
shasum -a 256 model-*.safetensors
```

The resulting hashes must match the table above exactly.

For a manifest-based check:

```bash
shasum -a 256 -c evidencias/PESOS-REGENERA-32B-SHA256.txt
```

For the signed evidence manifest:

```bash
ssh-keygen \
  -Y verify \
  -f evidencias/assinaturas/allowed_signers \
  -I regenera32b \
  -n file \
  -s evidencias/assinaturas/MANIFEST-SHA256.txt.sig \
  < evidencias/MANIFEST-SHA256.txt
```

Expected result:

```text
Good "file" signature for regenera32b with ED25519 key SHA256:OM4mUvOWjZILowERckms0ezssaFSujfN0SpbaeXIwhU
```

---

## Provenance boundary

This document establishes the identity and integrity relationship between the documented Regenera 32B release and the seven weight files through cryptographic hashes and a signed manifest.

It does **not**, by itself, constitute an independent audit of training provenance, dataset origin or authorship. Those claims require their corresponding primary technical records, training artifacts, logs and provenance evidence.

---

## Project identity

**Model:** Regenera 32B  
**Author & Developer:** Paulo Ricardo de Leão  
**CEO & Co-Founder:** Raphaela Cerveski  
**Organization:** Regenera Corporate  
**Canonical repository:** https://github.com/regenera-enterprise/32B-REGENERA

**WE FUTURE. WE REGENERA.**
