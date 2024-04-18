# FrequenciaDePalavras
 
Este é um programa em C# que conta a frequência das palavras em uma frase inserida pelo usuário.

1. **Declarações de Uso (`using`)**:
   - Importa os namespaces `System` e `System.Collections.Generic`, necessários para utilizar as classes do .NET Framework.

2. **Classe `Program`**:
   - Contém o método `Main()`, que é o ponto de entrada do programa.

3. **Método `Main()`**:
   - Solicita ao usuário que digite uma frase.
   - Lê a entrada do usuário.
   - Chama o método `ContarFrequenciaPalavras(input)` para contar a frequência das palavras na frase inserida.
   - Imprime a frequência das palavras na tela.

4. **Método `ContarFrequenciaPalavras(string input)`**:
   - Recebe uma string `input` como parâmetro.
   - Divide a frase em palavras usando o método `Split()` e armazena em um array de strings.
   - Inicializa um dicionário chamado `frequencia` para armazenar a frequência das palavras. O comparador `StringComparer.OrdinalIgnoreCase` é utilizado para ignorar diferenças de maiúsculas e minúsculas ao comparar as chaves do dicionário.
   - Itera sobre cada palavra no array de palavras.
   - Se a palavra já existe no dicionário, incrementa sua contagem.
   - Se a palavra não existe no dicionário, adiciona-a ao dicionário com uma contagem inicial de 1.
   - Retorna o dicionário contendo a frequência das palavras.

5. **Impressão de Resultados**:
   - No método `Main()`, cada palavra e sua frequência são impressas na tela usando um loop `foreach`.

