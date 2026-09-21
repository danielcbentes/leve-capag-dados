# leve-capag-dados

Artefato de dados assinado (contrato v2 rev. 4) consumido pelo app **Leve CAPAG**.

Publicado automaticamente por um workflow do repositório de código (privado, `Leve_CAPAG`), a partir de:
- Tesouro Nacional (STN) — classificação CAPAG oficial
- TCE-CE — API de Dados Abertos do SIM (`https://api-dados-abertos.tce.ce.gov.br/sim/`)

Nada aqui é sigiloso: são dados já públicos nas fontes originais, apenas recombinados, verificados e assinados (Ed25519) para o app baixar com segurança.

Estrutura:
- `versao-atual.txt` — ponteiro da versão mais recente (AAAA.MM.DD)
- `manifesto-<versao>.json`, `dataset-<versao>.json`, `parametros-<versao>.json`, `corpus-<versao>.json`, `indice-detalhes-<versao>.json` — arquivos BASE
- `<versao>/detalhes/detalhe-<ibge>-<versao>.json` — DETALHE por município, sob demanda
