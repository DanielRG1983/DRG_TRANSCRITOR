# DRG_TRANSCRITOR
# Transcritor – By DanielRG – PCPI é um aplicativo de interface gráfica para conversão e transcrição automática de arquivos de mídia (áudio e vídeo). Desenvolvido em Python e empacotado com PyInstaller, o programa converte arquivos para o formato WAV, divide o áudio em segmentos e utiliza a API do Google Speech Recognition para gerar transcrições – tudo por meio de uma interface intuitiva construída com CustomTkinter.

Visão Geral
Esta aplicação foi criada para facilitar a transcrição de arquivos de áudio e vídeo. Com ela, o usuário pode:

Converter automaticamente diversos formatos de mídia para o formato WAV (usando o ffmpeg.exe);

Dividir o áudio em segmentos (chunks) para uma transcrição mais eficiente;

Transcrever cada segmento utilizando a API do Google Speech Recognition (pt-BR);

Salvar as transcrições em arquivos de texto individuais e em um arquivo consolidado;

Acompanhar o andamento do processamento através de uma barra de progresso e um log de status;

Visualizar informações do desenvolvedor e um QR Code para doação (exibido na abertura e ao fechar o aplicativo).

Como Usar
Este repositório disponibiliza somente o executável da aplicação – o código-fonte não será divulgado.

Requisitos
Windows (o executável foi gerado para Windows).

Os arquivos ffmpeg.exe e QRCODE.jpeg já estão incluídos junto ao executável.

Execução
IMPORTANTE:

## Desative o antivírus ou crie uma exceção para a aplicação;

## Execute o aplicativo como administrador.

Extraia todos os arquivos da distribuição (eles devem estar na mesma pasta).

Execute o arquivo DRG_TRANSCRITOR_V7.exe.

Na interface:

Selecione a pasta contendo os arquivos de mídia ou escolha arquivos individuais.

Defina a pasta de destino para salvar os arquivos de transcrição.

Clique no botão Executar para iniciar o processamento.

Durante a execução, a barra de progresso e o log exibem as etapas do processo.

Ao fechar a aplicação, um QR Code para doação será exibido.

Distribuição e Licença
## Uso Livre: Este aplicativo é de uso livre.

Executável Único: Apenas o executável será disponibilizado a fim de facilitar o uso pelo usuário final, sem necessidade de instalação de dependências.

Sinta-se à vontade para compartilhar e utilizar este aplicativo conforme sua necessidade.
