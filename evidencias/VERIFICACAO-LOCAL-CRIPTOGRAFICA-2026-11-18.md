# Verificação local criptográfica — Regenera 32B

Data registrada pela execução local: **2026-11-18T15:43:36Z**

Este registro consolida resultados observados diretamente na execução local realizada em:

`/Users/enterprise/Desktop/32B-REGENERA`

Ele registra integridade de arquivos, hashes dos sete shards, assinatura SSH/Ed25519 e o estado Git observado no instante da geração.

## Resultado geral

- Arquivos incluídos no manifesto local: **19**
- Bytes totais incluídos no manifesto: **36,273,228,830**
- Arquivos SafeTensors: **7**
- Bytes totais SafeTensors: **36,265,925,343**
- SHA-256 dos arquivos críticos: **PASS**
- Assinatura do manifesto: **Ed25519 / SSH**
- Verificação da assinatura: **PASS**

Resultado observado:

```text
Good "file" signature for regenera32b with ED25519 key SHA256:OM4mUvOWjZILowERckms0ezssaFSujfN0SpbaeXIwhU
```

## Chave de assinatura

Fingerprint:

```text
SHA256:OM4mUvOWjZILowERckms0ezssaFSujfN0SpbaeXIwhU
```

Identificação registrada:

```text
Regenera 32B signing key
```

Algoritmo:

```text
ED25519
```

## Shards verificados

| Arquivo | Tamanho em bytes | SHA-256 |
|---|---:|---|
| `model-00001-of-00007.safetensors` | 5,355,749,848 | `cf7d6d85f39129dac205d8a8610ce18f9c4bb325effbe071bf61fbe51a26a130` |
| `model-00002-of-00007.safetensors` | 5,326,794,296 | `f23c7b5aa5013feffecec0888bc8d5e7eb28ccd0b8384d84b52a2b695aefd737` |
| `model-00003-of-00007.safetensors` | 5,326,794,343 | `5a4a40ffc4e79239032b71433ace0de995481e5e0166a940179d6220b60f044b` |
| `model-00004-of-00007.safetensors` | 5,255,948,093 | `0c176364d2f32375592c2ac870d7889fc1ff61a66b5a54f7b9776192a2043bf0` |
| `model-00005-of-00007.safetensors` | 5,326,794,396 | `bcb76e3c1dc3c34c005aa51a5d28e3ea47c8534c52937fc6bd6a4911b430635b` |
| `model-00006-of-00007.safetensors` | 5,326,794,305 | `8329885b9d2381ceb79e6e33ad2660501f277e30e761425ab254b0dd11564b84` |
| `model-00007-of-00007.safetensors` | 4,347,050,062 | `b8415f31cbb3eeeb4843059920de794acd142a463b49533e3e2dae0d4b52c1d6` |

## Arquivos críticos verificados

A execução local reportou `OK` para:

```text
README.md
config.json
generation_config.json
tokenizer.json
tokenizer_config.json
chat_template.jinja
model.safetensors.index.json
model-00001-of-00007.safetensors
model-00002-of-00007.safetensors
model-00003-of-00007.safetensors
model-00004-of-00007.safetensors
model-00005-of-00007.safetensors
model-00006-of-00007.safetensors
model-00007-of-00007.safetensors
```

## Estado Git registrado no momento da geração

```text
repository=https://github.com/regenera-enterprise/32B-REGENERA.git
branch=main
origin_main=298864e9f02586519c173db7e7c07d6cdecc4c0e
local_head=298864e9f02586519c173db7e7c07d6cdecc4c0e
readme_git_blob=605857a547f8f4fc9646fd439f4825d4985fcf59
banner_git_blob=e78427fe91bfdb7f337ea8d51cbaff5ab15ca742
generated_utc=2026-11-18T15:43:36Z
```

Esse estado Git é histórico: representa o instante da geração das evidências locais e não o HEAD remoto atual.

## Pacote local de evidências

A execução local gerou os seguintes arquivos:

```text
evidencias/assinaturas/allowed_signers
evidencias/assinaturas/MANIFEST-SHA256.txt.sig
evidencias/assinaturas/VERIFICACAO.txt
evidencias/ESTADO-GITHUB-2026-11-18.md
evidencias/EVIDENCIAS-PRINCIPAIS.sha256
evidencias/EVIDENCIAS-REAIS.md
evidencias/GIT-HISTORY.txt
evidencias/GIT-REMOTES.txt
evidencias/GIT-STATE.txt
evidencias/GIT-STATUS.txt
evidencias/github/github-public-authentication-keys.json
evidencias/github/github-public-signing-keys.json
evidencias/github/regenera-32b-signing-key-fingerprint.txt
evidencias/github/regenera-32b-signing-public-key.pub
evidencias/HASHES-CRITICOS.sha256
evidencias/MANIFEST-SHA256.json
evidencias/MANIFEST-SHA256.txt
evidencias/PESOS-REGENERA-32B-MANIFEST.json
evidencias/PESOS-REGENERA-32B-SHA256.txt
evidencias/RESUMO-PESOS.json
```

## Limite probatório

Este registro documenta resultados técnicos observados na execução local: integridade SHA-256, identidade dos sete arquivos SafeTensors, fingerprint da chave pública usada, verificação positiva da assinatura Ed25519 e estado Git registrado.

Ele não converte, por si só, declarações sobre treinamento, origem de dataset ou autoria em auditoria independente. Essas afirmações exigem seus respectivos artefatos primários de treinamento e proveniência.
