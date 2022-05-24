# BugLess

Sistema para mapeamento de casos de dengue na região.

  <img src="https://img.shields.io/badge/status-em%20desenvolvimento-green" alt="Status: Em Desenvolvimento">  <img src="https://img.shields.io/github/license/more-devs-2-blu/bugless" alt="Licença: MIT">

## Índice 

* [Índice](#índice)
* [Descrição do Projeto](#descrição-do-projeto)
* [Requisitos](#requisitos)
* [Orientações técnicas](#orientações-técnicas)
* [Funcionalidades e Demonstração da Aplicação](#funcionalidades-e-demonstração-da-aplicação)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
* [Desenvolvedores](#desenvolvedores)
* [Licença](#licença)
* [Conclusão](#conclusão)


## Motivação

  Mapear os casos de dengue na região, como solução para o Hackathon do programa [+Devs2Blu](https://www.devs2blu.com.br/) realizado pela [Proway](https://www.proway.com.br) e apoiado pelas empresas:. <br> 
  
  * [DBR](https://www.dbrsa.com.br/)
  * [Govbr](https://www.govbr.com.br/)
  * [Mindera](https://mindera.com/)
  * [Philips](https://www.philips.com.br/)
  
## Descrição do projeto

  <p>Aplicação web para cadastros de casos positivos de dengue nos postos de saúde e ambulatórios gerais.
  Os cadastros serão efetuados por funcionários agentes de saúde previamente autenticados no sistema.
  O cadastro irá conter nome, sexo, idade e endereço do paciente, bem como a data do teste.
  A partir do endereço, vamos obter a localização geográfica para sinalizar os casos acumulados no mapa.</p>
  
  Exemplo de uso:<br>
  [![Video-220524115921.gif](https://i.postimg.cc/x8CvPGyY/Video-220524115921.gif)](https://postimg.cc/YG5LrWsy)
  
## Requisitos

Funcionais:

* RF01: Cadastro de caso com paciente
* RF02: Mostrar o número de casos por bairro.
* RF03: Integração com Google Maps API.
* RF04: Mostrar o mapa da cidade sinalizando os bairros com maior incidência.

Não funcionais: 

* RN01: Autenticação por login
* RN02: Validação via BeanValidator @CPF
* RN03: Consulta de API viacep.com.br/ws
  
## Orientações Técnicas

No arquivo 'BugLess\front-BugLess\node_modules\@agm\core\lib\services\google-maps-api-wrapper.d.ts' é necessário comentar ou excluir a linha com o conteúdo:<br> 'subscribeToMapEvent<N extends keyof google.maps.MapHandlerMap>(eventName: N): Observable<google.maps.MapHandlerMap[N]>;'

No arquivo 'BugLess\front-BugLess\node_modules\@agm\core\lib\services\managers\marker-manager.d.ts' é necessário comentar ou excluir a linha com o conteúdo:<br>
  'createEventObservable<T extends (google.maps.MouseEvent | void)>(eventName: google.maps.MarkerMouseEventNames | google.maps.MarkerChangeOptionEventNames, marker: AgmMarker): Observable<T>;'
  
## Funcionalidades e Demonstração da Aplicação

> :construction: Projeto em construção :construction:

## Desenvolvedores
 
| <img src="https://avatars.githubusercontent.com/u/94122439?v=4" width=115><br><sub>[Alessandro B. Ferreira](https://github.com/alessandrobferreira)</sub><br><sub>[Linkedin](https://www.linkedin.com/in/alessandro-ferreira-a9199a115/)</sub> |<img src="https://avatars.githubusercontent.com/u/83621544?v=4" width=115><br><sub>[André F. Schwanz](https://github.com/Andre121193)</sub><br><sub>[Linkedin](https://www.linkedin.com/in/andr%C3%A9-schwanz-241a51216/)</sub> |<img src="https://avatars.githubusercontent.com/u/60515470?v=4" width=115><br><sub>[Douglas Lima da Luz](https://github.com/douglaslimaluz)</sub><br><sub>[Linkedin](https://www.linkedin.com/in/douglas-lima-da-luz-82895a19b/)</sub> |<img src="https://avatars.githubusercontent.com/u/79611444?v=4" width=115><br><sub>[José A. Klaumann](https://github.com/JoseKlaumann)</sub><br><sub>[Linkedin](https://www.linkedin.com/in/jos%C3%A9-augusto-klaumann-5258b6178/)</sub> |<img src="https://avatars.githubusercontent.com/u/5782250?v=4" width=115><br><sub>[Juliano H. S. Vieira](https://github.com/jucabnu)</sub><br><sub>[Linkedin](https://www.linkedin.com/in/juliano-h-vieira/)</sub> |<img src="https://avatars.githubusercontent.com/u/89278356?v=4" width=115><br><sub>[Luan L. G. Lima](https://github.com/LordeLuan)</sub><br><sub>[Linkedin](https://www.linkedin.com/in/luan-lordello-69aa58196/)</sub> |
| :---: | :---: | :---: | :---: | :---: | :---: |

## Tecnologias Utilizadas

<div style="display: inline_block"> 
  <img align="center" alt="Java" height="40" width="30" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg">   
  <img align="center" alt="logo spring" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg" />
  .
  <img align="center" alt="logo Angular" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-original.svg" />
  <img align="center" alt="typescript" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" />  
  <img align="center" alt="Html5" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg">
  <img align="center" alt="Css3" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg">    
  <img align="center" alt="logo bootstrap" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-plain.svg" />
  <img align="center" alt="javascript" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" />
  .  
  <img align="center" alt="Mysql" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-plain.svg">       
  <img align="center" alt="Git" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg">       
 </div> 
  
## Licença
  
  BugLess é [MIT licensed](./LICENSE).
  
  BugLess é licenciado pelo MIT. A documentação do BugLess (por exemplo, arquivos .md na pasta ./docs) é licenciada pelo [Creative Commons licensed](./LICENSE-docs).
 
## Conclusão

> :construction: Projeto em construção :construction:
