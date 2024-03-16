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
* 

---
## Materiais para Estudo

* [**PODCAST**: MONOLITOS](https://www.alura.com.br/podcast/hipsterstech-monolitos-hipsters-173-a395?_gl=1*16icx73*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjA2OTAuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
* [**CURSO**: CLOUD ONBOARDING](https://www.alura.com.br/curso-online-cloud-onboarding-trabalhando-principais-provedores?_gl=1*w02f89*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjA2OTAuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
* [**POSCAST**: HISTÓRIAS DO CLOUD](https://www.alura.com.br/podcast/hipsterstech-historias-do-cloud-hipsters-04-a582?_gl=1*w02f89*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjA2OTAuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
* [**CURSO**: GIT E GITHUB](https://www.alura.com.br/curso-online-git-github-controle-de-versao?_gl=1*r2iwzn*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjA2OTAuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
* [**PODCAST**: MICROSSERVIÇOS](https://www.alura.com.br/podcast/hipsterstech-microservicos-hipsters-17-a569?_gl=1*r2iwzn*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjA2OTAuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
* [**CURSO**: ESCALANDO EQUIPES ÁGEIS](https://www.alura.com.br/curso-online-escalando-equipes-ageis-v2?_gl=1*4fa3rt*_ga*ODM1Nzk2OTUyLjE2OTgzNDc1Mjk.*_ga_1EPWSW3PCS*MTcxMDYxNzYwOC41Ni4xLjE3MTA2MjEwMTUuMC4wLjA.*_fplc*dkx1VjQ0TVc5UVZySVdrTkV3ZVA1dVhjSDB0TW0wTk5Gd3lvMGN3NVRuem1BVDFOTWU2eEElMkIxamtaY3M4dTI2MTJMMWE3eXdQRjhWbXJSbm1wMHBzTXBBc1ZhSVN0Q2JrMmZJVnFLTW5KN1kzTnRwVjc1UktLVGtueWp3eXclM0QlM0Q.)
