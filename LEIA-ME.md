# Alerta SST — Projeto educacional

Aplicativo web instalável (PWA) para comunicação e acompanhamento de situações de risco no trabalho.

## Como testar
1. Extraia o ZIP.
2. Abra `index.html` em um navegador atualizado.
3. Entre em **Comunicar risco** e cadastre uma ocorrência.
4. Veja o painel, abra a ocorrência, atualize o status e exporte relatórios.

## Como instalar no Android
Para habilitar instalação PWA e cache offline, publique a pasta em um servidor HTTPS, como GitHub Pages:
1. Crie um repositório no GitHub.
2. Envie os arquivos da pasta `alerta-sst` para a raiz do repositório (ou configure a publicação da subpasta).
3. Em **Settings > Pages**, selecione a publicação pela branch principal e pasta raiz.
4. Acesse o endereço HTTPS gerado no Chrome do celular.
5. No menu do navegador, escolha **Instalar app** ou **Adicionar à tela inicial** (a opção depende do navegador).

Também é possível testar localmente com `python -m http.server 8000` e acessar `http://localhost:8000` no computador.

## Funcionalidades
- Painel com indicadores e gráficos por categoria e gravidade
- Registro de condições inseguras e quase acidentes
- Fotografia opcional até 2 MB
- Registro sem nome ou com nome
- Busca e filtros
- Status aberta / em andamento / resolvida
- Responsável, prazo e histórico de providências (campo de observações)
- Exportação CSV e backup JSON; importação de backup
- Impressão e salvar PDF pelo navegador
- PWA com cache offline dos arquivos do aplicativo

## Limitações importantes
- Dados salvos apenas no navegador local, sem servidor ou sincronização.
- O modo anônimo significa apenas que o nome não é registrado; não é um canal institucional de denúncias.
- Não há notificações reais nem envio automático para responsáveis.
- Não substitui procedimentos oficiais de emergência ou avaliação profissional de riscos.
- Fotos grandes podem exceder a capacidade de armazenamento local; faça backups.
- A impressão em PDF depende do recurso de impressão do navegador.

## Sugestão de demonstração
Cadastre uma tomada com fiação exposta em um laboratório fictício, gravidade alta. Mostre o gráfico e a lista. Atualize para "Em andamento", informe uma providência, depois "Resolvida". Exporte o relatório.
