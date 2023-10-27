# Teste de PSI 1 - Turno 1 - Versão 1

## Informação do aluno

    Nome: Edson Fernando Cachoeira Filho

Teste termina às 10:45.

Escreve as respostas dentro dos blocos correspondentes.
Substitui as reticências pelo que é pedido em cada pergunta.
Não desformates o documento.

### P1. Indica o que é impresso pelo seguinte código. Justifica a tua resposta

    int i = 5 / 2;
    
    Console.WriteLine($"*\t{i}");

P1 - Resposta

    É impresso um asterisco e o resultado da divisão realizada que é o numero dois, tendo um espaçamento entre eles.
    Isso acontece por que o $ ali coloca exatamente da forma que esta o código dentro do WriteLine;

### P2. Considera o seguinte código com um *bug*

    string s = "2.5";
    int i = Convert.ToInt32(s);

    Console.WriteLine(i);

### Indica uma possível correção para que o código não apresente erros. Explica porque foi necessário fazer essa correção

P2 - Resposta

       string s = "2.5";
        double i = Convert.ToDouble(s);
        Console.WriteLine(i);
        
       Converter a variavel para double. Foi necessario por que a variavel esta armazenando um valor que não é do tipo int assim precisando de uma conversão para um tipo que suporte o valor que ali esta.

### P3. Escreve um programa que solicite ao utilizador dois números inteiros e apresente a sua soma. Caso o resultado seja um número divisível por 3, deve também ser impressa a mensagem "Múltiplo de 3!"

P3 - Resposta
    
        Console.Write("Digite o primeiro número inteiro: ");
        int nmr1 = Convert.ToInt32(Console.ReadLine());

        Console.Write("Digite o segundo número inteiro: ");
        int nmr2 = Convert.ToInt32(Console.ReadLine());
        
        int soma = nmr1 + nmr2;
        
        if (soma % 3 == 0)
        {
            Console.WriteLine($"A soma {soma} é um múltiplo de 3!");
        }
        else
        {
            Console.WriteLine($"A soma {soma} não é um múltiplo de 3.");
        }

### P4. Tens um repositório git criado localmente, onde estás no ramo 'master'. Queres associá-lo ao repositório remoto contido no url 'https://github.com/PSI/OMeuRepositorioRemoto'. Queres também alterar o nome do ramo atual para 'main'. Deverás enviar os *commits* já feitos localmente para o repositório remoto. Indica os comandos necessários

P4 - Resposta

    git remote add origin https://github.com/PSI/OMeuRepositorioRemoto
    git branch -m master main
    git push -u origin main
