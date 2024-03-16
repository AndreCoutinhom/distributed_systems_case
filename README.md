---

![image](https://github.com/AndreCoutinhom/distributed_systems_case/assets/91290799/70eb3864-7934-43ab-bd7b-424d0df47abe)

---
### Tópicos:
> Cloud
>
> DevOps
> 
> GitHub
>
> Heroku
>
> LayerCI
>
> Metabase
>
> Programação
>
> Sentry
---
Boas-vindas ao AluraCases! Aqui você acompanha as principais tomadas de decisões de grandes equipes de desenvolvimento das maiores empresas de tecnologia do Brasil e do mundo.

Prepare-se para mergulhar em mais um case incrível! Vá para um ambiente calmo, respire fundo e vamos lá:

A maioria das empresas que conhecemos começaram com objetivos, tecnologias e decisões que, ao longo do caminho, foram mudando. Seja por mudanças no mercado, crescimento do negócio, aumento da concorrência ou até mesmo dificuldade para escalar um serviço que cresceu muito.

Neste case trazemos o Fabricio Buzeto, que é doutor em computação, CEO e CTO da BXBlue, um marketplace de crédito consignado.

Fabricio nos conta como foi o processo de evolução de um monolito para um sistema distribuído, explicando desde a tomada de decisão, erros e acertos, até os resultados que conseguiram a partir disso.

---
* A BXBlue começou como monolito e foi aplicando sistemas distribuídos através de arquitetura em cloud.

---
![image](https://github.com/AndreCoutinhom/distributed_systems_case/assets/91290799/027850b7-48c7-4b44-b739-e407117452a1)

* As features foram aos poucos implementadas aproveitando o que já havia sido construído. Ainda há componentes do sistema que permanecem os mesmos.

---
![image](https://github.com/AndreCoutinhom/distributed_systems_case/assets/91290799/e7e5156b-d3b3-4758-be11-7c1c90117210)

* O processamento que se tornou mais pesado, fez com que a BXBlue alterasse seu desenvolvimento com funções assíncronas de cálculo. Então o Rails já não rodava todos os cálculos sozinho.

---
### Vantagens de se usar um monolito

* Simples de desenvolver;
* Simples para testar;
* Simples de lançar;
* Simples de reutilizar;
* Simples de escalar (só não se sabe até onde).

---
### Dificuldades de se usar um monolito

* Escala de testes;
* Escala de times;
* Escala de deploy;
* Escala de stack;
* Escala de mudanças.

---
![image](https://github.com/AndreCoutinhom/distributed_systems_case/assets/91290799/bc1970cc-d839-4e52-8d6e-f0f60f9acfb0)

* O mapeamento de bases carentes de automação está fortemente ligado às possíveis irregularidades de performance monolítica por vários programadores. No geral, são formas de deixar os times mais adeptos a dados coesos e performance fluida.

---
![image](https://github.com/AndreCoutinhom/distributed_systems_case/assets/91290799/9a42c24e-ba3b-4274-b593-ed7b9490d48e)

* A BXBlue usou várias ferramentas próprias do framework Rails.

---
* Quando muitas responsabilidades são atribuídas a um monolito, isso pode se tornar um problema.

---
### Fatores comuns de influência para mudança (BXBlue)

* Tempo de build;
* Tempo de deploy;
* Número de acessos;
* Contexto do time;
* Rastreabilidade.

---
### Outras formas de sistema distribuído

* Micro-serviços;
* Citadel;
* Macroserviços;
* **Stonehenge**.

---
![image](https://github.com/AndreCoutinhom/distributed_systems_case/assets/91290799/ac381c1b-9239-4509-8193-2d592457d75e)

* O Stonehenge basicamente integra vários monolitos. A BXBlue percebeu que apesar de não usar muitos microsserviços, os monolitos eram bastante auto contidos.

![image](https://github.com/AndreCoutinhom/distributed_systems_case/assets/91290799/c7f29a53-c0cf-4ce2-9169-5f621133f1c8)

* Por isso, as novas necessidades foram acomodadas em pequenos monolitos.

---
## Materiais para Estudo

* [**PODCAST**: MONOLITOS](https://www.alura.com.br/podcast/hipsterstech-monolitos-hipsters-173-a395?_gl=1*16icx73*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjA2OTAuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
* [**CURSO**: CLOUD ONBOARDING](https://www.alura.com.br/curso-online-cloud-onboarding-trabalhando-principais-provedores?_gl=1*w02f89*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjA2OTAuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
* [**POSCAST**: HISTÓRIAS DO CLOUD](https://www.alura.com.br/podcast/hipsterstech-historias-do-cloud-hipsters-04-a582?_gl=1*w02f89*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjA2OTAuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
* [**CURSO**: GIT E GITHUB](https://www.alura.com.br/curso-online-git-github-controle-de-versao?_gl=1*r2iwzn*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjA2OTAuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
* [**PODCAST**: MICROSSERVIÇOS](https://www.alura.com.br/podcast/hipsterstech-microservicos-hipsters-17-a569?_gl=1*r2iwzn*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjA2OTAuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
* [**CURSO**: ESCALANDO EQUIPES ÁGEIS](https://www.alura.com.br/curso-online-escalando-equipes-ageis-v2?_gl=1*4fa3rt*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjEwMTUuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
