# DevPleno2020
Exercícios de Contratação do Desenvolvedor Pleno - Março/2020

<h2> Exercício #1 - C# </h1>
Crie um aplicativo que leia o arquivo ‘input.csv’ providenciado
Calcule a média aritmética de idade por estado
Monte um JSON com os resultados de acordo com o exemplo
Envie o JSON criado via POST para o endpoint: https://zeit-endpoint.brmaeji.now.sh/api/avg

Por exemplo:

conteúdo do arquivo exemplo:

Pedro, 15, Rio de Janeiro
Joana, 33, Rio de Janeiro
Alair, 24, Atibaia
Tobias, 35, Atibaia
Marina, 44, Campinas

Médias:

Rio de Janeiro, 24
Atibaia, 29,5
Campinas, 44

JSON:

{
 "medias":
      [
   	{
 	    "cidade" : "Rio de Janeiro",
 	    "idade" : 24
 		
 	},
 	{
                "cidade" : "Atibaia",
 	    "idade" : 29.5
 	},
 	{
                "cidade" : "Campinas",
 	    "idade" : 44
 	}
      ]
}

IMPORTANTE: 
a) Dados manuais digitados por usuários podem ter erro de digitação. Considere que “São Paulo” é igual a “Sao Paulo”.
b) O sistema de destino trabalha com um máximo de duas casas decimais. Se o valor for, por exemplo, 30.333333… , envie o valor arredondado de 30.33 .

Crie um repositório numa conta pessoal do github e compartilhe-a com o entrevistador.

<h2> Exercício #2 - NodeJS / Angular </h1>

Faça um pequeno serviço contendo duas partes:

BackEnd em NodeJS
FrontEnd em Angular (versão à sua escolha)

O FrontEnd deverá:

Conter uma form com um input, um label e um botão
O texto deverá ser “Qual o nome do principal produto da Sysplan?”
o botao “enviar” deve fazer um POST autenticado (basica) para o endpoint providenciado e exibir a resposta em tela

O BackEnd deverá:

1a) Servir interface web composta de um index.html e um arquivo .js com a aplicação em Angular.
1b) Gravar em um arquivo “tentativas.log”, local, o timestamp em formato “YYYY-MM-DD hh:mm:ss - TENTATIVA - RESULTADO” de cada tentativa de adivinhação. Ex.:

2020-03-20 14:35:22 - Sucrilhos - false
2020-03-20 14:38:34 - Guaraná - false
2020-03-20 14:41:55 - Bolacha Maizena - true

endpoint: https://zeit-endpoint.brmaeji.now.sh/api/auth
credenciais: candidato / entrevista

Formato da msg JSON:

{
   "nome" : "Paulo",
   "mensagem" : "Bolacha Maizena"
}


Crie um repositório numa conta pessoal do github e compartilhe-a com o entrevistador.

<h1> Exercício #3 </h1>

Faça o download do código localizado nesse repositório na pasta "exercicio3". 

Faça o build do projeto e execute a dll criada via prompt de comando, usando o CLI do dotnet:

dotnet MinhaDll.dll

acesse pelo seu browser o endereço http://localhost:5000

A página exibida contém uma lista dinâmica contendo 5 de nomes de filmes. Remova o item 3 e envie. Você verá no log de execução da sua DLL que somente os itens 1 e 2 foram enviados.

Corrija o programa de forma todos os 4 elementos restantes sejam enviados
Ao editar o nome de qualquer filme, você perceberá que o seu campo será iluminado com uma cor verde.. Se você adicionar um elemento novo nessa lista usando o botão “Novo”, esse novo item não tem o efeito de iluminação esperado. Corrija esse novo problema.

Ao ter o código corrigido, crie um repositório numa conta sua do github e compartilhe-a com o entrevistador.

