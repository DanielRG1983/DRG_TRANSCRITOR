# DRG_TRANSCRITOR

**Transcritor – By DanielRG – PCPI** é um aplicativo de interface gráfica para conversão e transcrição automática de arquivos de mídia (áudio e vídeo). Desenvolvido em Python e empacotado com PyInstaller, o programa converte arquivos para o formato WAV, segmenta o áudio e utiliza a API do Google Speech Recognition para gerar transcrições – tudo por meio de uma interface intuitiva construída com CustomTkinter.

## Visão Geral

O Transcritor foi criado para facilitar a conversão e transcrição de arquivos de mídia. Com ele, o usuário pode:

- **Converter** automaticamente vários formatos de mídia para o formato WAV (utilizando o `ffmpeg.exe`);
- **Dividir** o áudio em segmentos (chunks de 60 segundos) para uma transcrição mais eficaz;
- **Transcrever** cada segmento automaticamente com a API do Google (pt-BR);
- **Salvar** as transcrições em arquivos `.txt` individuais e em um arquivo consolidado;
- Acompanhar o andamento do processamento via uma **barra de progresso** e uma área de **log de status**;
- Visualizar informações do desenvolvedor e receber o **QR Code para doação** (exibido ao iniciar e ao fechar o aplicativo).

## Como Usar

Este repositório disponibiliza apenas o executável da aplicação; o código-fonte não será divulgado.

### Requisitos

- **Windows** (o executável foi gerado para esse sistema).
- Os arquivos **ffmpeg.exe** e **QRCODE.jpeg** já estão incluídos junto ao executável.

### Execução

**IMPORTANTE:**  
- Desative o antivírus ou crie uma exceção para a aplicação;  
- Execute o aplicativo como administrador.

1. Extraia todos os arquivos da distribuição (eles devem estar na mesma pasta).  
2. Execute o arquivo `DRG_TRANSCRITOR_V7.exe`.  
3. Na interface:
   - Selecione a pasta contendo os arquivos de mídia ou escolha arquivos individuais.
   - Defina a pasta de destino onde serão salvos os arquivos de transcrição.
   - Clique no botão **Executar** para iniciar o processamento.
4. Durante a execução, a barra de progresso e o log exibem as etapas do processo.
5. Ao fechar a aplicação, um QR Code para doação será exibido.

## Distribuição e Licença

- **Uso Livre:** Este aplicativo é de uso livre.
- **Executável Único:** Apenas o executável será disponibilizado, facilitando o uso pelo usuário final sem necessidade de instalar dependências.
- Sinta-se à vontade para compartilhar e utilizar o Transcritor conforme sua necessidade.

## Sobre o Desenvolvedor

Desenvolvido por:  
**DANIEL RODRIGUES GUIMARÃES**  
Agente de Polícia Civil do Estado do Piauí – Diretoria de Inteligência (PCPI)  
Bacharel em Ciência da Computação  
Pós-Graduado em Perícia Cibernética  
Pós-Graduado em Engenharia de Software

[DRG_TRANSCRITOR no GitHub](https://github.com/DanielRG1983/DRG_TRANSCRITOR)
