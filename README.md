# Sistema de Conversão de Voz com GPT

Repositório para o trabalho da disciplina de Tópicos Especiais em Computação

Higor D. Oliveira, Kaique S. Passos, Victor F. Rocha

- [Descrição](#descricao)
- [Funcionalidades](#funcionalidades)
- [Como funciona](#como-funciona)
- [Como Usar no Google Colab](#como-usar-no-google-colab)
- [Demonstração no Collab](#demonstração-no-collab)
- [Requisitos Collab](#como-funciona)
- [Instalação na versão Ubuntu](#instalação-na-versão-ubuntu)
- [Demonstração no Ubuntu](#demonstração-no-ubuntu)

- [Link para Relatório](#relatório)

Este é um sistema completo de conversão de voz em texto, interação com um modelo de linguagem e conversão do texto gerado de volta em fala, utilizando tecnologias de ponta como **Whisper**, **Grok API**, **DeepSeek**, e **gTTS**. O sistema funciona de maneira totalmente integrada no **Google Colab**, facilitando o uso sem a necessidade de configurações locais complicadas.

  ## Descricao

Este sistema é projetado para realizar a conversão de voz em texto, interagir com um modelo de linguagem, e transformar a resposta em texto de volta para voz. Ele utiliza:

1. **Whisper** (da OpenAI) para transcrever a fala do usuário em texto.
2. **Grok API** para interagir com o modelo de linguagem da DeepSeek e gerar respostas inteligentes.
3. **gTTS (Google Text-to-Speech)** para converter a resposta gerada em texto novamente para fala.

Com isso, é possível criar uma interface de voz natural e interativa usando modelos de IA e voz.

  ## Funcionalidades

- **Conversão de Fala em Texto**: A entrada de voz do usuário é convertida em texto utilizando a tecnologia **Whisper**.
- **Geração de Respostas Inteligentes**: O texto gerado é processado pela **API do Grok**, que utiliza o modelo de linguagem da **DeepSeek** para gerar respostas.
- **Conversão de Texto em Fala**: A resposta gerada pelo modelo é convertida de volta em fala usando a **gTTS**.

  ## Como Funciona

O sistema opera diretamente no Google Colab, o que facilita o acesso e a execução do código sem a necessidade de instalar dependências localmente. Para usar:

1. **Passo 1**: Gravação de audio através do Colab.
2. **Passo 2**: O áudio é processado pelo **Whisper** para transcrição em texto.
3. **Passo 3**: O texto é enviado para a **API do Grok**, que gera uma resposta inteligente.
4. **Passo 4**: A resposta é convertida em áudio novamente utilizando o **gTTS** e reproduzida.

## Como Usar no Google Colab

1. Acesse o [notebook do Google Colab](https://colab.research.google.com/drive/1X8tVAKdJyhdgOnTGtgWfoX4O4T8Ft85y?usp=drive_link) e execute as células para rodar o sistema.
2. Certifique-se de ter permissões adequadas para usar as APIs do **Grok** e **DeepSeek**.
3. Siga os passos no notebook para enviar áudio e ouvir a resposta gerada.

## Demonstração No Collab

Confira uma demonstração do sistema em funcionamento no seguinte vídeo:

[Link para o vídeo de demonstração](https://youtu.be/f3TB-Pr63QU)

## Requisitos no Collab

- Google Colab
- Conta na API do Grok
- Biblioteca `whisper` para transcrição de fala
- Biblioteca `gTTS` para conversão de texto em fala
- Conexão com a internet para acessar as APIs

## Instalação na versão Ubuntu

  Você vai precisar da cuDNN para rodar o script. Siga as instruções de instalação no site oficial. O link a seguir já está selecionado para Ubuntu 24.04

  https://developer.nvidia.com/cudnn-downloads?target_os=Linux&target_arch=x86_64&Distribution=Ubuntu&target_version=24.04&target_type=deb_local

  Para instalar os pacotes necessários:

    pip install -r requirements.txt

  Para rodar o script
  
    python3 VoiceGPT.py

## Demonstração No Ubuntu

Demonstração do fluxo de conversa no Ubuntu

[Link do vídeo](https://youtu.be/OlKZTT0qIfY)

## Relatório

[Link para o relatório](https://github.com/vfrocha/Sistema-de-Conversao-de-Voz-com-GPT/blob/main/paper.pdf)
