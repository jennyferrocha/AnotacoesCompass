# *Módulo 2* - **Blockchain: Safe Shallows**

## **Bitcoin**

#### CONCEITOS FUNDAMENTAIS: 
    - O Bitcoin é uma unidade de troca para comprar bens e serviços.

- não é necessário serviço externo para realizar transferência;
- possui reserva de valor (através da compra de bitcoins);
- tem um limite máximo de 21 milhões de unidades, o que resulta numa escassez digital;
- o bitcoin "talvez" substitua o sistema financeiro;
- através do bitcoin não pode realizar empréstimos e nem comprar ações.

*Vantagens: liberdade de pagamento, segurança, privacidade, taxas menores, controle e transparência.*

#### CARACTERÍSTICAS

- _Criptografia_: usada para garantir que as transações sejam seguras e que apenas o proprietário legítimo de um bitcoin possa gastá-lo. Cada transação é assinada digitalmente com uma chave privada;
- _Blockchain_: é tipo um livro público que registra todas as transações de Bitcoin. Cada transação é agrupada em blocos, que são conectados uns aos outros em uma cadeia. Isso garante segurança e transparência, pois uma vez que um bloco é adicionado, ele é imutável e visível para todos na rede;
- _Redes Descentralizadas_: O Bitcoin não é controlado por uma autoridade central, como um governo ou banco central. Ele opera em uma rede ponto a ponto (peer-to-peer), onde todos os participantes têm uma cópia do histórico de transações e podem validar as transações.
- _"Engenharia de Incentivo"_: se seguir as seguir, é retribuído com ganho de dinheiro.

#### BITCOIN vs. BANCOS

| Características | Sistema Tradicional | Bitcoin |
| --- | --- | --- |
| CONTABILIDADE   | Centralizada   | Blockchain status |
| ARMAZENAMENTO |Fracionado | 100%|
| SEGURANÇA | Institucional | Criptográfica |
| EMISSÃO DE MOEDA |Política Econômica | Algoritmo|
| TRANSAÇÕES | Centralizado | Distribuído, peer-to-peer |
| AUTENTICAÇÃO | Centralizado| Blockchain |
| REGULAMENTAÇÃO | Banco Central, Normas |Ainda Indefinida|
| PROCESSO DE DECISÃO | Arbitrário |Consenso  |
| CONTROLE DE DINHEIRO | Banco | Você |

#### COMO COMPRAR E VENDER BITCOINS

Atualmente existem três maneiras de adquirir bitcoins de maneira eficiente:

- MINERAR: É possível adquirir Bitconis através da mineração. E será necessário um computador específico para isso e ceder seu poder computacional para a rede, confirmando transações. Para cada bloco minerado, você será recompensado.
- FOXBIT: Bitcoins adquiridos através de Exchanges como a Foxbit. As Exchanges são sites que reúnem compradores e vendedores em um ambiente seguro, onde as trocas ocorrem de forma anônima e rápida.
- P2P: Compra de Bitcoins diretamente com outras pessoas, sem precisar passar por uma exchange. 

#### CARTEIRAS (WALLETS) NO BITCOIN

- São softwares ou dispositivos que permitem aos usuários armazenar, enviar e receber bitcoins de forma segura; 
- Elas gerenciam as chaves criptográficas necessárias para acessar os bitcoins na blockchain, onde todas as transações são registradas;
- Cada carteira contém uma chave pública (endereço de conta) e uma chave secreta (senha para assinar transações e gastar os bitcoins).

#### TIPOS DE CARTEIRAS BITCOIN

1. *CARTEIRA DE PAPEL*
   - Documento físico impresso que contêm a chave pública (CP) e a chave secreta (CS);
   -  Tão seguro quanto o papel;
   -  Imune a hackers;
   -  Inconveniente para transações, pois não oferece serviços;
   -  Cada carteira tem apenas um par de CP/CS;
   -  Fácil de rasgar e precisa ser guardada com muito cuidade;
   -  A perda da chave secreta, resultará na perda dos bitcoins.

2. *CARTEIRA DE HARDWARE*
   - Dispositivo físico, como pendrives;
   - Extremamente seguras: armazenam a chave secreta offline;
   - Interface segura com computador;
   - Recuperação das moedas e outros serviços;
   - Permite múltiplos pares CP/CS (infinitas chaves);
   - Os hackers não conseguem acesso;
   - O preço dessa carteira é alto.

3. *CARTEIRA DE SOFTWARE*
   - Desktop ou Mobile;
   - Permite múltiplas pares de CP/CS;
   - Recuperação das moedas e outros serviços;
   - Tão seguro quanto seu computador ou smartphone;
   - Muitas são adaptadas a mais de um tipo de moeda;
   - Envia bitcoins.

4. *CARTEIRA ONLINE*
   - Acessada por meio de navegadores e geralmente hospedada por terceiros;
   - Recebe Bitcoins;
   - Envia Bitcoins, mas não pode errar a chave, pois não é possível recuperar;
   - O usuário não sabe a chave secreta, está armazenada na nuvem;
   - Mais vulnerável a ataques.
  
## **Blockchain**

    - É uma estrutura para armazenamento de dados que consiste de vários blocos conectados entre si. Um esquema criptográfico garante a inviolabilidade da cadeia.
  
- Um livro-razão digital;
- Distribuído a todos os membros da rede;
- Descentralizado, pois nenhuma autoridade tem poder supremo sobre o sistema;
- Criptografado e protegido por meio de criptografia;
- Imutável, o que significa que cada alteração é permanente no livro-razão;
- Cada nó da rede segue um consenso.

Existe uma cadeia linear de blocos e cada bloco está conectado ao bloco anterior. Cada um dos blocos contêm quatro componentes principais:
  - _Dados_ — Qualquer informação que você deseja armazenar com segurança nos blocos;
  - _Hash_ — Identificador exclusivo atribuído a um bloco específico;
  - _Hash do bloco anterior_ — Inclui o valor de hash anterior para construir a estrutura dos blocos;
  - _Metadados_ — Dados relevantes sobre os dados dentro do bloco; ou seja, carimbo de data/hora ou número de bloco.

Esses quatro componentes criam essencialmente o esqueleto de todo a blockchain.

![Como funciona a Blockchain](https://101blockchains.com/wp-content/uploads/2018/09/Como-funciona-a-BlockChain-Passo-a-Passo.png.webp)

#### FUNÇÕES HASH

- Transformam um texto de entrada (input) em um texto de saída (output) de tamanho fixo;
- O texto de entrada pode ter qualquer tamanho;
- O texto de saída sempre tem o mesmo tamanho.

| INPUT | HASH FUNCTION | HASH SUM |
| --- | --- | --- |
| Raposa --> | Hash Function --> |  DFCDE454 |
| A raposa vermelha corre pelo gelo --> | Hash Function --> | 52ED879E |
| A raposa vermelha trabalha no gelo --> | Hash Function --> | 46042841 |

#### FUNÇÕES HASH CRIPTOGRÁFICAS

- Fácil de computar;
- Livre de colisão: impossível dois inputs com o mesmo output;
- Unidirecional: impossível descobrir o input dado seu hash;
- "Puzzle Friendly": amigável com quebra-cabeças.

#### ASSINATURAS DIGITAIS

- por meio de dados;
- só você pode assinar (assinatura única);
- qualquer um pode verificar sua assinatura;
- assinatura atrelada ao documento;
- impossível de falsificar.

## **O Bitcoin**

#### A REDE BITCOIN
  - Distribuída;
  - Sem hierarquia;
  - Protocolo de Consenso.
  
> Qualquer computador conectado à rede blockchain é um nó desta rede.

- Full Nodes: (_MINERADORES_)
  - validam todas as transações emitidas pela rede;
  - mantém a consistência do blockchain.

- Lite Nodes: (_CARTEIRAS_)
  - não armazena todo o blockchain;
  - necessitam de informação de outros nós.

#### TRANSAÇÃO DE BITCOIN
- Uma transação de Bitcoin envolve a transferência de bitcoins de uma carteira para outra usando a tecnologia blockchain. Cada transação é validada por mineradores e registrada de maneira pública e imutável no blockchain.

1. Cada usuário de Bitcoin possui uma chave privada e uma chave pública. A chave pública é o endereço da carteira do usuário (como um número de conta bancária), e a chave privada é usada para assinar digitalmente as transações, provando a propriedade dos bitcoins;
2. Toda transação tem um ou mais "inputs" e "outputs":
   - Inputs: São as transações anteriores de onde o Bitcoin está vindo (quem enviou para você).
   - Outputs: É o endereço (chave pública) de quem vai receber o Bitcoin.
3. Depois de criar e assinar a transação, o remetente a transmite para a rede Bitcoin. A transação é então enviada para todos os nós;
4. Validação da Transação:
   - Validação pelos Nós: Cada nó da rede recebe a transação e verifica se ela é válida. Eles verificam se:
     - O remetente tem bitcoins suficientes para enviar;
     - A assinatura digital é válida (garantindo que foi o remetente autorizado quem iniciou a transação).
   - Mineração e Inclusão no Bloco: As transações são agrupadas em blocos por mineradores. Esses mineradores competem para validar o bloco que contêm as transações (Proof of Work) e só se tornam efetivas quando são inseridas no blockchain. A mineração garante que todos os nós mantenham o mesmo blockchain armazenado.
5. Após a inclusão da transação no blockchain, o destinatário poderá ver que recebeu os bitcoins. Como o blockchain é público, qualquer pessoa pode verificar o histórico da transação e sua confirmação.
A transferência de Bitcoin é considerada concluída e irreversível após o recebimento das confirmações.

## _Exemplo Simplificado de uma Transação de Bitcoin:_
1.  Fernanda quer enviar 1 Bitcoin para João;
2. Fernanda cria uma transação com os seguintes detalhes:
     - Input: Bitcoins que Fernanda recebeu em uma transação anterior.
     - Output: Endereço de João (chave pública).
3. Fernanda assina a transação com sua chave privada e a envia para a rede;
4. A transação é validada pelos nós e incluída por um minerador em um novo bloco;
5. O bloco é adicionado ao blockchain, e a transação agora é registrada publicamente e permanentemente;
6. João recebe o Bitcoin em sua carteira.

![Exemplo do Processo de Validação](https://www.nucleodoconhecimento.com.br/wp-content/uploads/2021/05/grafico-3-23.png)


#### PROOF OF WORK

É usado em redes de blockchain para garantir a segurança e a validação de transações. Basicamente, os computadores (mineradores) competem para resolver um problema matemático muito difícil. O primeiro a resolver o problema ganha o direito de adicionar um novo bloco de transações à blockchain e recebe uma recompensa em criptomoeda. Esse processo é chamado de "prova de trabalho" porque mostra que o minerador fez um esforço computacional para resolver o problema.

![O ciclo de funcionamento da prova de trabalho](https://shardeum.nyc3.cdn.digitaloceanspaces.com/shardeum/2022/09/How-Proof-of-Work-works.png)

#### _PORQUE A "PROVA DE TRABALHO" É IMPORTANTE:_

- Satoshi Nakamoto criou o Bitcoin, a primeira criptomoeda, em 2008, marcando o início da comunidade cripto como a conhecemos hoje. Em seu famoso white paper, Nakamoto apresentou uma moeda digital baseada em protocolos de proof of work (prova de trabalho), que permitiria transações seguras sem a necessidade de uma autoridade central.
- O "problema do gasto duplo" era um grande desafio para a criação de dinheiro digital eficaz. _Esse problema ocorre quando alguém tenta gastar a mesma moeda mais de uma vez._ Sem uma solução para isso, a moeda digital se tornaria inflacionária e perderia valor.
- A prova de trabalho resolve esse problema sem a necessidade de um líder central. Ela garante que os mineradores verifiquem a validade de cada transação antes de adicioná-la ao blockchain, evitando o gasto duplo e mantendo a moeda estável e segura.

Com esse mecanismo, a prova de trabalho se torna essencial para a integridade das criptomoedas, impedindo fraudes e garantindo que as transações sejam confiáveis.

## **REVISÃO**

- O Blockchain é um registro público e imutável de todas as transações já realizadas desde a criação do Bitcoin;
- Identidade: Chave Pública;
- Segurança: assinaturas digitais e Chave Secreta;
- Rede peer-to-peer e protocolo de consenso;
- Mineradores (impedem gastos duplos): criam novos blocos com as novas transações válidas. Competem pelo direito de adicionar  próximo bloco à cadeia através de proof of work, recebem novos bitcoins como recompensa.

## **LINKS**

- [Blockchain de forma simples](https://101blockchains.com/blockchain-explained/)
- [Blockchain Demo](https://blockchaindemo.io/)
- [Blockchain na Prática](https://www.youtube.com/watch?v=7C4WLunfW3E)
- [Anotações Pessoais - PDF](https://drive.google.com/file/d/148DcFeTpnuvdWnbhUxoYFexYvkfWJnqw/view?usp=sharing)








  






