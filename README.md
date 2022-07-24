# Explicações e links

Repost de: https://github.com/dznwtf/Bot-de-vendas

Repostei com algumas informações para ajudar pessoas que precisam de ajuda para ligar o bot

# Requisitos

- Conta do Mercado Pago para pegar "accessToken" ([**Mercado Pago Developers**](https://mercadopago.com/developers)) **É NECESSÁRIO TER MERCADO PAGO**
- Token do bot discord ([**Token Bot**](https://discord.com/developers)) **É NECESSÁRIO TER**
- MongoDB zerada ([**MongoDB**](https://mongodb.com)) **É NECESSÁRIO TER**
- Saber um pouco de Java Script para entender os erros :) (Se não entende, também não precisa se importar)
- Se quiser alguma ajuda sobre o bot ou alugar, Meu discord: **[Mac☯#1230](https://discordapp.com/users/705013153800650814)**
--------------------------------------------------------------------------------------
# Tutorial

### Primeiramente:
- BAIXE O BOT, [dznwtf](https://github.com/dznwtf/Bot-de-vendas)

### Mercado Pago:
- Mercado Pago (A forma de pagamento usado no bot) **NÃO TEM OUTRA FORMA DE PAGAMENTO**
- Caso você tenha +18 e não tem conta no mercado pago, entre aqui > [**Mercado Pago**](https://mercadopago.com/) < e faça seu cadastro e espere pela analise da sua conta
- Ou faça que nem a maioria dos brasileiros, peça a alguém pra emprestar a conta do mercado pago ¯\\\_(ツ)\_/¯

Agora, caso você ja tenha conta, abra o [**Mercado Pago Developers**](https://mercadopago.com/developers/panel) e crie sua aplicação.

- Vá ao "Credenciais de produção"
- Copie o AccessToken 
- coloque no **config.json** onde está **"accessToken": "..."**

### Token do bot:
- Logue com sua conta do discord no web, aperte em [**Token Bot**](https://discord.com/developers)
- Crie o seu bot apertando em "BOT" no canto esquerdo da tela e "add bot"... colocando nome e tals
- Aperte em **Reset Token**
- Copie o token e cole onde está "token": "..."

### Prefixo do bot:
- Vai da sua preferencia, mas não deixe vazio ou não coloque apenas um espaço

### MongoDB:
- Registre em [MongoDB](https://www.mongodb.com/cloud/atlas/register) **First Name e Last Name pode ser qualquer coisa, mas email e senha NÃO PODE SER TEMPORARIO**
- Aperte em "Create" no "Shared", desce a barrinha do navegador lá pra baixo e se você quiser trocar o nome do Cluster, que não vai diferenciar nada na configuração do bot 
- Aperte em Create para finalizar
- Aperte faça uma conta da database, seu usuário e senha e no final coloque **0.0.0.0/0**
```yml 
OBSERVAÇÃO:
 (Isso fará que todos vão poder usar sua db, caso a pessoa saiba do username e senha e o link *Recomendado para Hosts)
```
- ou [**seu.ip.publico.aqui**](https://meuip.com/)/32 adicione o ip
- Aperte em connect, Connect MongoDB Compass (Se quiser baixar o programa, pode baixar)
- Copie o link e cole
```js 
"mongo_url": "mongodb+srv://..."
```

### Parte da mensagem do bot> (IMPORTANTE LER COM ATENÇÃO)
- Cor que irá ficar na barrinha lateral da embed em hex:  [HEX](https://htmlcolorcodes.com/color-picker/)
```js 
"color": "..."
```
- Link de uma imagem qualquer (Opcional, pode deixar vazio)
```js 
"author": ""
```
- Titulo da mensagem que ficara como nome (que no caso é a sua loja)
```js 
"nome": "..."
``` 
- O nome miudo na mensagem (pode colocar qualquer coisa, só não coloque vazio)
```js 
"footer": "..."
``` 

### Pegar o id do discord
- Seu ID do discord, caso não consiga pegar seu id, use um bot usando o comando "userinfo" ou vá no configurações do seu discord > "Avançado" > Modo de desenvolvedor e ative
- Botão direito do mouse em algum lugar do seu nome onde estiver mostrando(Sem ser lá no bagui de copiar seu nome) ou aperte na foto pelo celular e aperte em "Copiar ID"
```js 
"owner": "..."
``` 

### Canais do discord
- Id da categoria onde vão ficar as compras
```js 
"categoria": "..."
```  
- Id do Canal de log das compras, pode ser um canal publico que geral pode ver e não falar ou pode ser só pra moderação
```js 
"logs": "..."
```  

# Pronto, você acabou de configurar o seu bot!

