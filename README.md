## gemini-ia

### Imersão Inteligência Artificial 2ª Edição (Alura)

#### Arquivo "ChatBot_Aula04_ImersaoIA(V2).ipynb" é o projeto da aula 04 onde foi criado um ChatBot integrado com o Google Gemini usando a API Key.
------------------------------------------------------------------------------------------

## AI Studio

#### Temperatura: serve para deixar o Gemini mais preciso

#### Quanto mais próximo do "0", mais "preciso" ele ficará (mais especifica de controle);
- A resposta vai ser quase sempre igual
- De acordo com as palavras que ele aprendeu;

#### Quanto mais alta a temperatura, mais criativa o Gemini fica;
- É como pegar várias palavras, colocar num saquinho e pegar aleatóriamente
- Não será sempre a palavra mais precisa num conexto específico
- Será mais criativo
- Exemplo: Viagens e roles (locais mais pesquisados), palaras mais digitadas

#### Usando o IA Studio, temperatura 0 e depois 1, use o prompt:
- Escreva um tuíte curto sobre o Japão.

#### Add Stop Sequence
- definir que conjunto de caracteres, que sequencia ira usar para o modelo marcar como final da crianção
- ficando mais claro onde ira finalizar
- categoria de escape, aspa, barra
- automatiza algumas coisas
- Exemplo: simples, apenas um "." (ponto de texto)

#### Usar este prompt:
- Escreva um texto sobre o Japão.

#### Safety settings
- parametros de segurança
- podendo bloquear ou desbloquear alguns filtros
- deixa o modelo para uso geral (perfil da pessoa)
- somente usado para fins de estudo (bloquear ou detectar discursos hate/sexuais/preconceitos)
- com isso conseguimos detectar esses conteudos, podendo ter um cuidado ativando os filtros em locais como X, Youtube, conteudo para crianças e etc

### Advanced settings
- Sequencias de passos entre o Top K, o Top P e depois a temperatura

#### Top K
- calibrar quantas possiveis palavras (mais, porém e mais 10) queremos utilizar
- Exemplo: se são 10 e queremos contar somente com 4 palavras, afim de obter um controle maior do que vai ser gerado, é com o Top K que iremos definir qual que é tamanho do conjunto de palavras (prestando atenção que, neste momento o modelo ainda não escolheu qual é a palavra). Uma vez executada, pula para o Top P

#### Top P
- seleção de palavras baseado em probabilidade (palavras conectadas ou seguida de outra.. 10%, 30%, 60% de chance)
- soma máxima que eu quero tolerar
- podemos dizer que o top máximo é de 20%
- escolha de 4 palavras, a soma de todas ela chega em 20% ou inferior a 15% (a primeira palavra tem 15% e a segunda tem 4%, ou seja, 19%.. se a terceira tem 3%, estoura em 22%.. ou seja, de 5 palavras virou 2, chegando na temperatura do modelo)
- se temperatura for 0, ele escolhe a palavra com mais probabilidade (15%)
- se temperatura for 1, escolhe aleatoriamente
- tomar cuidado pq limita o modelo
- somente pessoas mais avançadas pra usar
- utilizar em linguagens especificas (de dominio)
- tomar cuidado na criação de conteudos (estudos)

#### Enviando um audio, ele mostra que existe "tokens", então:
- LLM (modelo de linguagem gigantesco)
- NLP (processamento de linguagem natural)
- modelo de machine learning é um programa de computador
- trabalha com numeros
- transforma um texto em uma forma que o computador entenda (numeros)
- token é um resultado final desse processamento

#### Limpa a pontuação do texto, limpeza dos caracteres, lematização (pegar palavras que entendemos do idioma, portugues, criando formas de representar as palavras com menos caracteres), converter os lemas/representações em forma numerica
- radicais parecidos em portugues
- encurtando para o radical comum
- vira um lema, representação unica

------------------------------------------------------------------------------------------
# AULA 1: MERGULHANDO NO GEMINI, A IA DO GOOGLE
Nesta aula, vamos começar o nosso mergulho conhecendo o Gemini, a IA do Google, e ver como ele consegue criar tabelas, escrever poemas, gerar códigos e muito mais. Além disso, vamos conhecer também o Google AI Studio.

#### Nesta aula, você vai:
- Conhecer o Gemini, a IA do Google;
- Entender o que é a Inteligência Artificial generativa;
- Gerar tabelas, poemas, códigos pelo Gemini;
- Conhecer o Google AI Studio;
- Analisar imagens com o Gemini e o Google AI Studio.

#### Link do projeto base:
- Acesse o Google Gemini aqui: https://gemini.google.com/
- Acesse o Google AI Studio aqui: https://aistudio.google.com/app/prompts/new_chat/?utm_source=website&utm_medium=referral&utm_campaign=Alura&utm_content=
- Acesse o Google API Key aqui: https://aistudio.google.com/app/apikey/?utm_source=website&utm_medium=referral&utm_campaign=Alura&utm_content=
- Faça uma cópia da planilha com as avaliações dos hoteis aqui: https://docs.google.com/spreadsheets/d/1qKUKKI7BNmVFs4rvTkl4YeCEbddRNcCP5_r_-pICk4A/edit?usp=sharing
- Acesse a pasta com as Imagens utilizadas na aula aqui: https://drive.google.com/drive/folders/1w8lfurPj3TakbhAiSiVtbMPji_PU-KNC?usp=sharing
- Acesse os prompts utilizados na aula aqui: https://docs.google.com/document/d/130u8Kd6GewOsuRhoL4vWCENdh9ppDKabFAeUSWvYrlI/edit?usp=sharing

#### Desafios desta aula
Deseja ir além? Experimente estes desafios:
- Use o Gemini ou o Google AI Studio para algo do seu dia a dia no trabalho, visando a automação de alguns processos já realizados por você;
- Pegue o seu histórico do Google Chrome por meio dessa extensão e peça para o Gemini tirar conclusões de como você tem usado o seu tempo, criando um resumo do que você mais acessa, quantidade de uso e tipo de site;
- Faça parte da comunidade gratuita de desenvolvedores e de usuários da Google Cloud Innovators, acesse a plataforma aqui! (https://cloud.google.com/innovators?hl=pt-br)
- Histórico Chrome: https://chromewebstore.google.com/detail/quick-chrome-history-expo/hdfpifhfphhgjipcnfnolgalplokmmge

#### Mergulhe mais profundo
Aprofunde-se nos seguintes tópicos:
- Google Gemini e Imersão Inteligência Artificial | Hipsters Ponto Tech #407 (https://www.hipsters.tech/google-gemini-e-imersao-inteligencia-artificial-hipsters-ponto-tech-407/) 
- O que é o Google Gemini (https://www.alura.com.br/artigos/google-gemini?_gl=1*1tqucwc*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTAyNjgzNS4xOS4wLjE3MTUwMjY4MzUuMC4wLjA.*_fplc*SXQ5NDdCJTJGM0tLblVLd1AxWG80c3lOU3dWdlZOV3VxOHhvMW54TWt0VlUwM095dnJpc3U2TU15MmNZUXlObUlsbHRwcUVpTjNtZ1NQOHJKaVczY3JXekFiZDNyM0M1RGhoQXhFS2R1OG9LOGh3YlFJdUl0SjJDNTc4b2M5S1ElM0QlM0Q.)
- O que é IA generativa? (https://www.alura.com.br/artigos/inteligencia-artificial-ia-generativa-chatgpt-gpt-midjourney?_gl=1*1tqucwc*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTAyNjgzNS4xOS4wLjE3MTUwMjY4MzUuMC4wLjA.*_fplc*SXQ5NDdCJTJGM0tLblVLd1AxWG80c3lOU3dWdlZOV3VxOHhvMW54TWt0VlUwM095dnJpc3U2TU15MmNZUXlObUlsbHRwcUVpTjNtZ1NQOHJKaVczY3JXekFiZDNyM0M1RGhoQXhFS2R1OG9LOGh3YlFJdUl0SjJDNTc4b2M5S1ElM0QlM0Q.)
- Como criar uma Inteligência Artificial? (https://www.alura.com.br/artigos/como-criar-inteligencia-artificial-ia?_gl=1*1tqucwc*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTAyNjgzNS4xOS4wLjE3MTUwMjY4MzUuMC4wLjA.*_fplc*SXQ5NDdCJTJGM0tLblVLd1AxWG80c3lOU3dWdlZOV3VxOHhvMW54TWt0VlUwM095dnJpc3U2TU15MmNZUXlObUlsbHRwcUVpTjNtZ1NQOHJKaVczY3JXekFiZDNyM0M1RGhoQXhFS2R1OG9LOGh3YlFJdUl0SjJDNTc4b2M5S1ElM0QlM0Q.)
- O que é Machine Learning | Hipsters Ponto Tube (https://www.youtube.com/watch?v=Iuz_jc96bQk)

------------------------------------------------------------------------------------------

# AULA 2: MELHORES TÉCNICAS EM ENGENHARIA DE PROMPT
Nesta aula, iremos conhecer as melhores técnicas e práticas de engenharia de prompt por meio do Google AI Studio!

#### Nesta aula, você vai:
- Aprender as melhores técnicas de como realizar um prompt;
- Conhecer o conceito de zero-shot prompting;
- Aprender a técnica de few-shot prompting;
- Conhecer a técnica Few-shot Chain-of-Thought prompting.

#### Links importantes para você acompanhar a aula
- Guia de desing de prompts do Google: https://ai.google.dev/gemini-api/docs/prompting-strategies?hl=pt-br
- Comunidade de Innovators: https://cloud.google.com/innovators?hl=pt-br

#### Desafios desta aula
- Use a técnica de Few-shot Chain-of-Thought para um problema da sua vida real;
- Escolha 10 textos do seu site de notícias preferido. Apresente para o Google AI Studio o padrão dos títulos e das suas respectivas notícias e quando chegar no décimo primeiro texto, apresente somente a notícia e peça para ele gerar um título. Veja se existe alguma técnica ou padrão;
- Faça parte da comunidade gratuita de desenvolvedores e de usuários da Google Cloud Innovators, acesse a plataforma aqui! (https://cloud.google.com/innovators?hl=pt-br)

#### Aprofunde-se nos seguintes tópicos:
- Paper da OpenAI "Language Models are Few-Shot Learners" (https://arxiv.org/abs/2005.14165)
- Paper do Google "Chain-of-Thought Prompting Elicits Reasoning in Large Language Models" (https://arxiv.org/abs/2201.11903)
- Paper do Google "Least-to-Most Prompting Enables Complex Reasoning in Large Language Models" (https://arxiv.org/abs/2205.10625)
- Paper do Google "Self-Consistency Improves Chain of Thought Reasoning in Language Models" (https://arxiv.org/abs/2203.11171)
- Machine Learning no mundo da biometria, Google Gemini e verificação de alucinações Hipsters: Fora de Controle #29 (https://www.alura.com.br/podcast/hipsterstech-machine-learning-no-mundo-da-biometria-google-gemini-e-verificacao-de-alucinacoes-hipsters-fora-de-controle-29-a9140?_gl=1*1d7gx5x*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTA4OTcwMi4yMS4wLjE3MTUwODk3MDIuMC4wLjA.*_fplc*SXo1JTJGclBtU0NqeE5kSzR2MVZBOHdTZHNYTHVpYXp6JTJCYVp1bU5TVFB1YzVHdmRONTNWeUhBQ1IwcUpIQW4yVlNnTGowYnZoUkhvbGIlMkJjUXBEMGxJQTQ1U2FZMTJmb1h4WHBoZWdYJTJCMERQSDNtSmxKQzRqTXRpaGJHdHBlZ3clM0QlM0Q.)
- O que é Engenharia de Prompt e quais as suas principais técnicas? (https://www.alura.com.br/artigos/engenharia-prompt?_gl=1*1d7gx5x*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTA4OTcwMi4yMS4wLjE3MTUwODk3MDIuMC4wLjA.*_fplc*SXo1JTJGclBtU0NqeE5kSzR2MVZBOHdTZHNYTHVpYXp6JTJCYVp1bU5TVFB1YzVHdmRONTNWeUhBQ1IwcUpIQW4yVlNnTGowYnZoUkhvbGIlMkJjUXBEMGxJQTQ1U2FZMTJmb1h4WHBoZWdYJTJCMERQSDNtSmxKQzRqTXRpaGJHdHBlZ3clM0QlM0Q.#principios-para-a-criacao-de-um-prompt)

------------------------------------------------------------------------------------------

# Aula 3: Explorando os parâmetros do Google AI Studio
Nesta aula, vamos ver mais sobre o Google AI Studio e explorar seus parâmetros e configurações até o suporte do modelo multimodal que o Gemini nos dá, iniciando a automação desse modelo com as APIs.

#### Nesta aula, você vai:
- Conhecer os 3 tipos de prompts do Google AI Studio: chat prompts, freeform prompts e structured prompts;
- Explorar os parâmetros do Google AI Studio;
- Conhecer mais sobre os tokens e PLN;
- Iniciar o contato com Python pelo Google Colab.

#### Link do projeto:
- Acesse o Google AI Studio aqui: https://aistudio.google.com/app/prompts/new_chat/?utm_source=website&utm_medium=referral&utm_campaign=Alura&utm_content=
- Acesse o Google API Key aqui: https://aistudio.google.com/app/apikey/?utm_source=website&utm_medium=referral&utm_campaign=Alura&utm_content=
- Acesse o Google Colab aqui: http://colab.research.google.com/
- Acesse os prompts dessa aula aqui: https://docs.google.com/document/d/1HSBfjW8nVnDp3PG9KCLspzkdxlRZDL-YnubpFI369uQ/edit?usp=sharing

#### Links importantes para você acompanhar a aula
- Guia de Mergulho da Imersão IA! (https://grupoalura.notion.site/Imers-o-IA-Guia-de-Mergulho-41ae5fadd8fd47899167a115e96244d9)
- Acesse o Google AI Studio aqui (https://aistudio.google.com/app/prompts/new_chat/?utm_source=website&utm_medium=referral&utm_campaign=Alura&utm_content=)
- Acesse o Google API Key aqui (https://aistudio.google.com/app/apikey/?utm_source=website&utm_medium=referral&utm_campaign=Alura&utm_content=)
- Galeria de prompts do Google AI Studio (https://ai.google.dev/examples?hl=pt-br)
- Vlog do Fabrício Carraro no Japão (https://www.youtube.com/watch?v=dWO-9SyD7yc)
- Guia em PDF de Nara e Kyoto (https://drive.google.com/file/d/1vByLRS3AED7NxrkgLTl2Haay53lylopr/view?usp=sharing)
- Live 08/05 às 18:30 | Masterclass em Python: Prepare-se para criar o seu chatbot (https://youtube.com/live/j_0HRH7gZtA)

#### Desafios desta aula
Deseja ir além? Experimente este desafio:
- Criar seu próprio áudio e realizar um prompt para análise pelo Google AI Studio;
- Pesquise como colocar a imagem do Google AI Studio dentro do código de Pyhton no Google Colab;
- Pegue os códigos que não contenham imagens do AI Studio e exporte para o Google Colab.
- Solução do desafio: Acesse a resolução do desafio dessa aula aqui (https://docs.google.com/document/d/1xDRlgrB2XmFUdoliXqdInmJSTCGIqDRuqkFunbd7x20/edit?usp=sharing)

#### Mergulhe mais profundo
Aprofunde-se nos seguintes tópicos:
- Google I/O, desenvolvimento responsável e modelos multimodais | Hipsters: Fora de Controle #05 (https://www.hipsters.tech/google-i-o-desenvolvimento-responsavel-modelos-multimodais-hipsters-fora-de-controle-05/)
- O que é Machine Learning? (https://www.alura.com.br/artigos/machine-learning?_gl=1*1fwnesh*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTI3MTc0MS4yNy4wLjE3MTUyNzE3NDEuMC4wLjA.*_fplc*RHlUc2tvTWFKWDNiNWRvSndHJTJCUVVjM0hjd2g0U3ZMaExGVGpXZG9mTklKb2pkejVVZFl0SVRjaHlTek9oNW1iN1I3ZnBUJTJGd1R3VE9yeXlLUTJBWVVBZkVMdGtrZlpmZDg3Y29peDc4WEJSY0dRNFZ5MURHcEElMkJYejElMkZEY0ElM0QlM0Q.)
- O que é PLN? (https://www.alura.com.br/artigos/o-que-e-pln?_gl=1*1fwnesh*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTI3MTc0MS4yNy4wLjE3MTUyNzE3NDEuMC4wLjA.*_fplc*RHlUc2tvTWFKWDNiNWRvSndHJTJCUVVjM0hjd2g0U3ZMaExGVGpXZG9mTklKb2pkejVVZFl0SVRjaHlTek9oNW1iN1I3ZnBUJTJGd1R3VE9yeXlLUTJBWVVBZkVMdGtrZlpmZDg3Y29peDc4WEJSY0dRNFZ5MURHcEElMkJYejElMkZEY0ElM0QlM0Q.)
- Guia de Python (https://www.alura.com.br/artigos/python?_gl=1*1fwnesh*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTI3MTc0MS4yNy4wLjE3MTUyNzE3NDEuMC4wLjA.*_fplc*RHlUc2tvTWFKWDNiNWRvSndHJTJCUVVjM0hjd2g0U3ZMaExGVGpXZG9mTklKb2pkejVVZFl0SVRjaHlTek9oNW1iN1I3ZnBUJTJGd1R3VE9yeXlLUTJBWVVBZkVMdGtrZlpmZDg3Y29peDc4WEJSY0dRNFZ5MURHcEElMkJYejElMkZEY0ElM0QlM0Q.)

------------------------------------------------------------------------------------------

# Aula 4: Criando seu próprio chatbot com a Gemini API no Google Colab
Nesta aula, vamos criar um chatbot com a Gemini API pelo Google Colab e descobrir como funciona a premiação de melhores projetos!

#### Nesta aula, você vai:
- Aprender a criar o seu próprio chatbot;
- Saber como funciona a competição de projetos dessa Imersão.
- Fique até o final da aula e tenha orientações exclusivas sobre como usar o GitHub e como colocar seu projeto do Google Colab nele.

#### Link do projeto:
- Acesse o Google Colab aqui: (https://colab.research.google.com/)
- Guia de início rápido na API Gemini: (https://ai.google.dev/gemini-api/docs/quickstart?hl=pt-br)
- Códigos da aula 4 aqui: (https://colab.research.google.com/drive/1wFIctGOaYwlgXD8xsyBiSi5LmTHrObai?usp=sharing)
- Formulário de submissão do seu projeto aqui: (https://forms.gle/xtn8UvC8spvoWEr57)

#### Links importantes para você acompanhar a aula
- Guia de Mergulho da Imersão IA; (https://grupoalura.notion.site/Imers-o-IA-Guia-de-Mergulho-41ae5fadd8fd47899167a115e96244d9)
- Live 08/05: Mergulhe em Python: Prepare-se para criar o seu chatbot; (https://youtube.com/live/j_0HRH7gZtA)
- IA Conference Brasil 2024; (https://iaconferencebrasil.com.br/)
- Faça parte da comunidade gratuita de desenvolvedores e de usuários da Google Cloud Innovators, acesse a plataforma aqui; (https://cloud.google.com/innovators?hl=pt-br)
- Live 13/05 às 18:30 | Projetos que inspiram e próximos desafios. (https://youtube.com/live/0x_WCLhen7Q)

#### Desafios desta aula: Premiação de melhores projetos
Deseja ir além? Envie seu projeto e concorra a prêmios:
- Tutorial: https://youtu.be/bLK66y0CcR8

#### Desenvolva um Projeto Relacionado à Aula 4 e/ou Aula 5 da Imersão IA 2ª Edição
- O projeto deve estar relacionado ao conteúdo da Aula 4 e/ou Aula 5 da Imersão IA 2ª edição, organizada pela Alura em parceria com o Google.
#### Uso Obrigatório da API Key do Google
- É obrigatório o uso da API Key do Google (acesse aqui para obter sua chave https://aistudio.google.com/app/apikey/?utm_source=website&utm_medium=referral&utm_campaign=Alura&utm_content=).
#### Publicação do Projeto no GitHub
- O projeto deve ser publicado no GitHub. Se precisar de ajuda para subir seu projeto, confira o tutorial aqui. (https://www.youtube.com/watch?v=9IiWoiBhWiA)
#### Submissão do Projeto
- A submissão do projeto deve ser feita através deste formulário entre os dias 09/05 e 11/05, até as 23h59. (https://forms.gle/xtn8UvC8spvoWEr57)
#### Publicação e Votação no Discord
- O projeto será publicado no Servidor do Discord da Imersão IA 2024 para votação pela comunidade até 11/05, às 23h59.
- A votação acontece no canal "#Votação". Dê estrelas no projeto que você mais gostou e conecte-se com outras pessoas para incentivá-las a votar no seu projeto.

#### Mergulhe mais profundo
Aprofunde-se nos seguintes tópicos:
- Guia de Python (https://www.alura.com.br/artigos/python?_gl=1*1cb4vv9*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTI3Mzg0MS4yOC4wLjE3MTUyNzM4NDEuMC4wLjA.*_fplc*RHlUc2tvTWFKWDNiNWRvSndHJTJCUVVjM0hjd2g0U3ZMaExGVGpXZG9mTklKb2pkejVVZFl0SVRjaHlTek9oNW1iN1I3ZnBUJTJGd1R3VE9yeXlLUTJBWVVBZkVMdGtrZlpmZDg3Y29peDc4WEJSY0dRNFZ5MURHcEElMkJYejElMkZEY0ElM0QlM0Q.)
- O que é API (https://www.alura.com.br/artigos/api?_gl=1*1cb4vv9*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTI3Mzg0MS4yOC4wLjE3MTUyNzM4NDEuMC4wLjA.*_fplc*RHlUc2tvTWFKWDNiNWRvSndHJTJCUVVjM0hjd2g0U3ZMaExGVGpXZG9mTklKb2pkejVVZFl0SVRjaHlTek9oNW1iN1I3ZnBUJTJGd1R3VE9yeXlLUTJBWVVBZkVMdGtrZlpmZDg3Y29peDc4WEJSY0dRNFZ5MURHcEElMkJYejElMkZEY0ElM0QlM0Q.)
- O que é Markdown (https://www.alura.com.br/artigos/como-trabalhar-com-markdown?_gl=1*1uxdzob*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTI3Mzg0MS4yOC4wLjE3MTUyNzM4NDEuMC4wLjA.*_fplc*RHlUc2tvTWFKWDNiNWRvSndHJTJCUVVjM0hjd2g0U3ZMaExGVGpXZG9mTklKb2pkejVVZFl0SVRjaHlTek9oNW1iN1I3ZnBUJTJGd1R3VE9yeXlLUTJBWVVBZkVMdGtrZlpmZDg3Y29peDc4WEJSY0dRNFZ5MURHcEElMkJYejElMkZEY0ElM0QlM0Q.#:~:text=O%20que%20%C3%A9%20Markdown%3F,mais%20complexas%2C%20como%20o%20HTML.)

------------------------------------------------------------------------------------------

# Aula 5: Criando um sistema para busca em documentos usando embeddings e a Gemini API
Nesta última aula, vamos criar um sistema de buscas semânticas por meio de embeddings e do Google API.

#### Nesta aula, você vai:
- Fazer uma LLM (Large Language Model) para acessar documentos;
- Criar um embedding pelo Google Colab.

#### Link do projeto:
- Acesse o Google Colab aqui: (https://colab.research.google.com/)
- Gemini API: Embeddings Quickstart (https://colab.research.google.com/github/google-gemini/cookbook/blob/main/quickstarts/Embeddings.ipynb)
- Código da Aula 05 aqui: (https://colab.research.google.com/drive/1Dags_xXdnmps_4Shbm8bH7m8VRjxp3t5?usp=sharing)

#### Links importantes para você acompanhar a aula
- Guia de Mergulho da Imersão IA! (https://grupoalura.notion.site/Imers-o-IA-Guia-de-Mergulho-41ae5fadd8fd47899167a115e96244d9)
- Guia de Embeddings: https://ai.google.dev/gemini-api/docs/embeddings?hl=pt-br
- Task Types (Tipos de Tarefas): https://ai.google.dev/gemini-api/tutorials/document_search?hl=pt-br#api_changes_to_embeddings_with_model_embedding-001

#### Aprofunde-se nos seguintes tópicos:
- O que é PLN? (https://www.alura.com.br/artigos/o-que-e-pln?_gl=1*1ssswlx*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTM3MzgwMy4zMi4xLjE3MTUzNzM4MDcuMC4wLjA.*_fplc*R2FGVnVMQU9mYnVwSDY3dHB1MXJnMHZ1UkRXR0FWdWhqdm9OMmRaZDh3bThWYTRrZW1hU2R0cFRwQzBUNHUzWUZPTVAxNjB1ZGNwTXNDbGJVRTRuMGFYUm5ZRndYeERURU5hckhsZHNSTCUyQmtWTlZMUDVCQkc2OFQ0VThuR2clM0QlM0Q.)
- O que é Deep Learning? (https://www.alura.com.br/artigos/deep-learning-deep-fake?_gl=1*1ssswlx*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTM3MzgwMy4zMi4xLjE3MTUzNzM4MDcuMC4wLjA.*_fplc*R2FGVnVMQU9mYnVwSDY3dHB1MXJnMHZ1UkRXR0FWdWhqdm9OMmRaZDh3bThWYTRrZW1hU2R0cFRwQzBUNHUzWUZPTVAxNjB1ZGNwTXNDbGJVRTRuMGFYUm5ZRndYeERURU5hckhsZHNSTCUyQmtWTlZMUDVCQkc2OFQ0VThuR2clM0QlM0Q.)
- Conheça mais sobre Numpy (https://www.alura.com.br/artigos/numpy-computacao-cientifica-com-python?_gl=1*1ssswlx*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTM3MzgwMy4zMi4xLjE3MTUzNzM4MDcuMC4wLjA.*_fplc*R2FGVnVMQU9mYnVwSDY3dHB1MXJnMHZ1UkRXR0FWdWhqdm9OMmRaZDh3bThWYTRrZW1hU2R0cFRwQzBUNHUzWUZPTVAxNjB1ZGNwTXNDbGJVRTRuMGFYUm5ZRndYeERURU5hckhsZHNSTCUyQmtWTlZMUDVCQkc2OFQ0VThuR2clM0QlM0Q.) 
- O que é o Python Pandas? (https://www.alura.com.br/artigos/pandas-o-que-e-para-que-serve-como-instalar?_gl=1*1ssswlx*_ga*MTUyMzg4NTg5My4xNzEwMjQ1MTcz*_ga_1EPWSW3PCS*MTcxNTM3MzgwMy4zMi4xLjE3MTUzNzM4MDcuMC4wLjA.*_fplc*R2FGVnVMQU9mYnVwSDY3dHB1MXJnMHZ1UkRXR0FWdWhqdm9OMmRaZDh3bThWYTRrZW1hU2R0cFRwQzBUNHUzWUZPTVAxNjB1ZGNwTXNDbGJVRTRuMGFYUm5ZRndYeERURU5hckhsZHNSTCUyQmtWTlZMUDVCQkc2OFQ0VThuR2clM0QlM0Q.)

------------------------------------------------------------------------------------------
