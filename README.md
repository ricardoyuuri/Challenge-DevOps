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

















