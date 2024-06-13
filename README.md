Módulo FizzBuzz em Elixir

Visão Geral:

Esse módulo em Elixir, FizzBuzz, lê um arquivo que contém uma lista de números, processa cada um desses valores, e aplica a lógica do FizzBuzz.

Funções

build/1

Lê e processa o conteúdo do arquivo especificado.

elixir

Copiar código

FizzBuzz.build("numeros.txt")

handle_file_read/1

Lida com os resultados da leitura do arquivo usando pattern matching.

Sucesso: Divide o conteúdo por vírgulas, converte para inteiros e avalia.

Erro: Retorna uma mensagem de erro.

convert_and_evaluate_numbers/1

Converte uma string em um inteiro e avalia usando a lógica FizzBuzz.

evaluate_numbers/1

Aplica as regras do FizzBuzz:

:fizzbuzz para múltiplos de 3 e 5

:fizz para múltiplos de 3

:buzz para múltiplos de 5

Caso contrário, retorna o número
Uso

Crie um arquivo (ex.: numeros.txt) com números separados por vírgulas.


Chame FizzBuzz.build("numeros.txt").

Retorna {:ok, resultado} com os valores processados ou {:error, razão} em caso de erro.




