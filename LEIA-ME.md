# wordcraft-web-teste

Hospedagem temporária (GitHub Pages) para a seção 6 do roteiro de medição da avaliação do port
do WordCraft para Android (`geocida/wordcraft`, branch `android-eval`).

| Arquivo | Origem |
|---|---|
| `index.html`, `*.js`, `*.wasm`, `snippets/`, licenças | `wordcraft-web-0.15.0.zip` do release v0.15.0 de `storytold/wordcraft`, sem alterações; SHA-256 `c5a02d4e4f1d3e59288da4647d2d734296fd31e39ccd060a83ac2d2faa12a79a`, igual ao `SHA256SUMS.txt` do release |
| `sonda.html` | `web/sonda.html` de `geocida/wordcraft-android-probe`, commit `0f47f1e` |
| `.nojekyll` | desliga o Jekyll do GitHub Pages, para servir os arquivos como estão |

O `README.md` desta pasta é o do WordCraft, que vem no zip.

## Endereços (depois de ligar o Pages)

1. WordCraft com o documento de exemplo: https://geocida.github.io/wordcraft-web-teste/?sample
2. Forçar WebGL2: https://geocida.github.io/wordcraft-web-teste/?sample&webgl
3. Sonda do Chrome: https://geocida.github.io/wordcraft-web-teste/sonda.html

## Observações

1. O `.wasm` tem 54.273.204 bytes. Se o GitHub Pages não comprimir esse tipo de arquivo, o
   tablet baixa os 54 MB na primeira abertura (não verificado).
2. O GitHub Pages ignora o `_headers` do pacote. Pelo `HOSTING.md` do WordCraft, o app não
   precisa de COOP nem COEP; exige HTTPS e `.wasm` como `application/wasm`.
3. O repositório é público: qualquer pessoa com o endereço abre as páginas.
