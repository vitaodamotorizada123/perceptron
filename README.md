1. Conceito

O Perceptron é um modelo de rede neural artificial criado na década de 1950 por Frank Rosenblatt. Ele foi o primeiro algoritmo capaz de aprender a partir de dados de forma supervisionada. Em termos simples, é como uma “unidade de decisão” que recebe entradas (valores), multiplica cada uma por um peso, soma tudo, aplica uma função de ativação e decide se a saída será 0 ou 1.
Sua importância histórica é enorme porque foi a base inicial para o desenvolvimento das redes neurais e abriu caminho para a Inteligência Artificial moderna, mesmo que tivesse limitações.

2. Funcionamento

O Perceptron é chamado de classificador linear porque ele só consegue separar os dados em duas classes usando uma linha (no caso de duas dimensões), ou um hiperplano (em dimensões maiores).
Isso significa que ele só funciona bem quando os dados são linearmente separáveis.
Por exemplo: se eu quiser separar pontos vermelhos de pontos azuis em um gráfico, e existe uma linha reta que divide bem os dois grupos, o Perceptron consegue resolver.
A limitação é que ele não consegue lidar com problemas mais complexos, como o clássico caso do XOR, em que os dados não podem ser separados por uma linha reta.

3. Código

Ao analisar o código de treinamento do Perceptron, as principais etapas são:

Inicialização dos pesos e do bias (geralmente valores pequenos ou zerados).

Entrada dos dados de treino (features e rótulos esperados).

Cálculo da saída predita multiplicando entradas × pesos + bias.

Função de ativação para decidir a classe (0 ou 1).

Atualização dos pesos com base no erro (diferença entre predição e valor real). Isso é feito até o modelo aprender a separar corretamente os dados ou até atingir um número máximo de épocas.

4. Aplicação prática

Um exemplo real seria o filtro de spam em e-mails.
O Perceptron pode ser usado para classificar se um e-mail é “spam” ou “não spam” com base em palavras-chave, frequência de termos e outras características simples.
A justificativa é que, mesmo sendo um modelo básico, ele pode aprender padrões lineares claros (por exemplo, presença de “promoção”, “clique aqui”, “grátis”) e já oferecer uma solução eficiente sem precisar de modelos complexos.


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

(README)
Funções
perceptron_input(inputs, weights, bias)
Calcula a entrada do perceptron.
Parâmetros:
inputs: Lista de valores de entrada.
weights: Lista de pesos correspondentes às entradas.
bias: Valor do bias.
Retorno: A soma ponderada das entradas mais o bias.
perceptron_output(inputs, weights, bias)
Calcula a saída do perceptron.
Parâmetros:
inputs: Lista de valores de entrada.
weights: Lista de pesos correspondentes às entradas.
bias: Valor do bias.
Retorno: 1 se a entrada do perceptron for maior ou igual a 0, caso contrário, 0.
Execução
Para executar o código, basta rodar o arquivo principal:
python main.py
(^^^^^^^^)

Perceptron em Python

Este projeto implementa um Perceptron simples, o modelo de rede neural mais básico, em Python.
O Perceptron realiza um somatório ponderado dos valores de entrada com seus respectivos pesos, adiciona um viés (bias) e aplica uma função de ativação do tipo degrau.

📌 Estrutura do Código
perceptron_input(inputs, weights, bias)

Calcula o somatório ponderado das entradas:

resultado

resultado=∑(entrada×peso)+bias
perceptron_output(inputs, weights, bias)

Aplica a função de ativação:

Retorna 1 se o valor do somatório for maior ou igual a 0.

Retorna 0 caso contrário.

main()

Exibe mensagens no console.

Calcula e mostra o resultado do perceptron.

▶️ Como Executar

Clone este repositório ou copie o código para um arquivo perceptron.py.

Execute no terminal:

python perceptron.py

📊 Exemplo de Saída

Com as entradas [1, 2, 3], pesos [0.1, 0.2, 0.3] e viés 0.4, a saída será:

Hello, World!
This is the main file.
The result of the perceptron input is:  1.8


Se você usar a função perceptron_output, o resultado será:

1
