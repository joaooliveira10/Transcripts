# 🎙️ Transcript

## 📝 Transcrição de Áudio e Vídeo com IA

**Transcript** é uma aplicação web desenvolvida em Python que utiliza a API da OpenAI (modelo Whisper) para transformar facilmente áudio e vídeo em texto. Com uma interface intuitiva construída em Streamlit, você pode transcrever arquivos de áudio, vídeos ou utilizar o microfone para captação em tempo real.

## 🔧 Pré-requisitos

- Python 3.8 ou superior
- Conta na OpenAI com chave de API
- Conexão com a internet

## 📋 Dependências

O projeto utiliza as seguintes bibliotecas:

```
openai
streamlit==1.33.0
streamlit_webrtc
python-dotenv
moviepy
pydub
ipykernel
```

## ⚙️ Instalação

1. Clone o repositório:

```bash
git clone https://github.com/joaooliveira10/Transcripts.git
cd Transcripts
```

2. Crie e ative um ambiente virtual:

```bash
python -m venv venv
# No Windows
venv\Scripts\activate
# No macOS/Linux
source venv/bin/activate
```

3. Instale as dependências:

```bash
pip install -r requirements.txt
```

4. Configure suas credenciais da OpenAI:

   - Crie um arquivo `.env` na raiz do projeto
   - Adicione sua chave de API: `OPENAI_API_KEY=sua_chave_aqui`

5. Crie uma pasta para arquivos temporários:

```bash
mkdir -p temp
```

## 🚀 Como executar

Execute o aplicativo Streamlit:

```bash
streamlit run 07_aula.py
```

O aplicativo abrirá automaticamente no seu navegador padrão, normalmente em `http://localhost:8501`.

## 📌 Como usar

### 🎤 Transcrição via Microfone

1. Clique na aba "Microfone"
2. (Opcional) Digite um prompt para guiar a transcrição
3. Clique no botão "Start" para iniciar a captura de áudio
4. Fale no seu microfone
5. A transcrição aparecerá na tela conforme você fala
6. Clique em "Stop" quando terminar

### 🎬 Transcrição de Vídeo

1. Selecione a aba "Vídeo"
2. (Opcional) Digite um prompt para guiar a transcrição
3. Faça upload de um arquivo de vídeo MP4
4. Aguarde o processamento
5. A transcrição completa será exibida na tela

### 🔊 Transcrição de Áudio

1. Selecione a aba "Áudio"
2. (Opcional) Digite um prompt para guiar a transcrição
3. Faça upload de um arquivo de áudio MP3
4. A transcrição será gerada e exibida automaticamente

## 💡 Recursos e Funcionalidades

- Transcrição em tempo real via microfone
- Extração e transcrição de áudio de arquivos de vídeo
- Transcrição direta de arquivos de áudio
- Suporte para prompts personalizados para melhorar a precisão da transcrição
- Interface intuitiva com abas para diferentes métodos de entrada
