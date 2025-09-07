Conceito
O Perceptron é um modelo de neurônio artificial criado por Frank Rosenblatt em 1958.
Recebe entradas, multiplica por pesos, soma e aplica uma função de ativação para gerar saída.
Importância histórica: foi o primeiro modelo de rede neural artificial, marcando o início do aprendizado de máquina e da Inteligência Artificial moderna.
Funcionamento,
É um classificador linear, ou seja, separa classes usando uma reta, plano ou hiperplano.
Limitação: não consegue resolver problemas não linearmente separáveis, como o XOR.
Código (etapas do treinamento),
Inicialização dos pesos e bias.
Cálculo da saída (soma ponderada + ativação).
Comparação com a saída esperada (erro).
Ajuste dos pesos e bias com base no erro.
Repetição até atingir número de épocas ou erro mínimo.
Aplicaçao prática,
Exemplo: filtro de spam simples em e-mails.
Justificativa: separa mensagens em spam e não spam com base em palavras-chave, sendo rápido e eficiente para problemas linearmente separáveis.

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
