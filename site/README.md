# OfereceAí — protótipo experimental (versão 3.0)

Esta pasta contém o **MVP navegável** de um conceito de marketplace inverso. O projeto foi desenvolvido com auxílio de IA para **experimentar fluxos de interface e documentar seu processo de construção**, não para oferecer um serviço comercial real.

Para conhecer a história do desenvolvimento, consulte o [DEVLOG](../DEVLOG.md) e o [README principal](../README.md).

## Como abrir

1. Abra `index.html` diretamente em um navegador moderno.
2. Ou, dentro desta pasta, execute `python -m http.server 8000` e abra `http://localhost:8000`.
3. Use os perfis **Comprador demo**, **Lojista demo** e **Admin demo** para percorrer o protótipo.

Não há instalação npm, API, credenciais, `.env`, banco remoto ou backend.

## Fluxos para experimentar

- Navegar pela homepage, categorias e pedidos fictícios.
- Pesquisar e filtrar pedidos.
- Publicar uma solicitação com quantidade, localização, características e orçamento opcional.
- Trocar para o perfil de lojista e enviar ou editar uma proposta com preço, frete e prazo.
- Voltar ao comprador para visualizar propostas, conversar e selecionar uma opção.
- Explorar o painel administrativo de demonstração.
- Acessar a página `#/para-vendedores`, que apresenta o conceito sem planos de preços nem créditos.

Os perfis de demonstração não exigem senha verdadeira. Trocar de perfil funciona apenas dentro deste navegador.

## Estrutura

```text
site/
├── index.html        # Estrutura HTML e metadados
├── styles.css        # Identidade visual e responsividade
├── app.js            # Telas, navegação e lógica demonstrativa
├── assets/favicon.svg
├── README.md         # Este guia
└── TESTES.md         # Registro das verificações relatadas na entrega
```

## Persistência e limites

O protótipo usa **HTML, CSS, JavaScript nativo e `localStorage`**, com as chaves `ofereceai_mvp_v1` e `ofereceai_session_v1`. Dados criados em um computador não aparecem automaticamente em outro. Pedidos, lojas e ofertas iniciais são fictícios; mensagens não são enviadas pela internet.

- Sem autenticação ou autorização real de usuários.
- Sem banco compartilhado, integração financeira, checkout ou notificações externas.
- Sem verificação de CNPJ, estoque ou reputação de vendedores reais.
- Sem deploy público informado.

**Não use informações sensíveis, senhas ou dados financeiros reais neste protótipo.**

## Decisões de produto representadas

- Modelo invertido: **comprador publica uma necessidade e lojistas oferecem propostas**.
- Propostas privadas no fluxo demonstrativo.
- Categorias com rótulos visíveis: Móveis, Celulares, Informática, Casa e Construção.
- Página pública de orientação para vendedores.
- **Sem venda de créditos, valores de planos ou cobrança implementada.** O Modelo B foi apenas uma direção conceitual escolhida durante a conversa.

## Testes e continuidade

O arquivo [`TESTES.md`](./TESTES.md) resume os testes locais **relatados na entrega**. Não há suíte automatizada versionada. Se este experimento for retomado, podem ser discutidas novas funcionalidades e outras arquiteturas, mas **não há lançamento comercial previsto neste escopo**.

**Autor e direção do projeto:** David Alexander · **Desenvolvimento assistido por IA**.
