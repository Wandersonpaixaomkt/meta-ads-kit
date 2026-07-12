# Conectar o MCP oficial da Meta Ads ao Codex

Este repositório já contém a configuração do servidor remoto oficial da Meta em `.codex/config.toml`.

## 1. Abra o repositório no Codex

Abra a pasta `meta-ads-kit` no Codex Desktop, na extensão do Codex ou no Codex CLI e marque o projeto como confiável quando solicitado.

## 2. Autentique sua conta Meta

No terminal aberto dentro do projeto, execute:

```bash
codex mcp login meta_ads
```

O navegador abrirá a autorização da Meta. Entre com o perfil que possui acesso às contas de anúncios e aprove apenas os ativos que deseja administrar.

## 3. Confirme a conexão

```bash
codex mcp list
```

Dentro do Codex, também é possível usar:

```text
/mcp
```

O servidor `meta_ads` deve aparecer como conectado.

## Segurança configurada

A configuração usa OAuth; nenhum token, senha ou segredo fica salvo neste repositório. Consultas e análises podem ser executadas normalmente. Ações que alteram campanhas, anúncios, conjuntos, status ou orçamento devem solicitar aprovação antes da execução.

## Exemplos de uso

```text
Liste as contas de anúncios às quais tenho acesso, sem fazer alterações.
```

```text
Analise o desempenho dos últimos 7 dias e identifique campanhas com CPA acima da meta. Não altere nada.
```

```text
Prepare uma proposta para pausar os anúncios com pior desempenho, mas peça minha aprovação antes de executar qualquer mudança.
```
