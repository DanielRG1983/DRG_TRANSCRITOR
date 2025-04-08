

Transcritor – By DanielRG – PCPI
O Transcritor é uma aplicação de interface gráfica desenvolvida em Python que automatiza o processo de conversão e transcrição de arquivos de mídia (áudio e vídeo). Utilizando diversas bibliotecas, como pydub e speech_recognition, a aplicação permite que o usuário converta arquivos para o formato WAV, divida o áudio em trechos menores e transcreva cada segmento por meio da API do Google para reconhecimento de voz. Toda essa funcionalidade é apresentada em uma interface moderna e intuitiva construída com CustomTkinter.

Funcionalidades Principais
Conversão de Mídia:

A aplicação suporta vários formatos de áudio e vídeo (ex: .mp3, .mp4, .avi, .flac, .ogg, etc.).

Se necessário, arquivos que não estejam no formato WAV são convertidos automaticamente utilizando o ffmpeg.exe (que deve estar na mesma pasta do executável ou empacotado com a aplicação).

Segmentação e Transcrição:

O áudio é dividido em segmentos (por padrão, de 60 segundos), facilitando o processamento e melhorando a robustez da transcrição.

Cada segmento é transcrito automaticamente utilizando a API do Google Speech Recognition com suporte para o idioma pt-BR.

As transcrições geradas para cada segmento são concatenadas para formar a transcrição final do arquivo.

Para cada mídia processada, é salvo um arquivo de texto individual e também é gerado um arquivo consolidado com todas as transcrições.

Interface Gráfica Intuitiva:

Seleção de Arquivos/Pastas: O usuário pode escolher uma pasta contendo diversos arquivos de mídia ou selecionar arquivos individuais.

Seleção do Destino: É possível definir uma pasta para salvar os arquivos de transcrição.

Feedback em Tempo Real: A interface inclui uma barra de progresso e uma área de log que exibe mensagens detalhadas do andamento do processamento.

Informações e Doação: Informações do desenvolvedor, juntamente com um QR Code para doação, são exibidas automaticamente ao iniciar e ao fechar a aplicação.

Operação Multithread:

O processamento (que pode ser demorado para arquivos grandes) é executado em uma thread separada, mantendo a interface responsiva durante a transcrição.

Como a Aplicação Funciona
Inicialização e Configuração:

Ao iniciar, a aplicação exibe sua interface gráfica com opções para selecionar os arquivos de mídia (ou uma pasta inteira), escolher o destino para salvar as transcrições e visualizar informações do desenvolvedor.

Um QR Code para doação é exibido automaticamente logo após a abertura e novamente ao fechar o aplicativo, reforçando a possibilidade de apoio ao projeto.

Seleção de Arquivos e Pastas:

O usuário pode clicar nos botões "Selecionar Pasta" ou "Selecionar Arquivos" para informar a origem dos arquivos de mídia.

Um campo específico é utilizado para definir a pasta de destino onde os arquivos de transcrição serão salvos.

Processamento dos Arquivos:

Quando o usuário clica em "Executar", a aplicação:

Converte os arquivos para WAV, se necessário, utilizando o ffmpeg.exe.

Divide o áudio em chunks (segmentos) de 60 segundos para facilitar a transcrição.

Transcreve cada chunk individualmente utilizando a API do Google, capturando possíveis erros e tentando novas tentativas em caso de falhas de conexão.

Combina as transcrições dos chunks em um único texto, salvando um arquivo .txt para cada mídia e gerando também um arquivo consolidado com todas as transcrições.

Feedback e Monitoramento:

Durante o processamento, uma barra de progresso e uma área de log fornecem informações em tempo real sobre o andamento, exibindo mensagens como "Áudio carregado", "Chunk transcrito", "Removido arquivo temporário", entre outras.

Caso algum erro ocorra (por exemplo, falha na conversão ou na transcrição), a aplicação registra a mensagem de erro no log para facilitar o diagnóstico.

Finalização:

Ao concluir o processamento de todos os arquivos, o usuário é notificado por meio de uma mensagem de sucesso.

O QR Code para doação é novamente exibido antes do fechamento da aplicação, permitindo que o usuário saiba onde ajudar no projeto.

Tecnologias Utilizadas
Python 3.9+: Linguagem de programação utilizada no desenvolvimento.

CustomTkinter: Biblioteca para criação de interfaces gráficas modernas e responsivas.

pydub: Utilizada para manipulação e conversão de arquivos de áudio.

speech_recognition: Responsável pela transcrição de áudio utilizando a API do Google.

ffmpeg: Ferramenta externa utilizada para converter vídeos e áudios para o formato WAV.

Pillow (PIL): Utilizada para manipular imagens, como exibição do QR Code.

PyInstaller: Ferramenta para empacotar o projeto em um único executável, incluindo todos os arquivos necessários.

Instruções de Uso
Pré-requisitos:

Certifique-se de ter o ffmpeg.exe e o QRCODE.jpeg na mesma pasta do aplicativo (ou empacotados com o executável).

Instale todas as dependências Python (consulte o arquivo requirements.txt se disponível).

Execução:

Rode o aplicativo via Python (python DRG_TRANSCRITOR_V7.py) ou, após empacotar, execute o arquivo .exe gerado (na pasta dist).

Na interface, selecione os arquivos ou a pasta de mídia a ser processada e defina a pasta de destino para os relatórios.

Processamento:

Clique em "Executar" para iniciar a conversão, segmentação e transcrição.

Acompanhe o andamento pelo log e pela barra de progresso.

Finalização:

Ao término, os arquivos de transcrição serão salvos individualmente e em um arquivo consolidado.

O aplicativo exibirá também uma mensagem de sucesso e o QR Code para doação aparecerá ao fechar a aplicação.

