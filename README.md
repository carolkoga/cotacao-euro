# cotacao-euro
 websocket para cotar euro/reais

**Descrição Detalhada**

Este projeto é uma aplicação em tempo real que utiliza WebSocket para realizar a conversão de Euro (EUR) para Reais (BRL) com base na cotação atual. Ele foi desenvolvido para demonstrar como a comunicação bidirecional e em tempo real pode ser implementada usando WebSocket, além de integrar APIs externas para obter dados atualizados.

**Servidor WebSocket:**

O servidor é implementado em Python usando a biblioteca websockets.
Ele escuta conexões na porta 8765 e aguarda que clientes se conectem.
Quando um cliente envia um valor em Euro, o servidor:Obtém a cotação atual do Euro (EUR-BRL) usando a API do Google Finance ou outra fonte confiável.
Realiza a conversão do valor enviado pelo cliente.
Retorna o valor convertido em Reais ao cliente.


**Cliente WebSocket:**

O cliente pode ser implementado em qualquer linguagem que suporte WebSocket (neste caso, Python).
Ele se conecta ao servidor e envia valores em Euro.
Recebe o valor convertido em Reais em tempo real.


**Obtenção da cotação:**

A cotação do Euro (EUR-BRL) é obtida em tempo real usando a biblioteca requests para fazer uma requisição HTTP ao Google Finance ou outra API de cotações.
A cotação é atualizada a cada requisição, garantindo que os valores convertidos estejam sempre precisos.


**Comunicação em tempo real:**

O WebSocket permite uma comunicação bidirecional e contínua entre o cliente e o servidor.
Isso é ideal para aplicações que exigem atualizações instantâneas, como conversores de moeda, chats ou notificações.

**Casos de Uso**

Este projeto pode ser utilizado em diversas situações, como:

Aplicações financeiras: Para fornecer conversões de moeda em tempo real.
Sistemas de e-commerce: Para exibir preços em diferentes moedas.
Educação: Como exemplo de implementação de WebSocket e integração com APIs externas.

**Tecnologias Utilizadas**

Python: Linguagem principal do projeto.
WebSocket: Protocol

-------------------------------------------------------

# Conversor de Euro para Reais via WebSocket

Este projeto consiste em um servidor WebSocket que realiza a conversão de Euro (EUR) para Reais (BRL) em tempo real. Ele permite que clientes se conectem ao servidor, enviem valores em Euro e recebam o valor convertido em Reais, com base na cotação atual.

## Funcionalidades

- **Conversão em tempo real**: Obtém a cotação atual do Euro (EUR-BRL) e realiza a conversão de valores.
- **Conexão via WebSocket**: Utiliza WebSocket para comunicação em tempo real entre cliente e servidor.
- **Escalabilidade**: O servidor pode lidar com múltiplos clientes simultaneamente.

## Pré-requisitos

Antes de executar o projeto, certifique-se de ter o Python instalado e os seguintes pacotes:

- `websockets`
- `requests`
- `asyncio`
