# Target Customer

## Descritivo da solução
A solução encontrada pelos desenvolvedores foi a criação de uma empresa
(TargetCustomer), no qual irá disponibilizar um serviço de consultoria para classificar um
público alvo de uma empresa contratante. Sendo assim a solução partiu do átomo da
problemática, os dados, portanto primeiro fomos atrás de conjuntos de dados interessantes de
serem trabalhados, sendo encontrado um específico envolvendo perfil de consumidores de
vinho (apenas nossa base inicial para o projeto, vinho não tem relação com nossa solução). A
partir desse conjunto de dados trabalharemos e analisaremos esse conjunto para chegar na
resposta da seguinte pergunta: “Qual o perfil de consumidor deste produto?”. Chegando nesta
resposta, podemos auxiliar da melhor maneira empresas parceiras que tipo de pessoas
consomem seus produtos, para assim sabermos qual a melhor maneira de entregar propagandas,
promoções, de adaptar seus produtos, de lançar produtos novos e etc. Então nossa solução
resumidamente trabalha com análise de personalidade do cliente, assim fazendo as melhores
recomendações para as empresas darem o segundo passo ao lidar com seus consumidores!

## Passo a passo de como criar o WebApp e realizar o deploy!!!

## Passo 1

### Clonar o repositório e abrir a pasta no VSCode

![image](https://github.com/user-attachments/assets/3fcefd52-3326-4f84-8416-8a46445c06cc)

Neste passo nós clonamos o codigo da nossa aplicação .NET e abrimos no Visual Studio Code! Porém para isto nós precisamos instalar duas extenções C#!

![Screenshot 2024-09-16 202737](https://github.com/user-attachments/assets/7ae1aece-9502-4e05-893b-d9c3cddf9902)

## Passo 2

## Começar a criação do WebApp pelo VSCode 

Vamos precisar baixar duas extenções da Azure!!!

![Screenshot 2024-09-16 203650](https://github.com/user-attachments/assets/abc481bc-d8ec-4157-8059-c7afe13089b7)

![Screenshot 2024-09-16 203714](https://github.com/user-attachments/assets/8a1cac2f-d4ba-4a05-a54c-4ae3c7aa3152)

Após isso realizamos o login com a nossa conta da azure! E ja vamos iniciar o processo de deploy da nossa aplicação .NET em um serviço de aplicativo da azure!!! 

Neste primeiro passo nós clicamos com o botão direito em cima do "AppService" e selecionamos o "Create New Web App (Advanced)"

![Screenshot 2024-09-16 202337](https://github.com/user-attachments/assets/28cd09b2-28ae-4f75-8c6a-f1cb48c9a825)

Agora vamos definir um nome para o nosso WebApp!!!

![Screenshot 2024-09-16 204144](https://github.com/user-attachments/assets/1320f967-7a73-4169-b0ab-e75430d73961)

Logo após isso, iremos realizar a criação de um novo grupo de recursos e definir um nome!!!

![Screenshot 2024-09-16 204248](https://github.com/user-attachments/assets/6c4ae400-a85d-4e74-bf17-64aac5c1c450)

No próximo passo iremos escolher qual será a linguagem da nossa runtime!!! Que no nosso caso é a .NET 8!!!

![Screenshot 2024-09-16 204443](https://github.com/user-attachments/assets/fc94064a-0f1c-4f0e-b66f-627e2241fd9b)

O próximo passo é selecionar o sistema operacional!!! Que no nosso caso é o linux!!!

![Screenshot 2024-09-16 204953](https://github.com/user-attachments/assets/dd23b22f-2c54-4406-b36e-4e644687d905)

Neste passo nós selecionamos o East Us por padrão!!!

![Screenshot 2024-09-16 205213](https://github.com/user-attachments/assets/cc703080-6b7e-420f-84c1-e71c18d79610)

Logo após, nós criamos um novo plano de serviço de aplicativo!!!

![Screenshot 2024-09-16 205316](https://github.com/user-attachments/assets/445c1ce3-118c-4491-bd96-37f97f03e155)

No próximo passo nós selecionamos o plano F1, pois o mesmo é gratuito e faz com que o nosso WebApp tenha um baixo custo!!!

![Screenshot 2024-09-16 205439](https://github.com/user-attachments/assets/2f57f1e4-d5e6-4c6f-ba8b-858242ba122e)

Na parte de App Insights nós iremos dar "skip for now"

![image](https://github.com/user-attachments/assets/b9570bad-b47b-4fcd-93a8-ce7e3d0632c0)

Após isso, irá aparecer um terminal mostrando a criação do nosso WebApp, e assim que finalizar irá aparecer uma mensagem no canto inferior esquerdo perguntando se você deseja realizar o deploy, nesta parte voce clica em "deploy" e iremos selecionar a pasta da nossa aplicação para o deploy!!!

![Screenshot 2024-09-16 205925](https://github.com/user-attachments/assets/4d7a8c9d-20c6-4007-9c67-06fef9acea7c)

Nesta parte clicamos em "AddConfig"

![Screenshot 2024-09-16 210928](https://github.com/user-attachments/assets/d7079921-6633-4e8a-8c60-18cbdf494ee0)

Após isso, irá iniciar o processo de deploy da nossa aplicação, que pode levar alguns minutos! Após o deploy ser finalizado, irá aparecer uma mensagem no canto inferior esquerdo perguntando se deseja abrir a aplicação em um browser, você confirma!!!

![Screenshot 2024-09-16 211058](https://github.com/user-attachments/assets/faaf3890-ba06-4348-9cbc-419f4a0b4d98)

Com isso o nosso navegador será aberto e de cara irá nos mostrar isso!!!

![Screenshot 2024-09-16 211353](https://github.com/user-attachments/assets/300001dc-b96b-4d82-bcdb-bae2b34b544a)

Porém basta adicionar na URL "/swagger/index.html", que o swagger da nossa aplicação será exibido!!!

![Screenshot 2024-09-16 211547](https://github.com/user-attachments/assets/d24582d3-b56c-48f9-974b-122142784fe8)

## Passo 3

### Testar todos os endpoints das duas tabelas que estão no swagger!!!

Primeiro realize o POST e aperte em execute!

![Screenshot 2024-09-16 221938](https://github.com/user-attachments/assets/42b113c8-b630-41aa-a534-360cf98a181a)

Depois realize o GET e aperte em execute! Este metodo retorna todos os clientes cadastrados no banco de dados!

![Screenshot 2024-09-16 222259](https://github.com/user-attachments/assets/d6d970ac-f3d8-4915-b0fe-0ce9d2647884)

Depois realize o GET pelo id e aperte em execute! Este metodo irá retornar o cliente em que voce esta procurando pelo ID!

![Screenshot 2024-09-16 222532](https://github.com/user-attachments/assets/2b015022-3562-430c-82ac-81f7b34b3874)

![Screenshot 2024-09-16 222653](https://github.com/user-attachments/assets/957e68f4-29d0-4fe6-a3f2-1168667d9211)

Depois realize o UPDATE e aperte em execute! Insira o id do cliente em que deseja atualizar algum dado e altere!

![Screenshot 2024-09-16 223024](https://github.com/user-attachments/assets/4f5e650f-136e-4371-aa75-d517782185c3)

![Screenshot 2024-09-16 225148](https://github.com/user-attachments/assets/0186105f-37f4-4490-9b0d-d47c2fd406c7)

Realize o GET novamente para ver a alteração ou veja pelo banco de dados!!!

O acesso do banco de dados da aplicação esta no arquivo "appsettings.json"

![Screenshot 2024-09-16 224943](https://github.com/user-attachments/assets/9cb7a113-595f-40fd-b2c7-09b439dac2a5)

E por fim vamos realizar o DELETE pelo ID!

![Screenshot 2024-09-16 225515](https://github.com/user-attachments/assets/26903859-4e02-495b-b832-7ca725bd08b6)

![Screenshot 2024-09-16 225537](https://github.com/user-attachments/assets/91806011-cb8c-4600-9e78-4dd5b5d48ee1)

## Agora é so testar todos os endpoints da tabela consultoria e ver a persistencia dos dados no banco!!!

## Scripts JSON do CRUD

# Tabela Cliente

### GET

Retorna todos os clientes salvos no banco de dados

### POST 

Cole o JSON e altere os dados, menos o ID, pois é gerado automaticamente!

```
{
  "clienteId": 0,
  "cnpj": "string",
  "nome": "string",
  "logradouro": "string",
  "ramodeAtuacao": "string",
  "email": "string",
  "senha": 0
}
```

### GET pelo ID 

Somente retorna o ID digitado

### PUT

Digite o ID e altere o dado!

```
{
  "clienteId": 0,
  "cnpj": "string",
  "nome": "string",
  "logradouro": "string",
  "ramodeAtuacao": "string",
  "email": "string",
  "senha": 0
}
```

### DELETE

Soemente o numero do ID

# Tabela consultoria 

### GET 

Retorna todos as consultorias salvas no banco de dados

### POST 

Cole o JSON e altere os dados, menos o ID, pois é gerado automaticamente!

```
{
  "consultoriaId": 0,
  "nomeConsultoria": "string"
}
```

### GET pelo ID

Somente retorna o ID digitado

### PUT

Digite o ID e altere o dado!

```
{
  "consultoriaId": 0,
  "nomeConsultoria": "string"
}
```

### DELETE

Soemente o numero do ID

# No final o serviço de WebApp ficará assim na azure!!!

![Screenshot 2024-09-16 232906](https://github.com/user-attachments/assets/abef7613-7612-4296-b440-8be1367fe6fc)

# Agora vamos criar o banco SQL da Azure na nuvem 

Para isso crie um novo recurso e selecione "SQL Database"!

![Screenshot 2024-09-16 233126](https://github.com/user-attachments/assets/ec3e7000-2d29-46de-a80f-3635725a5edb)

Selecione o mesmo grupo de recurso que criamos para o WebApp e defina um nome para o seu banco de dados na nuvem!!

![Screenshot 2024-09-16 233322](https://github.com/user-attachments/assets/dd8cdd00-0ee1-4593-ba3e-764fb454049a)

Após isso crie um novo servidor e defina um nome e selecione EastUs ou EastUS 2 

![Screenshot 2024-09-16 233451](https://github.com/user-attachments/assets/59417f07-7bf4-4a0b-a954-fa8ee286296a)

Habilite a autenticação SQL e defina um logon e uma senha! No nosso o caso o logon é "adm-sqldb-targetcustomer" e a senha "Fiap@2tds2024"!!!

![Screenshot 2024-09-16 233612](https://github.com/user-attachments/assets/0c5be04f-5530-47a2-a671-7e0711584afb)

Em computação + armazenamento selecione o plano básico!!!

![Screenshot 2024-09-16 233830](https://github.com/user-attachments/assets/9f49757c-1b66-466a-b72d-3db720885342)

Em rede selecione o "ponto de extremidade público" e nas regras de firewall deixe tudo como "sim"!!!

![Screenshot 2024-09-16 234030](https://github.com/user-attachments/assets/dc780e76-ebfb-49c3-8d23-26e3c4a6e8f6)

Após isso clique em "Criar" e espere a implantação!!!

![Screenshot 2024-09-16 234245](https://github.com/user-attachments/assets/f28a74f7-98be-449d-b8d3-0118a622cb14)

Assim que criado clique em "Ir para o recurso" e depois em "Editor de consultas" nas opções da lateral esquerda!!!

![image](https://github.com/user-attachments/assets/b93e6e45-3600-4d01-8381-cc9187b5e7a8)

Irá aparecer uma tela de acesso ao banco de dados!!! Coloque o logon e a senha que definimos!!!

![Screenshot 2024-09-16 234523](https://github.com/user-attachments/assets/313355a3-debb-48e7-88fc-1277b1e871fc)

Irá ser exebida uma tela onde iremos colocar o nosso script!!!

![Screenshot 2024-09-16 234631](https://github.com/user-attachments/assets/1a02a3d4-254a-47c7-96f3-5a70d5e0af3f)

```
--Criação da tabela com o drop
DROP TABLE T_TC_CADASTRO;
CREATE TABLE T_TC_CADASTRO(
  id_cadastro NUMERIC NOT NULL,
  nr_cnpj NUMERIC(14) NOT NULL,
  varchar_senha VARCHAR(60) NOT NULL,
  nm_razaosocial VARCHAR(80) NOT NULL,
  CONSTRAINT T_TC_CADASTRO_PK PRIMARY KEY (id_cadastro)
);
 
--CRUD
 
--Create
INSERT INTO T_TC_CADASTRO (id_cadastro, nr_cnpj, varchar_senha, nm_razaosocial) VALUES (1, 12345678901234, 'senha123', 'Empresa Exemplo LTDA');
INSERT INTO T_TC_CADASTRO (id_cadastro, nr_cnpj, varchar_senha, nm_razaosocial) VALUES (2, 23456789012345, 'senha234', 'Empresa Exemplo LTDB');
INSERT INTO T_TC_CADASTRO (id_cadastro, nr_cnpj, varchar_senha, nm_razaosocial) VALUES (3, 34567890123456, 'senha345', 'Empresa Exemplo LTDC');
INSERT INTO T_TC_CADASTRO (id_cadastro, nr_cnpj, varchar_senha, nm_razaosocial) VALUES (4, 45678901234567, 'senha456', 'Empresa Exemplo LTDD');
INSERT INTO T_TC_CADASTRO (id_cadastro, nr_cnpj, varchar_senha, nm_razaosocial) VALUES (5, 56789012345678, 'senha567', 'Empresa Exemplo LTDE');
 
--Read
SELECT * FROM T_TC_CADASTRO;
 
--Read pelo id
SELECT * FROM T_TC_CADASTRO
WHERE id_cadastro = 1;
 
SELECT * FROM T_TC_CADASTRO
WHERE id_cadastro = 2;
 
SELECT * FROM T_TC_CADASTRO
WHERE id_cadastro = 3;
 
SELECT * FROM T_TC_CADASTRO
WHERE id_cadastro = 4;
 
SELECT * FROM T_TC_CADASTRO
WHERE id_cadastro = 5;
 
--Read pelo cnpj
SELECT * FROM T_TC_CADASTRO
WHERE nr_cnpj = 56789012345678;
 
--Update no nome da razão social
UPDATE T_TC_CADASTRO
SET nm_razaosocial = 'Empresa Exemplo Atualizada LTDA'
WHERE id_cadastro = 1;
 
UPDATE T_TC_CADASTRO
SET nm_razaosocial = 'Empresa Exemplo Atualizada LTDB'
WHERE id_cadastro = 2;
 
UPDATE T_TC_CADASTRO
SET nm_razaosocial = 'Empresa Exemplo Atualizada LTDC'
WHERE id_cadastro = 3;
 
UPDATE T_TC_CADASTRO
SET nm_razaosocial = 'Empresa Exemplo Atualizada LTDD'
WHERE id_cadastro = 4;
 
UPDATE T_TC_CADASTRO
SET nm_razaosocial = 'Empresa Exemplo Atualizada LTDE'
WHERE id_cadastro = 5;
 
--Update de senha 
UPDATE T_TC_CADASTRO
SET varchar_senha = 'bananinha123'
WHERE id_cadastro = 5;
 
--Delete pelo id
DELETE FROM T_TC_CADASTRO
WHERE id_cadastro = 1;
 
DELETE FROM T_TC_CADASTRO
WHERE id_cadastro = 2;
 
DELETE FROM T_TC_CADASTRO
WHERE id_cadastro = 3;
 
DELETE FROM T_TC_CADASTRO
WHERE id_cadastro = 4;
 
DELETE FROM T_TC_CADASTRO
WHERE id_cadastro = 5;
 
--Delete pelo cnpj
DELETE FROM T_TC_CADASTRO
WHERE nr_cnpj = 56789012345678;
 
--Criação da tabela relacionada com drop
DROP TABLE T_TC_CONSULTA;
CREATE TABLE T_TC_CONSULTA(
  id_consulta NUMERIC NOT NULL,
  ds_consulta VARCHAR(80) NOT NULL,
  dt_consulta DATE NOT NULL,
  blob_csv_arquivo VARBINARY(MAX) NOT NULL,
  id_cadastro NUMERIC NOT NULL,
  CONSTRAINT T_TC_CONSULTA_PK PRIMARY KEY (id_consulta),
  CONSTRAINT T_TC_CADASTRO_CONSULTA_FK FOREIGN KEY (id_cadastro) REFERENCES T_TC_CADASTRO(id_cadastro)
);
 
--CRUD
 
--Create
INSERT INTO T_TC_CONSULTA (id_consulta, ds_consulta, dt_consulta, blob_csv_arquivo, id_cadastro) VALUES (1, 'Consulta sobre impostos', '2002-10-12', CAST(0x48656C6C6F AS VARBINARY(MAX)), 1);
INSERT INTO T_TC_CONSULTA (id_consulta, ds_consulta, dt_consulta, blob_csv_arquivo, id_cadastro) VALUES (2, 'Consulta sobre exportação', '2002-11-05', CAST(0x56656E646173 AS VARBINARY(MAX)), 2);
INSERT INTO T_TC_CONSULTA (id_consulta, ds_consulta, dt_consulta, blob_csv_arquivo, id_cadastro) VALUES (3, 'Consulta sobre importação', '2002-09-22', CAST(0x4573746F717565 AS VARBINARY(MAX)), 3);
INSERT INTO T_TC_CONSULTA (id_consulta, ds_consulta, dt_consulta, blob_csv_arquivo, id_cadastro) VALUES (4, 'Consulta sobre regulamentação', '2002-03-07', CAST(0x466F726E656 AS VARBINARY(MAX)), 4);
INSERT INTO T_TC_CONSULTA (id_consulta, ds_consulta, dt_consulta, blob_csv_arquivo, id_cadastro) VALUES (5, 'Consulta sobre inovação', '2002-02-15', CAST(0x46696E616 AS VARBINARY(MAX)), 5);
 
--Read
SELECT * FROM T_TC_CONSULTA;
 
--Read pelo id 
SELECT * FROM T_TC_CONSULTA
WHERE id_consulta = 1;
 
SELECT * FROM T_TC_CONSULTA
WHERE id_consulta = 2;
 
SELECT * FROM T_TC_CONSULTA
WHERE id_consulta = 3;
 
SELECT * FROM T_TC_CONSULTA
WHERE id_consulta = 4;
 
SELECT * FROM T_TC_CONSULTA
WHERE id_consulta = 5;
 
--Read pela data da consulta
SELECT * FROM T_TC_CONSULTA
WHERE dt_consulta = '2002-10-12';
 
--Update da descrição da consulta
UPDATE T_TC_CONSULTA
SET ds_consulta = 'Consulta sobre impostos atualizada'
WHERE id_consulta = 1;
 
UPDATE T_TC_CONSULTA
SET ds_consulta = 'Consulta sobre exportação atualizada'
WHERE id_consulta = 2;
 
UPDATE T_TC_CONSULTA
SET ds_consulta = 'Consulta sobre importação atualizada'
WHERE id_consulta = 3;
 
UPDATE T_TC_CONSULTA
SET ds_consulta = 'Consulta sobre regulamentação atualizada'
WHERE id_consulta = 4;
 
UPDATE T_TC_CONSULTA
SET ds_consulta = 'Consulta sobre inovação atualizada'
WHERE id_consulta = 5;
 
--Update da data da consulta
UPDATE T_TC_CONSULTA
SET dt_consulta = '2000-10-12'
WHERE id_consulta = 5;
 
--Delete pelo id
DELETE FROM T_TC_CONSULTA
WHERE id_consulta = 1;
 
DELETE FROM T_TC_CONSULTA
WHERE id_consulta = 2;
 
DELETE FROM T_TC_CONSULTA
WHERE id_consulta = 3;
 
DELETE FROM T_TC_CONSULTA
WHERE id_consulta = 4;
 
DELETE FROM T_TC_CONSULTA
WHERE id_consulta = 5;
 
--Delete pela data da consulta
DELETE FROM T_TC_CONSULTA
WHERE dt_consulta = '2000-10-12';
```

# Cole o script no console e realize a criação das tabelas (uma de cada vez) e os seus devidos CRUDS (um de cada vez)

## Após realizar as tabelas e seus devidos cruds, podemos ver que as tabelas foram criadas, na parte de tabelas na lateral esquerda do console!!!

![Screenshot 2024-09-16 235315](https://github.com/user-attachments/assets/c706b19e-05fb-4d85-baf7-8e960d746b41)

# Por fim podemos ver a criação do banco de dados dentro do grupo de recursos!!!

![Screenshot 2024-09-16 235457](https://github.com/user-attachments/assets/aa0130a9-09a8-4956-8485-881e12ebe4c2)











































