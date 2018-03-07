# Um Simples Chat desenvolvido com Shell Script

## Sinopse
Este é um simples chat desenvolvido em Shell script utilizando o intepretador **BASH** utilizando tambem ferramentas como **tmux** e **netpipes**, o mesmo aceita multiplas conexões.

## Motivação
Como é um projeto simples de encontrar em outras linguagens, vi a necessidade de desenvolver um simples projeto utilizando Shell Script para servir como exemplo para quem procura algo do tipo, já que o mesmo não é simples de encontrar.

## Pré-requisitos
Como citado acima, foram utilizadas duas ferramentas tmux e netpipes. Recomendamos utilziar um sistema baseado em **linux**, neste caso foi utilizado a distribuição Ubuntu 16.04, tanto para o servidor(utilizado ip publico) como para os clientes. <br>
Para instalar o Tmux utilize o comando:<br>
```
sudo apt-get install tmux
```
Para instalar o netpipes utilize o comando:<br>
```
sudo apt-get install netpipes
```

Ou caso não possui nenhuma das ferramentas, pode ser optado pelo comando:<br>
```
sudo apt-get install tmux netpipes
```

## Testes
### Servidor
Copie o script **server.sh** para a maquina que você utilizará como Servidor (pode ser usada a mesma que você usará como cliente), acesse o diretório pelo terminal onde você colocou o script (server.sh) dê a permissão para execução e execute.<br>
Dando permissões de execução:<br>
```
chmod +x server.sh
```
Executando o script:<br>
```
./server.sh
```
<br>

### Cliente
Acesse o diretório dos scripts do cliente, dê a permissão de execução para todos (cliente.sh, user_msg.sh, user_tela.sh) e execute o script **cliente.sh**.<br>
Dando permissões de execução:<br>
```
chmod +x cliente.sh user_msg.sh user_tela.sh
```
Executando o script:<br>
```
./cliente.sh
```

Ao executar o script do Cliente, será requisitado o nome de usuario e o IP do Servidor, após fornecer essas informações ja será possivel enviar mensagem para todos que estejam conectados.<br>

### Importante
Para sair do chat é recomendado utilizar o comando `exit()` dentro do chat como uma mensagem, caso você utilize o `CTRL + C` ou qualquer outro conjunto de teclas que venha parar de forma brusca o chat, pode ocorrer que aquela sessão do seu terminal que foi utilizada para executar o chat fique divida em duas telas por causa do **tmux**.

### Contribuintes
[Jardel Gonçalves](https://twitter.com/Jardel__G__F___)
