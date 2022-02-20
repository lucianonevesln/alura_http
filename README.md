# HTTP (protocolo de comunicação): https://datatracker.ietf.org/doc/html/rfc2616

* Fundamento da WEB:

Regras de comunicação para interação cliente-servidor.

Basicamente, o cliente efetua uma requisição para a rede, que pode ser composta de diversos
intermediários (roteador, modem, provedor) que ficam responsáveis por interpretar a requisição,
destiná-la e retornar um resultado do servidor.

HTTPS:

* WEB Segura

É um protocolo com os recursos HTTP com camadas de segurança SSL/TLS.

Certificado Digital: possui uma chave pública e é responsável por criptografar os dados enviado e, 
por outro lado, há uma chave privada pelo lado do servidor que fará a descriptografia dos dados
enviados.

* Endereços

https://cursos.alura.com.br/course/introducao-html-css

Protocolo | Dimínio         | Raiz    | Porta | Recurso

https:    | //cursos.alura. | com.br: | 443   | /course/introducao-html-css

Prompt:
nslookup google.com
...
Name:    google.com
Address: 216.58.202.238

O domínio (nome de endereços web) são destinados a identificação humana. Já a identificação numerada
é para facilitar o endereçamento/indexação de máquinas em rede. O processo de associação de um domínio
a uma identificação numerada se dá por meio de um DSN, que tem um banco de dados fazendo esse reconhecimento.

Porta padrão HTTP: 80.

Porta padrão HTTPS: 443.

Stateless: cada requisição é independente.

Sessão: para trabalhar com stateless preservando a identificação do usuário por um determinado tempo, utiliza-se
o recurso de sessão. Esse recurso só é possível através de outro recurso chamado de Cookie (par de chave-valor), 
que é responsável por armazenar informações no navegador(cliente).

Request-Response: ao ser requisitado algo e houver êxito no retorno, há uma série de informações contidas em 
ferramentas de desenvolvedor informando diversos dados utilizados para estabelecer essa comunicação.

* Status Code

2xx: Sucesso;

3xx: Redirecionamento;

4xx: Erro na requisição do cliente;

5xx: Erro no servidor;

Parâmetros de requisição

São adicionados na url no momento em que realizamos uma determinada busca ou acesso de página.

* Métodos

GET: receber dados;

POST: submeter dados;

DELETE: remover um recurso;

PUT: atualizar recurso;

* Serviços REST

Trata-se da junção entre URI (recurso), Operações (GET, POST, PUT, DELETE) e Representação (HTML, XML, JSON).

Request-Response em mobile. Também ocorre a união entre URI e Métodos.

HTML: linguagem de marcação

XML: linguagem de marcação;

JSON: estrutura composta por chave e valor dentro de um array;

* HTTP2

Contém todos os recursos de HTTP1, mas contém recursos avançados para atender melhor a demanda advinda de diversos
hosts conectados na rede.

Requisição fora do browser, usando o comando curl / curl -v. Também passa a fazer a compressão de dados por meio de 
gzip e hpack (ainda mais comprimido) para atender a necessidade de mercado trazida pelo universo dos mobiles. Também 
é adicionada a disposição de dados em forma de binários.

Headers Stateful: no HTTP2 é possível guardar os dados para serem aproveitados futuramente.