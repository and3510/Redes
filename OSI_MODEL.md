
Antigamente, existia varios tipos de padroes de proprietarios. O problema é que a maioria das vezes dava conflito pela incompatibilidade, devido os diferentes tipos de fabricantes.

Por isso, Crio-se o padrao de modelo OSI - (Open Systems Interconnection) desenvolvida pela ISO (International Standard Organization) com o objetivo de criar uma estrutura para definição de padrões para a conectividade e interoperabilidade de sistemas diferentes.

Modelo define um conjunto de 7 camadas (em inglês layers) e os serviços atribuídos a
cada uma, porém o modelo OSI é uma referência e não uma implementação!

### 1 Camada - Fisica:

- Trata da transmissão transparente de sequências de bits pelo meio físico.
- Contém padrões mecânicos (conectores, painéis de conexão, cabos, etc.), funcionais, elétricos e procedimentos para acesso a esse meio físico.
- satélite, coaxial, radiotransmissão, par metálico, fibra óptica, etc.

![[Pasted image 20240519011437.png]]


### 2 Camada - Enlace:

Esconde características físicas do meio de transmissão para as camadas superiores, pois ele transforma os bits em quadros (frames). Sua principal função é fornecer um meio de transmissão confiável entre dois sistemas adjacentes.

- Delimitação e formato dos quadros de bits
- Detecção de erros
- Sequenciamento dos dados
- Controle de fluxo de quadros
- Endereçamento físico (endereço MAC)
- Controle de acesso aos meios físicos


Para redes locais a camada de enlace é dividida em dois subníveis:

- LLC (Logical Link Control)
- MAC (Media Access Control)

obs: LLC faz interface com a camada de rede e o MAC com a camada física.

As informações trocadas pelos protocolos de camada 2, tais como o ethernet, fastethernet, PPP, HDL e demais são chamadas de quadros.

![[Pasted image 20240519012409.png]]

### 3 Camada - Rede

Função de fornecer um canal de comunicação independente do meio, pois ela transmite pacotes de dados através da rede utilizando um esquema de endereçamento lógico que pode ser “roteado” através de diversas redes até chegar ao seu destino.

- Tradução de endereços lógicos em endereços físicos (protocolo ARP)
- Esquema de endereçamento lógico
- Roteamento de pacotes
- Não possuem garantia de entrega dos pacotes

Os protocolos de camada 3 utilizados atualmente tanto na Internet como nas Intranets são o IP versão 4 e o IP versão 6 (o IPv6 está sendo aos poucos implementado em diversas redes e na Internet).

As informações trocadas pelos protocolos de camada 3, tais como o IP, são chamadas de
pacotes.

É importante ressaltar aqui que a comunicação em rede propriamente dita é realizadas pelas
camadas 1, 2 e 3.

![[Pasted image 20240519013042.png]]