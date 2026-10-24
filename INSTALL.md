# Guia de Instalação e Configuração — ROG Launcher

Este documento fornece o passo a passo completo para instalar, configurar e iniciar o **ROG Launcher** no Windows 10 e Windows 11 (64-bit).

---

## 📋 Pré-requisitos do Sistema

1. **Sistema Operacional**: Windows 10 (versão 1909 ou superior) ou Windows 11 de 64 bits.
2. **Bibliotecas de Sistema**:
   * O ROG Launcher vem compilado como um aplicativo autocontido (Standalone).
   * Para a execução de determinados jogos antigos adicionados à biblioteca, recomenda-se ter os runtimes do Visual C++ 2015-2022 e DirectX instalados (você pode instalá-los diretamente pelo launcher em **Configurações > Compatibilidade**).

---

## 📦 Método 1: Instalação via Executável Direto (`ROGLauncher.exe`)

1. Acesse a página de **[Releases Públicas](https://github.com/castellorogerio/rog-launcher-releases/releases)** ou baixe diretamente os pacotes da versão atual.
2. Baixe o arquivo **`ROGLauncher.exe`**.
3. Crie uma pasta para o aplicativo em um disco com boa velocidade (por exemplo: `C:\Jogos\ROGLauncher` ou `D:\ROGLauncher`).
4. Mova o executável baixado para dentro dessa pasta.
5. Dê um duplo clique para iniciar.

---

## 🗜️ Método 2: Instalação via Arquivo ZIP Portátil

1. Baixe o pacote compactado **`ROGLauncher-v4.9-beta-win64.zip`**.
2. Clique com o botão direito sobre o arquivo `.zip` e selecione **Extrair Tudo...**.
3. Escolha uma pasta de destino permanente.
4. Abra a pasta extraída e execute **`ROGLauncher.exe`**.

---

## 🛡️ Alerta do Windows Defender SmartScreen

Como o ROG Launcher é um projeto de distribuição independente e recente, o Windows pode exibir uma tela azul com o aviso:
> *"O Windows protegeu o seu computador - O Microsoft Defender SmartScreen impediu a inicialização de um aplicativo não reconhecido."*

### Como prosseguir com segurança:
1. Clique no link **"Mais informações"** localizado abaixo do texto principal.
2. Clique no botão **"Executar assim mesmo"**.
3. O launcher será iniciado normalmente. O Windows salvará a aprovação para as próximas execuções.

---

## 🎮 Primeira Execução e Criação de Perfil

1. Ao abrir o ROG Launcher pela primeira vez, será exibida a tela de seleção de perfis.
2. Clique em **Criar Perfil** ou utilize o perfil padrão pré-configurado.
3. Se desejar, defina uma senha de bloqueio.
4. Clique no ícone de imagem do perfil para selecionar uma foto e utilize a ferramenta integrada de corte para ajustá-la em formato circular.
5. Pronto! Você será direcionado à **Home** do launcher.

---

## 🕹️ Configuração do Controle

* **Xbox One / Series / 360**: Conecte via USB ou Bluetooth. O reconhecimento é automático e instantâneo via XInput.
* **PlayStation (DualShock 4 / DualSense)**: Reconhecido nativamente ou com suporte DirectInput.
* O cursor do mouse desaparecerá automaticamente ao navegar pelos direcionais do controle e reaparecerá assim que o mouse for movimentado.
