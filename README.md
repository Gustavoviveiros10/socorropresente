# Socorro, Presente! · Vitrine

Site estático (um `index.html`) da vitrine do link da bio do @socorropresente_.

## Onde mexer
- **Configuração** (topo do `index.html`, em `SP_CONFIG`): link do grupo do WhatsApp, redes, ID do GTM, data em destaque e URL da planilha.
- **Produtos**: vêm da planilha do Google "Socorro Presente - Produtos da vitrine" (precisa estar compartilhada como "Qualquer pessoa com o link: leitor"). Se a planilha não carregar, o site usa a lista `SP_PRODUTOS` do próprio arquivo.
  - `status` = `ativo` ou `exemplo` aparece; `esgotado` ou `pausado` some.
- **Links filtrados** (para DM e bio): `?p=sogra`, `?preco=30`, `?data=blackfriday`, combináveis.

## Eventos no dataLayer (GTM)
`clique_oferta` (categoria, produto_id, produto_nome, plataforma, preco_aprox, sub_id), `filtro_vitrine`, `busca_vitrine`, `ordem_vitrine`, `clique_whatsapp`, `clique_rede`, `vitrine_carregada`.

## Publicação
Sem build: qualquer host estático serve (Vercel: importar o repositório, framework "Other").
