# Loteria LOTOFÁCIL em Java

Este é um projeto de implementação da loteria LOTOFÁCIL em Java. O sistema é capaz de gerar jogos aleatórios, permitir que os jogadores façam suas apostas, verificar os resultados e calcular prêmios de acordo com as regras da loteria. Este sistema funciona por meio do terminal, lendo e escrevendo dados.

## Regras de negócio/requisitos:

### Menu LOTOFÁCIL:

O sistema apresenta um menu interativo para o usuário realizar suas apostas. Enquanto o usuário não digitar 0 para sair, novas apostas serão permitidas.

### Regras para a aposta de 0 a 100:

- Utilizando a biblioteca `Scanner`, o usuário deve digitar um número inteiro de 0 a 100 via teclado. Caso o número seja maior que 100 ou menor que 0, uma mensagem de "Aposta inválida." é exibida.
- Utiliza-se a biblioteca `Random` para sortear aleatoriamente um número de 0 a 100.
- Compara-se o número escolhido pelo usuário com o número sorteado pelo sistema.
  - Se o usuário acertar a aposta, imprime-se "Você ganhou R$ 1.000,00 reais.". Caso contrário, imprime-se "Que pena! O número sorteado foi: X.".

### Regras para a aposta de A à Z:

- Utiliza-se o método `System.in.read()` para ler um caractere de A à Z via teclado, podendo ser lido como maiúsculo ou minúsculo. Caso não seja uma letra, exibe-se a mensagem "Aposta inválida.". Utiliza-se o método `Character.isLetter()` para verificar se a entrada digitada é uma letra válida.
- Converte-se a entrada do usuário para maiúsculo utilizando `Character.toUpperCase()`.
- Escolhe-se uma letra inicial para ser a letra premiada.
- Compara-se a letra lida com a letra premiada.
  - Se o usuário acertar a aposta, imprime-se "Você ganhou R$ 500,00 reais.". Caso contrário, imprime-se "Que pena! A letra sorteada foi: X.".

### Regras para a aposta de número par ou ímpar:

- Utiliza-se o `Scanner` para ler um número inteiro via teclado.
- Utiliza-se o operador de módulo (%) para verificar se o número é par ou ímpar.
  - Se o resto da divisão do número por 2 for 0, o número é par.
- Se o número digitado for par, imprime-se "Você ganhou R$ 100,00 reais.". Caso contrário, imprime-se "Que pena! O número digitado é ímpar e a premiação foi para números pares.".

## Vídeo do Projeto

Veja uma demonstração do projeto em ação:

[![Assista ao vídeo](https://github.com/lucas-novaesm/lotofacil-java-interface-grafica/assets/122632100/564ffd1f-1a35-44b3-8fdf-07c61b81cb7d)

## Como rodar o projeto

1. Certifique-se de ter o JDK (Java Development Kit) instalado em sua máquina.
2. Clone este repositório.
3. Navegue até o diretório do projeto.
4. Compile o código-fonte.
5. Execute o programa.
6. Siga as instruções exibidas no terminal para fazer suas apostas na LOTOFÁCIL.
7. Divirta-se!

Este projeto foi desenvolvido utilizando a versão do JDK 8 e não requer bibliotecas externas além das fornecidas pelo próprio Java.
