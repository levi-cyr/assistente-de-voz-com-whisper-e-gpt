# Conversando por voz com o ChatGPT utilizando Whisper (OpenAI) e python

Este projeto é uma demonstração da DIO pelo Google Colab. Você pode acessar o código-fonte original clicando [aqui.](https://colab.research.google.com/drive/1rHGq5N-sbEGtZsNUiQFT8q60BhRbj99b?usp=sharing) 

## Como começar

Com o código-fonte aberto, você pode estar copiando ele para seu próprio workspace.

![alt text](/Assets/1.png)
Em "arquivos" selecione a opção "Salvar uma cópia no Drive".

![alt text](/Assets/2.png)

O código original está comentado e, com um pouco de pesquisa, você consegue entender o que ele faz, mesmo sendo mais avançado. Podemos utilizar IA para nos explicar a funcionalidade, ver em sites como StackOverflow e afins para dúvidas específicas. Que tal darmos uma modificada para que ele detecte nossa fala e só pare de gravar quando o usuário parar de falar?

## Como funcionam os novos parâmetros?

Basicamente, precisamos criar uma "sensibilidade" de detecção do áudio, que você configura o quão sensível será o microfone. O programa vai ter o tempo de silêncio, que após um certo tempo (1,5 segundos no caso do código) sem detectar áudio, ele para a gravação e continua o programa.

| Parâmetro | Padrão | Descrição |
| :--- | :--- | :--- |
| **silenceThreshold** | 0.01 | **Sensibilidade:** Define o volume mínimo para ser considerado "fala". Se o ambiente for barulhento, aumente este valor. |
| **silenceDuration** | 1500 | **Tempo de Espera:** Quanto tempo de silêncio (em milissegundos) deve passar antes de encerrar a gravação. |

Clique [aqui](https://colab.research.google.com/drive/1xR2bJP9YN2henRdN9IPQUbycgNFI2O1_?usp=sharing) para acessar o projeto atualizado. 
- **Atenção:** Infelizmente, a API do ChatGPT é paga, então será preciso pagar para realizar os testes. 
