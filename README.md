# ProjetoExtensao

# SOFTWARE DE GESTÂO DE PREZOS

## Índice
1. [Descrição do projeto](#Descrição_projeto)
2. [Tecnologias usadas](#Tecnologias)
3. [requisitos funcionais](#Funcionalidades)
4. [Imagens](#imagens_projeto)
5. [Instalação para uso](#Instalação-uso)
6. [Instalação para modificação](#instalação-codigo-fonte)

## Descrição
O aplicativo foi desenvolvido por estudantes universitários de cursos relacionados à Tecnologia da Informação (TI), e visa facilitar a administração e o controle de pedidos para um microempreendedor individual (MEI).

	1- Centralização de Pedidos
Consolidar todos os pedidos em um único lugar, independentemente da plataforma de venda (iFood, WhatsApp, etc.), 
para facilitar o gerenciamento e a visualização.
	2- Ordenação de Pedidos por Data de Entrega
	3- organização de tarefas menores
o aplicativo tem uma funcionalidade para anotar pequenas tarefas menores que devem ser feitas durante a semana como preparar embalagens, comprar ingredientes, fazer publicidade
	4- Geração de Estatísticas e Relatórios
Produzir relatórios financeiros detalhados, incluindo receitas, custos e lucros, proporcionando uma visão clara das finanças, também a possibilidade de ver o volume de vendas mensais


## Tecnologias
Todas os programas e bibliotecas que usamos eram de livre uso
Para o software:
1. java
2. javafx (biblioteca para interfaces graficas)
    2.1 scenebuilder (aplicativo para usar o javafx com drag and drop)
3. postgresql 
    modelagem do banco site -> Brmodelo
4. modelagem de clases site -> lucid.app

Para documentação e comunicação:
1. whatsapp (comunicacao)
2. Onedrive - Word
3. Google drive
4. Trello



## funcionalidades
1. Cadastro de pedidos (feito) 
2. Visualização dos pedidos (feito) 
3. Mostrar os pedidos em ordem de entrega (LISTA DE PEDIDOS) (feito) 
4. Pesquisa sobre os pedidos abertos por CPF, NOME ou DATA ENTREGA (PESQUISA DOS PEDIDOS) (feito) 
5. Estatísticas da empresa filtrada por tempo (dia, semana, mês...) (feito) 
    5.1 Receita (feito) 
    5.2 Custo operacional (feito) 
    5.3 Lucro (feito) 
    5.4 Quantidade de pedidos (feito) 
    5.5 Impressão das estatísticas (feito) 
    5.6 Salvar os dados ou enviar por Email (não feito devido à complexidade e pq seria a única coisa do programa que precisaria de conexão com a internet) 
6. Histórico dos pedidos (feito) 
7. Pesquisa no histórico dos pedidos por CPF, NOME ou DATA ENTREGA (PESQUISA DOS PEDIDOS) (feito) 
8. Task list da semana basicamente um espaço para poder anotar tarefas pequenas a serem feitas na semana (feito) 
9. Notificação sobre os pedidos (também envolveria a internet e é simples ver os pedidos que estão chegando perto do prazo) 
10. forma de imprimir um resumo do pedido (removido, pois a cliente não precisa e não tem impressora) 

## imagens_projeto
menu onde mostar a tabela de pedidos em cima e em baixo a parte de anotaçoes ![alt text](image-1.png)
pedido aberto é a mesma janela da ciraçao de pedido  ![alt text](image-2.png)
financeiro é onde fica o histórico de pedidos e por onde é possivel gerar o relatório em excel ![alt text](image-3.png)





## Instalação-uso
Para instalar o aplicativo:

1. Baixe a pasta "instalacao" do repositório do github:
    link: https://github.com/Thiago-Weiss/Projeto-Extensao

2. configurar o banco de dados
    2.1 na pasta "install" instale o postgresql e na senha dele coloque: 2015
    2.2 crie um novo banco de dados com o nome de: confeitariaBD
    2.1 use o arquivo "banco_dados.sql" criar as estruturas de pasta do banco

3. instale o java
    3.1 na pasta de "install" instale o jdk-21

4. instalar o app
    4.1 copie a pasta "App" para onde vc quiser que o aplicativo fique no seu computador
    4.2 para abrir o app é só clicar no iniciar.bat
    4.3 se quiser colocar o icon ![alt text](image.png) do brigadeiro na pasta do progama
        4.3 botão direito na pasta "App" -> propriedades -> personalizar -> alterar ícone -> selecione o icone (ele está dentro da pasta "bibliotecas")




## Instalação-codigo-fonte
1. baixe a pasta "codigo-fonte" do repositório do github
    link: https://github.com/Thiago-Weiss/Projeto-Extensao
    
2. configure o seu ambiente de desenvolvimento (vs-code)
	1- instale o vs-code
	2- instale a instencao do java no vs code
	3- crie uma pasta para o projeto e coloque a pasta "src" dentro
	4- importe as 3 bibliotecas pro vs code -> javafx, jxlr e as dos postgre (server)
	5- rode o arquivo "MainStart" para ele criar uma pasta rais no projeto
	6- no arquivo launch.json dentro da pasta .vscode que ele acabou de criar adicione mais um argumento no projeto que ele criou
		coloque o diretorio da biblioteca javafx no argumento
		"vmArgs": "--module-path \"S:/java_gui/javafx-sdk-17.0.10/lib\" --add-modules javafx.controls,javafx.fxml" 
		
	7- instale o postgresql e use o arquivo "banco_dados.sql" para cirar o banco de dados
	8- no arquivo "MainStart" atualize os dados de conexao com o banco de dados
