# Desafio da semana #4

```js
/*
Declare uma variável chamada `isTruthy`, e atribua a ela uma função que recebe
um único parâmetro como argumento. Essa função deve retornar `true` se o
equivalente booleano para o valor passado no argumento for `true`, ou `false`
para o contrário.
*/
var isTruty = function(a){
return !! a
};

// Invoque a função criada acima, passando todos os tipos de valores `falsy`.
isTruty("");
//false
isTruty('');
//false
isTruty(0);
//false
isTruty(-0);
//false
isTruty(undefined);
//false
isTruty(null);
//false
isTruty(false);
//false
isTruty(NaN);
//false

/*
Invoque a função criada acima passando como parâmetro 10 valores `truthy`.
*/
 isTruty({});
//true
isTruty([]);
//true
isTruty(1);
//true
isTruty("Clovis");
//true
isTruty(function(){});
//true
isTruty(10+10);
//true
isTruty(12);
//true
isTruty([2,4]);
//true
isTruty("Clovis Lindo");
//true
isTruty(1,2,3);
//true

/*
Declare uma variável chamada `carro`, atribuindo à ela um objeto com as
seguintes propriedades (os valores devem ser do tipo mostrado abaixo):
- `marca` - String
- `modelo` - String
- `placa` - String
- `ano` - Number
- `cor` - String
- `quantasPortas` - Number
- `assentos` - Number - cinco por padrão
- `quantidadePessoas` - Number - zero por padrão
*/
var carro = {
... marca: "VW",
... modelo : "GOL",
... placa : "abc1234",
... ano : 2009,
... cor : "Branco",
... quantasPortas: 4,
... assentos : 5,
... qtdPessoas : 0
... };

/*
Crie um método chamado `mudarCor` que mude a cor do carro conforme a cor
passado por parâmetro.
*/
 carro.mudaCor = function(cor){
... carro.cor = cor;
... }

/*
Crie um método chamado `obterCor`, que retorne a cor do carro.
*/
carro.obterCor = function(){
... return carro.cor
... }

/*
Crie um método chamado `obterModelo` que retorne o modelo do carro.
*/
 carro.obterModelo = function(){
... return carro.modelo;
... }

/*
Crie um método chamado `obterMarca` que retorne a marca do carro.
*/
carro.obterMarca = function(){
... return carro.marca;
... }

/*
Crie um método chamado `obterMarcaModelo`, que retorne:
"Esse carro é um [MARCA] [MODELO]"
Para retornar os valores de marca e modelo, utilize os métodos criados.
*/
carro.obterMarcaModelo = function(){
... return "Esse carro é "+carro.obterMarca()+" "+carro.obterModelo();
... }

/*
Crie um método que irá adicionar pessoas no carro. Esse método terá as
seguintes características:
- Ele deverá receber por parâmetro o número de pessoas entrarão no carro. Esse
número não precisa encher o carro, você poderá acrescentar as pessoas aos
poucos.
- O método deve retornar a frase: "Já temos [X] pessoas no carro!"
- Se o carro já estiver cheio, com todos os assentos já preenchidos, o método
deve retornar a frase: "O carro já está lotado!"
- Se ainda houverem lugares no carro, mas a quantidade de pessoas passadas por
parâmetro for ultrapassar o limite de assentos do carro, então você deve
mostrar quantos assentos ainda podem ser ocupados, com a frase:
"Só cabem mais [QUANTIDADE_DE_PESSOAS_QUE_CABEM] pessoas!"
- Se couber somente mais uma pessoa, mostrar a palavra "pessoa" no retorno
citado acima, no lugar de "pessoas".
*/
carro.addP = function(qtd){
... totPessoas = carro.qtdPessoas + qtd;
...
... if(carro.qtdPessoas === carro.assentos && totPessoas >= carro.assentos){
... return "O carro esta lotado!";
... }
...
... if(totPessoas > carro.assentos){
... var assentosDisponiveis = carro.assentos - carro.qtdPessoas;
... var Pessoa = assentosDisponiveis === 1 ? "pessoa" : "pessoas";
... return "Só cabe mais "+assentosDisponiveis+ Pessoa+ "!";
... }
...
... carro.qtdPessoas += qtd;
... return "Temos " +carro.qtdPessoas+ " pessoas no carro!";
}

/*
Agora vamos verificar algumas informações do carro. Para as respostas abaixo,
utilize sempre o formato de invocação do método (ou chamada da propriedade),
adicionando comentários _inline_ ao lado com o valor retornado, se o método
retornar algum valor.

Qual a cor atual do carro?
*/
carro.cor
//'Branco'

// Mude a cor do carro para vermelho.
carro.cor = "vermelho"
//'vermelho'

// E agora, qual a cor do carro?
carro.cor
//'vermelho'

// Mude a cor do carro para verde musgo.
carro.cor = "Verde Musgo"
//'Verde Musgo'

// E agora, qual a cor do carro?

carro.cor 
//'Verde Musgo'

// Qual a marca e modelo do carro?

carro.obterCarroModelo();
'Esse carro é VW GOL'

// Adicione 2 pessoas no carro.
 carro.addP(2);
//'Temos 2 pessoas no carro!'

// Adicione mais 4 pessoas no carro.

carro.addP(4);
//'Só cabe mais 3pessoas!'

// Faça o carro encher.

carro.addP(3);
//'Temos 5 pessoas no carro!'

// Tire 4 pessoas do carro.
carro.addP(-4);
//'Temos 1 pessoas no carro!'

// Adicione 10 pessoas no carro.
 
 carro.addP(10);
'O carro esta lotado!'

// Quantas pessoas temos no carro?
carro.qtdPessoas
//5
```
