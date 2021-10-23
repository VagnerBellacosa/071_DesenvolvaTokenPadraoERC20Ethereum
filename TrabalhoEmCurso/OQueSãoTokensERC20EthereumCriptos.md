# O que são tokens ERC-20 e como eles garantem o sucesso da Ethereum no mundo das criptos

[![img](https://cointelegraph.com.br/assets/img/explained/svg/user.svg)Maxwell William](https://cointelegraph.com.br/authors/maxwell-william)

![img](https://cointelegraph.com.br/assets/img/explained/svg/clock.svg)12 MAI 2018

![O que são tokens ERC-20 e como eles garantem o sucesso da Ethereum no mundo das criptos](https://images.cointelegraph.com/images/1024_aHR0cHM6Ly9zMy5jb2ludGVsZWdyYXBoLmNvbS9zdG9yYWdlL3VwbG9hZHMvdmlldy80ZTM1Y2FkYzM3OTc4MGVjNjZmZDM5MWVkZWY1OWZiMC5qcGc=.jpg)

[![Cointelegraph]()](https://cointelegraph.com/)

Cointelegraph



**1.**

## O que são tokens ERC-20?

**2.**

## Em primeiro lugar, o que é Ethereum?

**3.**

## Onde os contratos inteligentes entram nisso tudo?

**4.**

## O que acontece depois que um contrato inteligente cria um token?

**5.**

## Peguei a analogia, mas como exatamente tudo isso funcionaria?

**6.**

## Agora, sobre as regras obrigatórias: o que é [totalSupply]?

**7.**

## E a [transfer]?

**8.**

## O que a função [balanceOf] faz?

**9.**

## Como posso receber tokens ERC-20 de outros usuários?

**10.**

## Existe alguma maneira de se criar um token falso?

**11.**

## Posso mentir e dizer que tenho mais tokens do que realmente tenho?

**12.**

## Quais são os benefícios do ERC-20?

**13.**

## O ERC-20 tem algum defeito?

**14.**

## Chega de hipóteses, quero um exemplo no mundo real

**1.**

## O que são tokens ERC-20?

*Tokens ERC-20 são tokens projetados e usados somente na plataforma Ethereum.*

Eles seguem uma lista de padrões para que possam ser compartilhados, trocados por outros tokens ou transferidos para uma carteira de criptomoeda.

A comunidade Ethereum criou esses padrões com três regras opcionais e seis obrigatórias.

**Opcionais**

- Nome do Token
- Símbolo
- Decimal (até 18)

**Obrigatórias**

- totalSupply
- balanceOf
- transfer
- transferFrom
- approve
- allowance

Confuso? Vamos dar um passo atrás.

**2.**

## Em primeiro lugar, o que é Ethereum?

*[Ethereum](https://br.cointelegraph.com/tags/ethereum) é uma rede de computadores descentralizada com duas funções básicas.*

São elas: uma blockchain que pode gravar transações e uma máquina virtual que pode produzir contratos inteligentes.

Por causa dessas duas funções, a Ethereum tem a capacidade de suportar aplicativos descentralizados (DApps). Esses DApps são construídos sobre a blockchain existente da Ethereum, pegando carona de sua tecnologia subjacente. Em troca, a Ethereum cobra dos desenvolvedores pelo poder de computação em sua rede, que só pode ser pago em Ether, a única moeda aceita entre as plataformas.

Dependendo de seu propósito, os DAPPs podem criar tokens ERC-20 para funcionar como moeda, participação numa empresa, pontos em um programa de fidelidade ou até mesmo comprovante de propriedade, digamos, de uma quantia de ouro ou da escritura em uma casa.

**3.**

## Onde os contratos inteligentes entram nisso tudo?

*Contratos inteligentes são usados para criar tokens ERC-20.*

Eles também são usados para facilitar transações de tokens e registrar saldos de tokens em uma conta.

Os contratos inteligentes são escritos na linguagem de programação "Solidity" com base na lógica If-This-Then-That (IFTTT - Se-Isso-Então-Aquilo, em tradução livre).

Pense nisso como uma máquina de venda automática.

![Where do smart contracts fit into all this?](https://cointelegraph.com/storage/uploads/view/dbe3a6f854b09aa99072a6b2484fa391.png)

**4.**

## O que acontece depois que um contrato inteligente cria um token?

*É aqui que entra o ERC-20.*

Depois que um token é criado, ele pode ser negociado, gasto ou dado a outra pessoa.

O ERC-20 é a linguagem universal usada por todos os tokens da rede Ethereum. Ela permite que um token seja negociado com outro.

Vamos supor que queiramos fazer um cassino cripto. Assim como em um cassino tradicional, queremos que nossos jogadores usem nossas fichas, para simplificar.

Assim, um jogador troca seu dinheiro fiduciário pelos nossos tokens e dirige-se a uma mesa de pôquer.

**5.**

## Peguei a analogia, mas como exatamente tudo isso funcionaria?

*Vamos dar uma olhada em cada uma das regras do ERC-20 em nosso exemplo de "cassino cripto".*

É muito importante que os desenvolvedores as sigam.

Vamos começar com as regras opcionais:

Nome do Token: Chip Blu

Símbolo: BLU

Decimal: 2*

**Queremos que nossos tokens sejam divisíveis, de modo que uma aposta mínima de jogadores seja 0,01 BLU. Poderíamos deixar o decimal em 0 e fazer de 1 o mínimo de BLU ou aumentar o decimal para 18 resultando em .000000000000000001 BLU a menor divisão possível, mas vamos ficar na opção mais simples.*

**6.**

## Agora, sobre as regras obrigatórias: o que é [totalSupply]?

*[totalSupply] identifica o número total de tokens ERC-20 criados.*

A primeira coisa que nosso cassino precisa saber é o total de quantos tokens BLU estão em circulação. Digamos que nossa mesa de pôquer tenha um total de 10 BLUs com dez jogadores.

![Now to the mandatory rules: what is [totalSupply]?](https://cointelegraph.com/storage/uploads/view/bb5863baa6b28c068f2cc43bc52497d8.png)

**7.**

## E a [transfer]?

*A [transfer] permite que um determinado número de tokens seja transferido do montante total para uma conta de usuário.*

Antes do início do jogo, os jogadores devem receber o BLU do crupiê.

Cada jogador recebe 1 BLU.

![What about [transfer]?](https://cointelegraph.com/storage/uploads/view/609bcb7c8a367b2015ac3b11e99a2b70.png)

**8.**

## O que a função [balanceOf] faz?

*Quando a função [balanceOf] é executada, retorna o número de tokens que um determinado endereço possui a sua conta.*

Na primeira mão do nosso jogo de pôquer, 5 dos jogadores olharam suas cartas e decidiram não jogar. Cada um dos 5 restantes decidiu apostar 0,5 BLU. Usando a [balanceOf], vemos que cinco dos jogadores têm 1 BLU e 5 têm 0,5 BLU.

![What does the function [balanceOf] do?](https://cointelegraph.com/storage/uploads/view/aa3061e268923d5fd3979802e5f35afd.jpg)

**9.**

## Como posso receber tokens ERC-20 de outros usuários?

*É a função [transferFrom] que permite que um usuário transfira tokens para outro usuário.*

Boas notícias! Você venceu a primeira mão e ganhou 2,5 BLU dos outros jogadores.

Mas para pegar suas fichas isso deles, você precisa da [transferFrom]. Sem isso, o que impede alguém de roubar seu BLU?

![How can I get ERC-20 tokens from other users?](https://cointelegraph.com/storage/uploads/view/844283234ab72bda15c3630b3d200c18.png)

**10.**

## Existe alguma maneira de se criar um token falso?

*Não mesmo, porque o [approve] verifica uma transação frente ao fornecimento total de tokens.*

Certifique-se de que não há nada a mais nem a menos.

Outra forma de salvaguardar a integridade do nosso hipotético jogo de pôquer é garantir que ninguém tenha trazido BLUs a mais para a mesa. Então, a função [approve] autoriza a mudança de mãos das fichas, verificando se o número total de BLU na tabela é igual a 10.

![Is there any way to make a counterfeit token?](https://cointelegraph.com/storage/uploads/view/9ee839b7047df962f60ef103c3172fff.png)

**11.**

## Posso mentir e dizer que tenho mais tokens do que realmente tenho?

*Não!*

Antes de uma transação ocorrer, a função *[allowance]* verifica o saldo da conta do usuário e cancela a transação caso não haja tokens suficientes.

Não trabalhamos com créditos em nosso "cassino cripto", por isso, precisamos garantir que cada jogador tenha BLU suficiente para fazer a aposta. Se eles tiverem apenas 1 BLU, eles não poderão apostar 2 BLU.

**12.**

## Quais são os benefícios do ERC-20?

*Basicamente, ele torna tudo mais simples.*

Antes dos tokens ERC-20, os desenvolvedores podiam usar outras terminologias no código.

Por exemplo - um token usa *[totalAmount]* enquanto outro usa *[totalNumber]*.

Exchanges e carteiras necessárias para construir suas plataformas para acomodar cada código de um token.

Com um padrão universal, novos tokens podem ser colocados em uma exchange ou transferidos para uma carteira automaticamente, logo depois de criados.

O ERC-20 também torna a criação de novos tokens extremamente fácil e é por isso que o Ethereum [se tornou](https://techcrunch.com/2017/06/08/how-ethereum-became-the-platform-of-choice-for-icod-digital-assets/) a plataforma mais popular para ICO em 2017.

**13.**

## O ERC-20 tem algum defeito?

*Nem o ERC-20 não é perfeito.*

Existem alguns problemas que os padrões de token ERC-20 não abordam.

Há situações em que os tokens podem ser destruídos acidentalmente quando são usados como pagamento por um contrato inteligente, em vez de usar o Ether. [Estima-se](https://github.com/Dexaran/ERC223-token-standard) que US$ 3 milhões já foram perdidos por causa disso.

Para corrigir esse bug, a comunidade Ethereum está atualmente trabalhando em um novo padrão chamado [ERC-223](https://medium.com/cryptomover/what-are-erc20-and-erc223-tokens-307badcca5a). Esses padrões não são compatíveis com o ERC-20, portanto, os desenvolvedores são incentivados a continuar usando o ERC-20 até que a compatibilidade seja realizada.

Em abril de 2018, várias exchanges [suspenderam](https://br.cointelegraph.com/news/multiple-exchanges-suspend-erc20-token-trading-due-to-potential-batchoverflow-bug) depósitos e saques de tokens baseados em Ethereum devido ao bug [batchOverflow](https://medium.com/@peckshield/alert-new-batchoverflow-bug-in-multiple-erc20-smart-contracts-cve-2018-10299-511067db6536). Ele é descrito como um "problema clássico do estouro do número inteiro" e pode permitir que um invasor "apodere-se de uma enorme quantidade de tokens".

Foi [observado](https://medium.com/@peckshield/alert-new-batchoverflow-bug-in-multiple-erc20-smart-contracts-cve-2018-10299-511067db6536) que não há uma abordagem de segurança tradicional para corrigir essas vulnerabilidades no momento.

**14.**

## Chega de hipóteses, quero um exemplo no mundo real

*Cada token na plataforma Ethereum é um token ERC-20.*

A [numeração](https://etherscan.io/tokens) atual é de 82815 no momento desta publicação, vamos dar uma olhada em alguns deles.

O [EOS](https://eos.io/) (EOS), atualmente a 5ª maior criptomoeda, com quase US$ 12 bilhões em valor de mercado, está tentando construir uma rede que pode utilizar comunicação interblockchain e o [TRON](https://tron.network/enindex.html) (TRX), que [ocupa](https://coinmarketcap.com/currencies/tron/) a 10ª posição entre as criptomoedas no momento, é descrito como um "protocolo de código aberto para a indústria do entretenimento digital". Ele tem como objetivo lançar uma plataforma de conteúdo com ecossistema conectando todas as pessoas criando diferentes tipos de conteúdo.

Uma "plataforma blockchain pública de nível empresarial", o [VeChain](https://www.vechain.org/) (VEN), a [15ª](https://coinmarketcap.com/currencies/vechain/) criptomoeda em termos de capitalização de mercado, está planejando implementar a tecnologia da Internet das Coisas (IoT) para fornecer chaves privadas para que cada produto permita rastreá-las.