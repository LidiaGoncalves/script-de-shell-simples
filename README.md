# script-de-shell-simples
Como criar scripts de shell simples no Linux
Os scripts de shell desempenham um papel enorme na automação de tarefas repetitivas que, de outra forma, seriam tediosas executando linha por linha.

Neste tutorial, destacamos algumas das operações básicas de script de shell que todo usuário do Linux deve ter.

1. Crie um script de shell simples
Um script de shell é um arquivo que contém texto ASCII . Começaremos criando um shell script simples e, para isso, usaremos um editor de texto. Há um grande número de editores de texto , tanto de linha de comando quanto baseados em GUI. Para este guia, usaremos o editor vim .

Começaremos criando um script simples que exibe “ Hello world ” quando executado.

![image](https://user-images.githubusercontent.com/113737343/192147405-679c12f1-7fae-4a5b-8a3c-b06b8c69141e.png)

Cole o seguinte conteúdo no arquivo e salve.

![image](https://user-images.githubusercontent.com/113737343/192147476-fcea4614-68e2-4e1c-b0fc-644fda802f5e.png)

Vamos examinar o script de shell linha por linha.

A primeira linha – #!/bin/bash– é conhecida como cabeçalho shebang. Esta é uma construção especial que indica qual programa será usado para interpretar o script. Neste caso, este será o shell bash indicado por /bin/bash . Existem outras linguagens de script, como Python , que é indicada por #!/usr/bin/python3e Perl , cujo cabeçalho shebang é indicado por #!/usr/bin/perl.
A segunda linha é um comentário. Um comentário é uma instrução que descreve o que um script de shell faz e não é executado quando o script é executado. Os comentários são sempre precedidos pelo sinal de hash #.
A última linha é o comando que imprime a mensagem ' Hello World ' no terminal.
A próxima etapa é tornar o script executável atribuindo permissão de execução usando o comando chmod conforme mostrado.

![image](https://user-images.githubusercontent.com/113737343/192147508-b69e55f7-3ccc-4631-8b37-0cdf669a03fc.png)

Por fim, execute o script de shell usando um dos comandos:

![image](https://user-images.githubusercontent.com/113737343/192147541-c4708d27-9c8f-4faf-8844-7f67967158ca.png)

![image](https://user-images.githubusercontent.com/113737343/192147571-8d37a394-9790-4972-875f-2b5d05f59fbf.png)

2. Usando Instruções Condicionais para Executar Código
Como outras linguagens de programação, instruções condicionais são usadas em scripts bash para tomar decisões, com apenas uma pequena variação na sintaxe. Vamos cobrir as instruções condicionais if , if-else e elif .

Exemplo de uma instrução if somente
A instrução if pode ser usada para testar condições únicas ou múltiplas. Começaremos com o uso fundamental da instrução if para testar uma única condição. A instrução if é definida pelos if ... fiblocos.

![image](https://user-images.githubusercontent.com/113737343/192147667-d3780ed1-da7e-46c5-989f-6549c02ef818.png)

Vamos dar uma olhada no script de shell abaixo.

![image](https://user-images.githubusercontent.com/113737343/192147688-e16dfc60-9d0c-4c22-98e3-5055326c9006.png)

O script de shell acima solicita que o usuário forneça uma pontuação que é então armazenada em uma variável x . Se a pontuação corresponder a 70 , o script retornará a saída “ Bom trabalho! ”. O operador de comparação ==é utilizado para testar se a pontuação inserida, que está armazenada na variável x , é equivalente a 100 .

![image](https://user-images.githubusercontent.com/113737343/192147713-be28ace6-ac33-4fec-8ef0-49097d609505.png)

Outros operadores de comparação que você pode usar incluem:

-eq- Igual a
-ne– Não igual a
-lt- Menor que
-le- Menos que ou igual a
-lt- Menor que
-ge- Melhor que ou igual a
Por exemplo, o bloco de instrução if abaixo imprime ' Work Harder ' se a pontuação de entrada for qualquer valor menor que 50 .

![image](https://user-images.githubusercontent.com/113737343/192147755-1cf95575-debd-48b0-8857-5396a66f72b8.png)

![image](https://user-images.githubusercontent.com/113737343/192147773-6b19b25d-969e-4734-919c-c1fa316f1a5e.png)


Exemplo de uma instrução if-else
Para situações em que você tem 2 resultados possíveis: – seja isso ou aquilo – a instrução if-else é útil.
![image](https://user-images.githubusercontent.com/113737343/192147814-28346182-60bb-4ec0-930f-4d5e22176beb.png)

O script abaixo lê a pontuação de entrada e verifica se é maior ou igual a 70 .

Se a pontuação for maior ou igual a 70 , você recebe um ' Ótimo trabalho, você passou! ' mensagem. No entanto, se a pontuação cair abaixo de 70 , a saída ' Você falhou ' será impressa.
![image](https://user-images.githubusercontent.com/113737343/192147861-97971da3-7844-48ee-bcd7-2c86da954e64.png)

![image](https://user-images.githubusercontent.com/113737343/192147896-a838e955-fa56-4d5a-8127-07a2614df03b.png)

Exemplo de uma instrução if-elif-else
Em cenários em que há várias condições e resultados diferentes, a instrução if-elif-else é usada. Esta declaração tem o seguinte formato.

![image](https://user-images.githubusercontent.com/113737343/192147918-4fe45f12-d648-4fde-bddb-aaf441442c2c.png)

Por exemplo, temos um script para uma loteria que verifica se o número digitado é 90 , 60 ou 30 .

![image](https://user-images.githubusercontent.com/113737343/192147963-16e93723-7a48-4c96-8449-ef318230e594.png)

![image](https://user-images.githubusercontent.com/113737343/192147987-75591741-9ef8-48d4-a449-e6308134bbe7.png)



