# ROG Launcher — Distribuição Oficial (Beta)

<p align="center">
  <img src="https://raw.githubusercontent.com/castellorogerio/rog-launcher-releases/main/assets/rog_launcher_banner.png" alt="ROG Launcher Banner" width="700" onerror="this.style.display='none'"/>
</p>

<p align="center">
  <strong>O launcher de jogos moderno, fluido e unificado para Windows com suporte nativo a controle e gerenciador de downloads integrado.</strong>
</p>

<p align="center">
  <a href="https://github.com/castellorogerio/rog-launcher-releases/releases"><img src="https://img.shields.io/github/v/release/castellorogerio/rog-launcher-releases?include_prereleases&label=Vers%C3%A3o%20Beta&color=red" alt="Versão Beta"/></a>
  <a href="https://github.com/castellorogerio/rog-launcher-releases/releases"><img src="https://img.shields.io/github/downloads/castellorogerio/rog-launcher-releases/total?label=Downloads&color=blue" alt="Total Downloads"/></a>
  <img src="https://img.shields.io/badge/Plataforma-Windows%2010%20%7C%2011%20(64--bit)-0078D6" alt="Windows 10/11 64-bit"/>
  <img src="https://img.shields.io/badge/Licen%C3%A7a-MIT-green" alt="Licença MIT"/>
</p>

---

## 🎮 1. Apresentação do ROG Launcher

O **ROG Launcher** é uma interface desktop moderna, construída sobre **Python, PySide6 e Qt Quick (QML)**, desenvolvida para unificar toda a sua experiência com jogos de PC em um só lugar. Seja utilizando controle (estilo console portátil ou TV) ou mouse e teclado, o ROG Launcher entrega navegação responsiva, animações fluidas a 60 FPS, gerenciamento de múltiplos perfis e integração com fontes e downloaders de alta velocidade.

> [!NOTE]
> **Aviso de Versão Beta**: O aplicativo encontra-se atualmente em fase **Beta aberta**. Recursos centrais estão totalmente operacionais, mas novas melhorias de desempenho e integrações continuam sendo implementadas ativamente.

---

## ✨ 2. Funcionalidades Efetivamente Disponíveis

* **🏠 Home Dinâmica**:
  * Carrossel de títulos em destaque com capas em alta definição e banners panorâmicos.
  * Lista de jogos populares com estatísticas da comunidade **HowLongToBeat** (tempo de campanha, extras e 100%).
  * Estatísticas gerais do jogador e atalhos de inicialização rápida.
* **🔍 Catálogo Unificado**:
  * Busca em tempo real integrada à Steam Search API com correspondência precisa de títulos.
  * Filtragem por gênero (Ação, RPG, Aventura, Indie, etc.) e filtro exclusivo **"Com fontes ativas"**.
  * Visualização de opções de download com múltiplos provedores e links de repackers.
* **📚 Biblioteca Pessoal Flexível**:
  * **Modo Grade (Grid)**: Visão panorâmica dos jogos instalados e adicionados com bordas dinâmicas de foco e botões de ação rápida.
  * **Modo Console**: Layout no estilo TV/Handheld com Hero superior em destaque e carrossel inferior com rolagem horizontal contínua.
  * Suporte a jogos nativos de PC, jogos Steam e emuladores (PCSX2, RPCS3, DuckStation, PPSSPP).
* **⚡ Central de Downloads Integrada (Estilo Hydra)**:
  * Motor de transferência assíncrono baseado no **aria2c** com suporte a downloads diretos e BitTorrent com DHT e trackers públicos.
  * Telemetria em tempo real: velocidade em MB/s, tempo estimado (ETA), progresso percentual e tamanho total.
  * Notificação global (*toast*) sonora e visual na conclusão de cada download, persistindo sobre qualquer tela.
* **👤 Perfis Personalizados e Independentes**:
  * Múltiplos perfis de usuário com senha de segurança opcional.
  * Ferramenta visual de corte de avatar (*Avatar Cropper*) com zoom e centralização em proporção circular.
  * Armazenamento isolado de favoritos, tempos de jogo e modo de exibição preferido por perfil.
* **🕹️ Navegação Nativa por Controle e Teclado**:
  * Suporte nativo a controles de Xbox (XInput), PlayStation e genéricos (DirectInput).
  * Troca automática e invisível de cursor: ao tocar no analógico ou D-Pad, o cursor do mouse se oculta automaticamente; ao mover o mouse, o cursor retorna instantaneamente.
* **🔄 Atualização Automática Atômica**:
  * Verificação com 1 clique diretamente nas configurações via GitHub Releases pública.
  * Substituição segura com backup automático e rollback em caso de falha.
* **⚙️ Diagnóstico e Compatibilidade**:
  * Verificação e instalação silenciosa de redistribuíveis essenciais (DirectX End-User Runtimes, Visual C++ 2015-2022 x86/x64).
  * Painel de diagnóstico com exportação de pacote de logs `.ZIP` para suporte.

---

## 💻 3. Requisitos de Sistema

| Componente | Requisito Mínimo | Recomendado |
|---|---|---|
| **Sistema Operacional** | Windows 10 (64-bit) versão 1909+ | Windows 10 / 11 (64-bit) versão mais recente |
| **Processador (CPU)** | Intel Core i3 / AMD Ryzen 3 (Dual-Core) | Intel Core i5 / AMD Ryzen 5 (Quad-Core ou superior) |
| **Memória RAM** | 4 GB | 8 GB ou mais |
| **Placa de Vídeo (GPU)** | Compatível com DirectX 11 / OpenGL 3.3 | Placa dedicada compatível com Direct3D 11/12 ou Vulkan |
| **Armazenamento** | 500 MB livres para o launcher e cache de capas | SSD com espaço livre proporcional aos jogos instalados |
| **Rede** | Conexão banda larga para catálogo e downloads | Conexão de alta velocidade (Fibra/Cabo) |

---

## 🚀 4. Como Baixar a Versão Beta

Você pode baixar a versão mais recente diretamente na página de **[Releases](https://github.com/castellorogerio/rog-launcher-releases/releases)**:

1. **Opção 1 — Executável Direto (`ROGLauncher.exe`)**:
   * Arquivo único pré-compilado, pronto para rodar.
   * [Baixar ROGLauncher.exe](https://github.com/castellorogerio/rog-launcher-releases/releases/download/v4.9-beta/ROGLauncher.exe)
2. **Opção 2 — Pacote ZIP Portátil (`ROGLauncher-v4.9-beta-win64.zip`)**:
   * Pacote compactado contendo o executável, instruções e ferramentas auxiliares.
   * [Baixar ROGLauncher-v4.9-beta-win64.zip](https://github.com/castellorogerio/rog-launcher-releases/releases/download/v4.9-beta/ROGLauncher-v4.9-beta-win64.zip)

### Verificação de Integridade (Checksums SHA-256)
Para garantir que o arquivo baixado não foi corrompido, abra o PowerShell e compare a hash:
```powershell
Get-FileHash .\ROGLauncher.exe -Algorithm SHA256
```
Confira a hash oficial no arquivo [`checksums.sha256`](checksums.sha256) anexado à release.

---

## 📥 5. Como Instalar e Iniciar o Launcher

O ROG Launcher é distribuído em formato **portátil** (*portable*), não necessitando de instalador MSI com privilégios de administrador:

1. Baixe o pacote `.zip` ou `.exe`.
2. Mova o arquivo para uma pasta permanente de sua preferência (Exemplo: `C:\Programas\ROGLauncher` ou `D:\ROGLauncher`).
   > Evite executar diretamente da pasta temporária de Downloads ou de arquivos `.zip` sem extrair.
3. Dê um duplo clique em `ROGLauncher.exe`.
4. *(Opcional)* Clique com o botão direito sobre o executável e selecione **Enviar para > Área de trabalho (criar atalho)**.

> [!TIP]
> **Aviso do Windows SmartScreen**: Na primeira execução em sistemas Windows 10/11, o Windows Defender pode exibir a mensagem *"O Windows protegeu o seu computador"*. Clique em **Mais informações** e em seguida em **Executar assim mesmo**. Esse comportamento é normal para softwares de código aberto recentes que ainda não possuem assinatura de certificado comercial pago.

---

## 👥 6. Como Utilizar os Perfis

1. **Criação de Perfil**:
   * Na primeira inicialização, você será recepcionado pela tela de seleção de perfis. Clique em **Novo Perfil**, escolha um nome e, opcionalmente, defina uma senha de 4 a 8 dígitos.
2. **Recortador de Avatar Integrado**:
   * Clique sobre o círculo de foto para escolher qualquer imagem JPG ou PNG do seu computador.
   * A janela de corte interativa permitirá arrastar a imagem com o mouse, dar zoom suave e centralizar o enquadramento.
3. **Alternar de Perfil ou Fazer Logout**:
   * Acesse **Configurações (engrenagem) > Perfil** para alterar nome, senha, trocar o avatar ou clicar em **Sair (Logout)** para bloquear a sessão e retornar à seleção de usuários.

---

## 🎮 7. Como Adicionar e Organizar Jogos

1. **Jogos Steam**:
   * O launcher detecta automaticamente bibliotecas e jogos instalados pela Steam configurados nas suas unidades.
2. **Adicionar Jogos de PC (.exe Manual)**:
   * Acesse a aba **Biblioteca** ou **Adicionados** e clique no botão **Adicionar Jogo Manual**.
   * Localize o executável principal (`.exe`) do jogo. O launcher buscará metadados e capas automaticamente pelo nome do título.
3. **Filtros e Visualização**:
   * Na Biblioteca, alterne entre a visualização **☵ Grade** e **▬ Console** no canto superior direito. Sua escolha é salva individualmente por perfil.
   * Utilize a barra de pesquisa rápida para filtrar sua biblioteca instantaneamente.

---

## 🔄 8. Como Verificar e Instalar Atualizações

O ROG Launcher possui um sistema de atualização automático integrado:

1. Clique no ícone de **Configurações** (engrenagem) no topo da tela.
2. Na categoria **Geral**, localize o card **Atualização do Aplicativo**.
3. Clique em **Verificar Atualizações**.
4. Se houver uma nova versão, clique em **Baixar Atualização**. Acompanhe a barra de progresso em tempo real.
5. Quando o download terminar, clique em **Reiniciar e Instalar Agora**. O launcher aplicará a atualização atomicamente e reabrirá pronto para jogar.

---

## 🛠️ 9. Solução de Problemas Comuns

Consulte o documento completo em [TROUBLESHOOTING.md](TROUBLESHOOTING.md) para detalhes aprofundados. Destaques:

* **O jogo não abre ao clicar em Jogar**:
  * Verifique se o executável de destino não foi movido de pasta.
  * Acesse **Configurações > Compatibilidade** e clique em **Instalar Todos os Componentes** para garantir que as DLLs do DirectX 9/11 e Visual C++ estão instaladas.
* **Downloads lentos ou sem conectar**:
  * Certifique-se de que o seu antivírus ou firewall não está bloqueando o motor `tools/aria2c.exe`.
  * Verifique se a pasta de downloads definida em **Configurações > Downloads** possui permissão de gravação.

---

## 📢 10. Como Enviar Relatórios de Erros

Se encontrar alguma anomalia:

1. Acesse **Configurações > Diagnóstico e Logs**.
2. Clique no botão **Exportar Pacote de Diagnóstico (.ZIP)**. Um arquivo `.zip` com os logs relevantes (filtrados de informações pessoais) será gerado.
3. Abra uma issue em: **[GitHub Issues](https://github.com/castellorogerio/rog-launcher-releases/issues)**.
4. Descreva o que aconteceu, o modelo do seu controle (se aplicável) e anexe o relatório.

---

## 📜 11. Histórico de Versões

* **v4.9-beta (Atual)**:
  * Catálogo com busca de alta precisão via Steam API e filtro exclusivo com fontes ativas.
  * Novo Modo Console na Biblioteca pessoal com carrossel dinâmico e Hero responsivo.
  * Toast global de download concluído com z-index alto e novo efeito sonoro harmônico.
  * Otimizações no motor aria2c: remoção de estrangulamento de upload, trackers públicos integrados e cálculo de ETA corrigido.
  * Novo sistema de atualização automática via GitHub Releases com substituição atômica.
  * Recortador interativo de fotos de avatar com proporção circular.
* **v4.8-beta**:
  * Controles de áudio e vídeo aprimorados, compatibilidade com monitores de diferentes resoluções.
* **v4.7-beta**:
  * Implementação da fila assíncrona de downloads e integração inicial de fontes.

Para ver o histórico detalhado, acesse [CHANGELOG.md](CHANGELOG.md).

---

## ⚖️ 12. Licença

Este projeto é disponibilizado sob a licença **MIT**. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.

---

<p align="center">
  Desenvolvido por <strong>Rogério Castello</strong> • ROG Launcher Team<br>
  <em>Feito para jogadores que valorizam liberdade, velocidade e um visual premium.</em>
</p>
