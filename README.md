@Uchoa Jorgiano@

Portal cativo


A função do Captive Portal no pfSense permite proteger uma rede exigindo um nome de usuário e senha (ou apenas um clique), inseridos em uma página do portal.

Se a autenticação for usada, isso pode ser feito usando o gerenciamento de usuários integrado do pfSense ou um servidor de autenticação externo, como um servidor RADIUS.

A melhor fonte de informações do portal cativo pode ser encontrada no livro pfSense .

O portal cativo é configurado a partir de serviços> portal cativo .

Existem várias guias disponíveis para a configuração do portal cativo, cada uma descrita abaixo:

Zones
Zonas de portal cativas permitem a criação de portais separados e independentes que operam em uma ou mais interfaces separadas. Por exemplo, pode haver uma zona para Wireless e uma zona para Wired. Cada zona tem um conjunto completamente isolado de páginas, configuração, usuários, etc.

Uma zona pode ser usada por várias interfaces, mas somente uma zona pode ser usada por interface.

Captive Portal Tab
Gerenciamento geral da configuração e autenticação do portal cativo. Cada opção é descrita em detalhes na página

Guia Pass-Through MAC 
Permite gerenciar uma lista de endereços MAC que podem contornar o portal.

Quando especificado pelo endereço MAC dessa maneira, o endereço IP do cliente pode mudar e eles ainda serão permitidos. No entanto, o cliente ainda será desconectado após o período de tempo limite do portal cativo ter decorrido.

Endereços IP permitidos 
Permite gerenciar uma lista de endereços IP que podem:

Sempre conecte por trás do portal (clientes)
Permitir sempre clientes para um endereço IP (servidores externos)
Esses endereços IP ignoram a autenticação do portal na direção especificada.

Vouchers
Códigos de acesso de portal de uso único, descritos em mais detalhes em: Cupons do portal cativo .

Gerenciador de arquivos 
Permite o gerenciamento dos arquivos que podem ser usados ​​para compor o conteúdo da página de autenticação / click-through do portal cativo.


