# Histórico de Mudanças (Changelog) — ROG Launcher

Todas as mudanças relevantes e lançamentos públicos do ROG Launcher são registrados neste documento.

O formato segue as diretrizes do [Keep a Changelog](https://keepachangelog.com/pt-BR/1.0.0/) e respeita o Versionamento Semântico.

---

## [v4.9-beta] — 2026-10-24

### ✨ Adicionado
* **Sistema de Atualização Automática**:
  * Consulta atômica ao endpoint público do GitHub Releases (`castellorogerio/rog-launcher-releases`).
  * Card dedicado em **Configurações > Geral** com barra de progresso percentual em tempo real.
  * Script de substituição segura `tools/apply_update.bat` com criação de backup `.bak`, rollback em falha e reinício automático.
* **Biblioteca em Modo Console**:
  * Novo alternador `☵ Grade` e `▬ Console` no cabeçalho da biblioteca pessoal.
  * Hero superior moderno exibindo arte panorâmica do jogo, tempo de jogo, gênero e botões de ação (`▶ Jogar`, `ℹ Detalhes`, `··· Gerenciar`).
  * Carrossel inferior contínuo de pôsteres verticais com foco suave por controle e teclado.
  * Preferência de modo persistida individualmente por perfil.
* **Recortador Visual de Avatar (Cropper)**:
  * Ferramenta interativa para enquadramento de fotos de perfil em proporção circular perfeita.
  * Controles de arrastar, zoom suave e botão de centralização automática.
* **Novo Efeito Sonoro de Conclusão**:
  * Efeito sonoro harmônico de download concluído (`audio/download_complete.wav`), reproduzido mesmo com o launcher minimizado.

### 🔧 Modificado
* **Catálogo Unificado**:
  * Substituído endpoint legado pela API oficial Steam Search com suporte a paginação contínua e filtragem de fontes ativas (`_match_sources_summary_for_game`).
  * 100% dos títulos do catálogo agora possuem arte de capa oficial (`header.jpg` e `capsule`), eliminando cards cinzas.
  * Removidos botões desnecessários "A-Z" e "Z-A" do cabeçalho da página.
  * Resolução fixa de texturas com `sourceSize: Qt.size(460, 215)` para evitar redimensionamento tardio de imagens.
* **Motor aria2c**:
  * Removida a opção `--max-overall-upload-limit=1K` que causava estrangulamento (*choking*) no protocolo BitTorrent.
  * Injetados trackers públicos rápidos, nós DHT e limite ampliado para 120 conexões simultâneas.
  * Mensagens claras de estimativa de tempo (ETA) informando "Buscando pares e metadados..." em vez de travar em "Calculando...".
* **Toast Global de Conclusão**:
  * z-index elevado para `100000`, garantindo sobreposição mesmo sobre caixas de diálogo modais.
  * Adicionado botão de fechar ("✕") e clique para abrir a aba Downloads diretamente.
* **Gerenciamento de Perfis**:
  * Removida a área de clique invasiva de tela inteira do card de perfil. A seleção agora é acionada estritamente pelo avatar ou pelo botão **Selecionar**.
  * Correção da indicação de perfil ativo: ao deslogar da sessão, nenhum perfil permanece marcado como "Selecionado".

### 🔒 Segurança e Integridade
* Integridade de `rog.py` verificada e preservada (`SHA-256: 521F2B3E643D649730C356145C79438C6735C4C3DF8693B5EFFDBA036D851800`).
* Isolamento estrito entre repositório de código-fonte privado e repositório público de distribuição.

---

## [v4.8-beta] — 2026-10-23

### ✨ Adicionado
* Suporte nativo a reprodução de vídeo em tela cheia na visualização de detalhes.
* Módulo de compatibilidade e instalação silenciosa de pacotes DirectX e Visual C++ Redistributables.

### 🔧 Modificado
* Ajustes de estabilidade para navegação com controle de Xbox e PlayStation.
* Otimização na rotação de logs e supressão de mensagens de layout em loops do QML.

---

## [v4.7-beta] — 2026-10-22

### ✨ Adicionado
* Fila de downloads assíncrona com suporte a pausa e cancelamento.
* Leitura de fontes de repackers e provedores de download em JSON.
* Tela de gerenciamento de múltiplos perfis locais.
