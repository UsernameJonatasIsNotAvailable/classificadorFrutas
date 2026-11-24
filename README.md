# 🍎 Detector Inteligente de Frutas e Qualidade

Este projeto identifica 5 tipos de frutas (maçã, banana, laranja, goiaba e limão) e classifica se estão boas ou ruins para consumo usando Inteligência Artificial e Visão Computacional.

## 🚀 Como Executar o Projeto em 1 Clique

Qualquer pessoa pode rodar e testar o aplicativo diretamente no navegador pelo Google Colab (sem precisar treinar o modelo do zero):

1. **Abra o Notebook no Google Colab:**
   Clique no botão abaixo para abrir o ambiente de execução:
   
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Nwyr1vaJ9xjFpVTxQm2QvJJEfhGkLyJg#scrollTo=_xdVrEBiW2HB)

2. **Execute as Células:**
   * No menu superior do Colab, clique em **Ambiente de execução** > **Executar tudo** (ou use o atalho `Ctrl + F9`).
   * **🔑 Passo Importante (Autenticação do Kaggle):**
     Como o notebook usa imagens reais de teste, ele precisa fazer o download do dataset do Kaggle de forma segura. Por segurança, suas senhas não ficam expostas no código público. Durante a execução da primeira célula, o Colab abrirá duas caixas de texto para você preencher:
     
     * **Kaggle Username:** Seu nome de usuário do Kaggle.
     * **Kaggle Key:** Sua chave de API privada.
     
     *Caso ainda não tenha uma chave do Kaggle, é gratuito e rápido:* 
     1. Crie uma conta no [Kaggle](https://www.kaggle.com/).
     2. Vá nas configurações do seu perfil (Settings) e clique em **Create New Token** para baixar um arquivo chamado `kaggle.json` contendo seu usuário e sua chave.

3. **Abra o Aplicativo:**
   * Ao chegar na última célula (**Etapa 8**), um link público temporário do **Gradio** será gerado (ex: `https://xxxx.gradio.live`).
   * Basta clicar no link, enviar a foto de uma fruta e ver o resultado na hora!
