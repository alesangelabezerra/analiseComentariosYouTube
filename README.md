#  TÉCNICAS DE ANÁLISE DE DADOS
## DASHBOARD ANÁLISE DE COMENTÁRIOS DO YOUTUBE

<h3>SOBRE O PROJETO</h3>

### INTRODUÇÃO

O objetivo deste projeto é analisar o sentimento e as tendências nos comentários de um vídeo específico do YouTube. Onde eu quis entender melhor como o público reage ao conteúdo do vídeo, analizando como os sentimentos variam ao longo do tempo. Calculando cada comentário como positivo, negativo ou neutro. E mostrar as palavras mais frequentes nos comentários, o que pode dar insights sobre os tópicos mais discutidos.

### TÉCNICAS UTILIZADAS

Raspagem de Dados: Usamos a API do YouTube, que fez a coleta dos comentários de um vídeo específico.

Processamento de Linguagem Natural (NLP): Aplicamos técnicas de NLP, como análise de sentimentos, usando a biblioteca TextBlob que criou uma nuvem de palavras para visualizar os termos mais frequentes nos comentários.

### COLETA E PREPARAÇÃO DOS DADOS

API do YouTube: Configuramos a API do YouTube para acessar os comentários, filtrando os dados relevantes.

Limpeza dos Dados: Implementamos a remoção de stopwords que fosse retirada algumas palavras e caracteres irrelevantes.

Análise de Sentimento: Utilizamos TextBlob para analisar a polaridade dos sentimentos nos comentários.

### Análises

**DISTRIBUIÇÃO DE SENTIMENTOS NOS COMENTÁRIOS**

Este gráfico de barras mostra a proporção de comentários positivos, negativos e neutros. Ele oferece uma visão geral do tom emocional dos comentários do vídeo.

**EVOLUÇÃO DOS SENTIMENTOS AO LONGO DO TEMPO**

Este gráfico de linha traça a variação dos sentimentos (positivo, negativo, neutro) ao longo do tempo, mostrando como as reações do público mudaram no decorrer do tempo.

**GRÁFICO DE PALAVRAS MAIS FREQUENTES**

Este gráfico de barras exibe as palavras mais frequentes e suas contagens, revelando os termos mais destacados e recorrentes nos comentários.

**NUVEM DE PALAVRAS MAIS COMUNS NOS COMENTÁRIOS**

Utilizamos uma nuvem de palavras que destaca as palavras mais frequentes nos comentários. Palavras maiores indicam maior frequência, oferecendo insights sobre os temas mais discutidos.


<h3>Informações para rodar o projeto</h3>


**Obtendo a CHAVE_API**

Guia para Obter a Chave API do Google Cloud para usar com a API do YouTube

Passo 1: Crie uma conta no Google Cloud
- Acesse https://cloud.google.com/ e crie uma conta ou faça login se já tiver uma.

Passo 2: Crie um novo projeto no Google Cloud
- No console do Google Cloud, vá para o Dashboard e crie um novo projeto.

Passo 3: Ative a API do YouTube Data
- No menu 'Library' do console do Google Cloud, procure por 'YouTube Data API v3' e ative-a para o seu projeto.

Passo 4: Crie uma chave de API
- No console, vá para 'Credentials' e clique em 'Create credentials'.
- Escolha 'API key'. Após a criação, a chave da API será exibida.

Passo 5: Restrinja a chave (opcional, mas recomendado para segurança)
- Você pode restringir a chave para ser usada apenas com a API do YouTube e limitar os IPs que podem usá-la.

Passo 6: Use a chave em seu código
- Em seu código Python, use esta chave para autenticar suas solicitações à API do YouTube.
  Exemplo: 
  youtube = build('youtube', 'v3', developerKey='SUA_CHAVE_AQUI')

Lembre-se: Mantenha sua chave API segura e não a compartilhe publicamente.

**OBTENDO O ID DO VIDEO**

Você encontra o ID do video na URL.
Ex.: https://www.youtube.com/watch?v=abcdefghijk
O ID de video é abcdefghijk

**BIBLIOTECAS QUE PRECISAM SER INSTALADAS**

pip install google-api-python-client textblob pandas plotly wordcloud nltk gensim

**COMANDOS PARA RODAR E VISUALIZAR O DASHBOARD**
 python app.py
 O Dashboard poderá ser visto no endereço "http://localhost:8050"

