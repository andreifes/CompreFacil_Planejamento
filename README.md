# TRABALHO DE PI: CompreFácil
Trabalho desenvolvido durante a disciplina de Projeto Integrador

## Sumário

### 1.COMPONENTES<br>
André Neves Alves: andrenevesalves99@gmail.com<br>
Diogo Lucca Chaves Araújo: diogolucca06@gmail.com<br>
João Matheus Siller Pessanha: universitariodoano@gmail.com<br>


### 2.MINIMUNDO - Para versão final<br>
>Fazer compras em supermercados de forma virtual se mostra muito eficiente em momentos como o que estamos atualmente, em quarentena. Porém, muitos Apps(aplicativos) não se mostram práticos e agradáveis de serem usados, além de que, como cada supermercado possui seu próprio sistema, o usuário precisa realizar todo o processo de cadastro todas vez que usar um App novo. E também, por mais que os muitos Apps sejam parecidos em alguns pontos, cada um possui uma interface, funcionalidades e dinâmica com os usuários diferentes. Pensando nisso, o CompreFácil, App de delivery para supermercados, trará uma interface simples, prática e intuitiva, fazendo com que a forma de comprar seja bem mais agradável. A interface será padronizada, sendo assim, independente de qual supermercado for escolhido, um usuário só precisa se familiarizar com o processo de uma compra e isso não muda para comprar em outro local. O sistema será capaz de comparar preços dos produtos entre os supermercados. Por exemplo: se o usuário procurar por uma Coca-Cola 1L, ele poderá selecionar uma opção que mostra os resultados para todos os supermercados e ordenar por preço, para ver qual tem o produto mais barato. Só é possível ter os produtos de um mesmo local em uma compra, então para isso, o usuário deve entrar no supermercado que deseja, preencher o carrinho com os produtos que escolher e depois é só escolher a forma de pagamento e endereço, caso não queira pegar a compra no local. O usuário poderá fazer seu login com dados pessoais e cadastrar diversos endereços para recebimento do pedido, além de ter uma carteira, onde pode adicionar cartões de crédito e dinheiro via boleto. Ele terá a opção de pagar online, durante a entrega ou no local, dependendo de como quer receber a compra. Todos os produtos devem ter informações bem detalhadas e ilustrações precisas, para que o usuário saíba bem do que está comprando. O sistema também terá registros de todas as compras feitas, como se fossem notas fiscais, onde são mostrados os produtos, valores, quantidades, forma de pagamento, entre outras informações.


### 3.RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS) - Para versão inicial<br>
![Arquivo PDF do Protótipo Balsamiq feito para o CompreFácil](https://raw.githubusercontent.com/andreifes/CompreFacil_Planejamento/main/Arquivos/Wireframes_Inicial.pdf")

#### 3.1 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO? - Para versão inicial<br>
* Relatório com a quantidade total de produtos vendidos pelo supermercado, incluindo as seguintes informações: nome do supermercado e quantidade total de produtos vendidos.
* Relatório dos supermercados de uma cidade, incluindo as seguintes informações: nome da cidade e nomes dos supermercados.
* Relatório com os produtos de um supermercado, incluindo as seguintes informações: nome do supermercado, nomes dos produtos e preço.
* Relatório que informe os produtos de uma categoria, incluindo as seguintes informações: nome da categoria e nomes dos produtos.
* Relatório com as formas de pagamento e quantidade utilizadas no supermercado, incluindo as seguintes informações: nome do supermercado, forma de pagamentos e quantidades.


### 4.TABELA DE DADOS DO SISTEMA - Para versão inicial<br>


### 5.PMC - Para versão final<br>
![Aquivo PNG do PMC feito para o protótipo CompreFácil](https://github.com/andreifes/CompreFacil_Planejamento/raw/main/Arquivos/IMGS/PMC_Final.PNG)


### 6.MODELO CONCEITUAL - Para versão inicial<br>    
![Aquivo PNG do Modelo Conceitual feito para o protótipo CompreFácil](https://github.com/andreifes/CompreFacil_Planejamento/raw/main/Arquivos/IMGS/Conceitual_Inicial.PNG)

#### 6.1 Descrição dos dados - Para versão inicial<br> 
  USUARIO: tabela que armazena as informações relativas ao usuário<br>
   >ID: campo que armazena o identificador do usuário<br>
   NOME: campo que armazena o nome do usuário<br>
   EMAIL: campo que armazena o e-mail do usuário<br>
   TELEFONE: campo que armazena o telefone do usuário<br>
   SENHA: campo que armazena a senha do usuário<br>

  ENDERECO: tabela que armazena as informações relativas a endereço do mercado<br>
   ID: campo que armazena o identificador do endereço<br>
   CIDADE: campo que armazena a cidade referente ao endereço<br>
   BAIRRO: campo que armazena o bairro referente ao endereço<br>

  CATEGORIA: tabela que armazena as informações relativas a categoria do produto<br>
   ID: campo que armazena o identificador da categoria<br>
   NOME: campo que armazena o nome das possíveis categorias de um produto<br>

  FORMA_PGTO: tabela que armazena as informações relativas a opção de forma de pagamento da uma compra<br>
   ID: campo que armazena o identificador da forma de pagamento<br>
   NOME: campo que armazena o nome da forma de pagamento<br>

  MERCADO: tabela que armazena as informações relativas ao mercado<br>
   ID: campo que armazena o identificador do mercado<br>
   NOME: campo que armazena o nome do mercado<br>
   IMG: campo que armazena a imagem(base64) do mercado<br>
   ID_ENDERECO: campo que armazena o identificador do endereço do mercado<br>

  PRODUTO: tabela que armazena as informações relativas ao produto<br>
   ID: campo que armazena o identificador do mercado<br>
   NOME: campo que armazena o nome do produto<br>
   IMG: campo que armazena a imagem(base64) do produto<br>
   ID_CATEGORIA: campo que armazena o identificador da categoria do produto<br>

  COMPRA: tabela que armazena as informações relativas a compra feita por um usuário<br>
   ID: campo que armazena o identificador da compra realizada pelo usuário<br>
   DATA_HORA: campo que armazena a data e hora da compra<br>
   STTS_PGTO: campo que armazena a confirmação ou não de pagamento da compra<br>
   ID_USUARIO: campo que armazena o identificador do usuário que realizou a compra<br>
   ID_FORMA_PGTO: campo que armazena o identificador da forma de pagamento utilizada<br> 

  ITEM: tabela que armazena as informações relativas aos items dos mercados<br>
   ID: campo que armazena o identificador do item<br>
   ID_MERCADO: campo que armazena o identificador do mercado <br>
   ID_PRODUTO: campo que armazena o identificador do produto contido no item<br>
   PRECO: campo que armazena o preco do produto<br>

  COMPRA_ITEM: tabela que armazena as informações relativas a compra dos itens de um mercado<br>
   ID_COMPRA: campo que armazena o identificador da compra que contém os itens<br>
   ID_ITEM: campo que armazena o identificador do item<br>
   QUANTIDADE: campo que armazena a quantidade do item<br>


### 7.MODELO LÓGICO - Para versão inicial<br>
![Aquivo PNG do Modelo Lógico feito para o protótipo CompreFácil](https://github.com/andreifes/CompreFacil_Planejamento/raw/main/Arquivos/IMGS/Logico_Inicial.PNG)


### 8.MODELO FÍSICO - Para versão inicial<br>
```sql
CREATE TABLE USUARIO (
    ID INT PRIMARY KEY,
    nome VARCHAR(255),
    email VARCHAR(255),
    telefone VARCHAR(30),
    senha VARCHAR(30)
);

CREATE TABLE ENDERECO (
    ID INT PRIMARY KEY,
    cidade VARCHAR(255),
    bairro VARCHAR(255)
);

CREATE TABLE CATEGORIA (
    ID INT PRIMARY KEY,
    nome VARCHAR(255)
);

CREATE TABLE FORMA_PGTO (
    ID INT PRIMARY KEY,
    nome VARCHAR(255)
);

CREATE TABLE MERCADO (
    ID INT PRIMARY KEY,
    nome VARCHAR(255),
    img TEXT,
    ID_endereco INT
);

CREATE TABLE PRODUTO (
    ID INT PRIMARY KEY,
    nome VARCHAR(255),
    img TEXT,
    ID_categoria INT
);

CREATE TABLE COMPRA (
    ID INT PRIMARY KEY,
    data_hora TIMESTAMP,
    stts_pgto BOOLEAN,
    ID_usuario INT,
    ID_forma_pgto INT
);

CREATE TABLE ITEM (
    ID INT PRIMARY KEY,
    preco MONEY,
    ID_mercado INT,
    ID_produto INT
);

CREATE TABLE COMPRA_ITEM (
    ID_item INT,
    ID_compra INT,
    quantidade INT
);
 
ALTER TABLE MERCADO ADD CONSTRAINT FK_MERCADO_2
    FOREIGN KEY (ID_endereco)
    REFERENCES ENDERECO (ID)
    ON DELETE RESTRICT;
 
ALTER TABLE COMPRA ADD CONSTRAINT FK_COMPRA_2
    FOREIGN KEY (ID_usuario)
    REFERENCES USUARIO (ID)
    ON DELETE CASCADE;
 
ALTER TABLE COMPRA ADD CONSTRAINT FK_COMPRA_3
    FOREIGN KEY (ID_forma_pgto)
    REFERENCES FORMA_PGTO (ID)
    ON DELETE CASCADE;
 
ALTER TABLE PRODUTO ADD CONSTRAINT FK_PRODUTO_2
    FOREIGN KEY (ID_categoria)
    REFERENCES CATEGORIA (ID)
    ON DELETE CASCADE;
 
ALTER TABLE ITEM ADD CONSTRAINT FK_ITEM_2
    FOREIGN KEY (ID_mercado)
    REFERENCES MERCADO (ID)
    ON DELETE RESTRICT;
 
ALTER TABLE ITEM ADD CONSTRAINT FK_ITEM_3
    FOREIGN KEY (ID_produto)
    REFERENCES PRODUTO (ID)
    ON DELETE RESTRICT;
 
ALTER TABLE COMPRA_ITEM ADD CONSTRAINT FK_COMPRA_ITEM_1
    FOREIGN KEY (ID_item)
    REFERENCES ITEM (ID)
    ON DELETE RESTRICT;
 
ALTER TABLE COMPRA_ITEM ADD CONSTRAINT FK_COMPRA_ITEM_2
    FOREIGN KEY (ID_compra)
    REFERENCES COMPRA (ID)
    ON DELETE SET NULL;
```


### 9.INSERT APLICADO NAS TABELAS DO BANCO DE DADOS - Para versão inicial<br>


### 10.TABELAS E PRINCIPAIS CONSULTAS - Para versão inicial<br>

#### 10.1 CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS - Para versão inicial<br>

#### 10.2 PRINCIPAIS CONSULTAS DO SISTEMA - Para versão inicial<br>

### 11.PERSONAS - Para versão final<br>
### 11.HISTÓRIA DE USUÁRIOS - Para versão final<br>
