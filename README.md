# Omnes BarHub — Downloads

Canal público de distribuição dos instaladores Windows x64 do Omnes BarHub.

`update.json` é o catálogo consultado pelo aplicativo. `release: null` significa que ainda não há instalador publicado. Atualizar o código-fonte não publica um instalador automaticamente.

Para publicar: gere e homologue o instalador EXE/MSI, mantenha UpgradeCode/identidade de atualização no Advanced Installer e preserve a pasta de dados em LocalAppData. Use `scripts/prepare-update.cjs` do projeto BarHub para calcular SHA256 e tamanho do arquivo final. Envie o instalador para uma release estável com tag `vX.Y.Z`, confira o download e somente então substitua `update.json` pelo manifesto gerado. O nome do asset deve coincidir exatamente com a URL do manifesto.

Nenhum instalador foi publicado na configuração inicial deste catálogo. Não use arquivos de código-fonte, hashes fictícios ou URLs que ainda não existem como atualização.
