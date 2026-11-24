```markdown
# 🍎 Detector Inteligente de Frutas e Qualidade

Este projeto consiste em um sistema inteligente capaz de classificar frutas e avaliar o seu estado de qualidade (boas ou ruins para o consumo). Ele utiliza Visão Computacional tradicional (OpenCV) para isolar as frutas do fundo da imagem e uma Rede Neural Convolucional profunda (baseada na arquitetura **MobileNetV2** via Transfer Learning) para realizar a inferência de 10 classes.

Uma interface gráfica web e interativa foi desenvolvida utilizando a biblioteca **Gradio**, permitindo que qualquer pessoa envie uma imagem para analisar a fruta em tempo real.

## 🚀 Como Executar o Projeto

Qualquer usuário pode rodar a aplicação diretamente no navegador sem a necessidade de configurar ambientes locais complexos ou realizar o treinamento demorado do modelo, pois o sistema está configurado para baixar o modelo pré-treinado automaticamente.

### Passo a Passo para Execução:

1. **Abra o Notebook no Google Colab:**
   Clique no botão abaixo para abrir o notebook de desenvolvimento diretamente no ambiente do Google Colab:
   
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](SUA_URL_DO_NOTEBOOK_NO_COLAB_AQUI)

2. **Configure suas Credenciais do Kaggle (Opcional):**
   * O notebook necessita do dataset original para fins de avaliação de métricas.
   * Na primeira célula (**Etapa 1**), o script solicitará interativamente o seu **Kaggle Username** e a sua **Kaggle Key**. Se você não tiver uma conta, você pode criá-la gratuitamente no site do [Kaggle](https://www.kaggle.com/) e gerar sua API Key nas configurações do seu perfil.

3. **Baixe o Modelo Pré-Treinado Automaticamente:**
   * O notebook conta com um script de download automatizado na **célula de ID 0ac4b148**.
   * Ao executar a célula de carregamento do modelo, o notebook fará o download do arquivo `modelo_frutas_v3.keras` de um repositório público do Google Drive criado pelo desenvolvedor. Isso elimina a necessidade de treinar a inteligência artificial do zero (o que levaria bastante tempo).

4. **Inicie a Interface Web do Gradio:**
   * Vá até a última célula do notebook (**Etapa 8**) e execute-a.
   * O Gradio gerará um link público temporário no console do Colab (ex: `https://xxxx.gradio.live`).
   * Clique no link gerado para abrir a interface em uma nova guia, envie a imagem de uma fruta e veja o diagnóstico completo do modelo!

## 📂 Estrutura do Pipeline

1. **Segmentação (OpenCV):** Remove o fundo desnecessário aplicando conversões para o espaço HSV, filtros gaussianos e a máscara morfológica pelo algoritmo de Otsu.
2. **Classificação (Deep Learning):** A imagem recortada é enviada à rede MobileNetV2 refinada para prever o percentual de certeza das classes.
3. **Interface Gráfica (Gradio):** Apresenta o resultado de forma intuitiva, exibindo a imagem original, a máscara de isolamento, a fruta segmentada e um gráfico de barras com as probabilidades de acerto.

---
Desenvolvido com 💻, TensorFlow e OpenCV por [Seu Nome](https://github.com/seu-usuario).
