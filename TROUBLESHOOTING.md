# Guia de Solução de Problemas (Troubleshooting) — ROG Launcher

Este documento reúne os diagnósticos e soluções para os problemas e dúvidas mais comuns encontrados durante a instalação e uso do ROG Launcher.

---

## 1. O aplicativo não abre ou fecha imediatamente após iniciar

### Causas comuns:
* **Falta de componentes de tempo de execução C++**:
  * *Solução*: Baixe e instale o pacote [Microsoft Visual C++ Redistributable 2015-2022 (x64)](https://aka.ms/vs/17/release/vc_redist.x64.exe).
* **Bloqueio pelo antivírus**:
  * Determinados antivírus corporativos ou heurísticos podem emitir falsos-positivos sobre novos executáveis empacotados por PyInstaller.
  * *Solução*: Adicione a pasta do ROG Launcher à lista de exceções do seu antivírus ou Windows Defender.

---

## 2. Erro "av1_mf could not find any MFT" ou avisos de codecs no log

* Esses avisos referem-se à ausência de decodificadores de hardware específicos (como AV1 ou HEVC) no Media Foundation do Windows para trailers e vídeos de apresentação.
* **Impacto**: O launcher continuará funcionando normalmente em modo de áudio e imagem estática sem qualquer perda de dados ou instabilidade funcional.

---

## 3. Downloads travados ou velocidade em 0 KB/s

### Causas e Soluções:
* **Bloqueio do motor aria2c**:
  * O motor de downloads assíncronos está localizado na pasta `tools/aria2c.exe`. Verifique se o Firewall do Windows não bloqueou a comunicação de rede do executável.
* **Permissão na pasta de downloads**:
  * Acesse **Configurações > Downloads** e confira o caminho da pasta padrão de downloads. Evite diretórios protegidos do sistema (como `C:\Windows` ou a raiz de `C:\`).
* **Swarm de Torrent sem sementes (seeders)**:
  * Repacks muito antigos podem ter poucos pares ativos. O launcher continuará tentando conectar via DHT e trackers públicos configurados.

---

## 4. O jogo instalado não inicia ao clicar em "Jogar"

1. Acesse os detalhes do jogo ou clique nos três pontos (`···`) e selecione **Configurar Executável**.
2. Certifique-se de que o caminho apontado corresponde ao `.exe` real do jogo e não a um arquivo de desinstalação ou launcher intermediário.
3. Se o jogo exigir privilégios de administrador para salvar dados, execute o ROG Launcher como Administrador.

---

## 5. Como Exportar e Enviar Logs de Diagnóstico

Se o problema persistir:

1. Abra o ROG Launcher e clique no ícone de **Configurações** (engrenagem).
2. Vá até a categoria **Diagnóstico e Logs**.
3. Clique em **Exportar Pacote de Diagnóstico (.ZIP)**.
4. O launcher empacotará os arquivos de log recentes com mascaramento automático de dados confidenciais.
5. Abra uma issue em nosso repositório no GitHub:  
   👉 [https://github.com/castellorogerio/rog-launcher-releases/issues](https://github.com/castellorogerio/rog-launcher-releases/issues)  
   e anexe o arquivo `.zip` para análise técnica.
