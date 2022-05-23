<h1>Gerenciar carros e locações - FIAP</h1>

<p align="center">
  <img src="http://img.shields.io/static/v1?label=License&message=MIT&color=green&style=for-the-badge"/>
   <img src="http://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=GREEN&style=for-the-badge"/>
</p>

> Status do Projeto: :heavy_check_mark: :warning: (concluido)

### Tópicos

:small_blue_diamond: [Descrição do projeto](#descrição-do-projeto)

:small_blue_diamond: [Funcionalidades](#funcionalidades)

:small_blue_diamond: [Deploy da Aplicação](#deploy-da-aplicação-dash)

:small_blue_diamond: [Pré-requisitos](#pré-requisitos)

:small_blue_diamond: [Como rodar a aplicação](#como-rodar-a-aplicação-arrow_forward)

## Descrição do projeto

Este sistema compôem 3 modulos de um Projeto de Monitoramento de Drones:

- **drone-monitor-job** -> Responsável por enviar de forma simulada 4 drones com informações aleatórias do temperatura e de umidade
- **drone-monitor-producer** -> Responsável por receber dados do drone através do end-point (localhost:8082/api/v1/drones-monitor/drones/register/), validar suas rastreabilidade, e envia para o tópico do Kafka.
- **drone-monitor-consumer** -> Responsável por consumir as mensagens do tópico do kafka e trata-las a sua deserialização e validar as informações do drone, estando dentro das regras de alerta, será enviado um e-mail

## Funcionalidades

#### :heavy_check_mark: **Monitoramento de Informações enviadas de Drones**
- ##### Monitoramento de Informações enviadas de Drones

  - ###### Seleção de drones para recuperar informações
  - ###### Postagema automatizada de informações do drone no end-point do produtor kafka
  - ###### Validar rastreabilidade do drone e serialização dos dados
  - ###### Postar no tópico do kafka
  - ###### Consumir do tópico do kafka
  - ###### Deserializar as informações do drone
  - ###### Validar a regra para envio do alerta
  - ###### Enviar e-mail quando igual ou superior a regra parametrizada

## Tecnologias


- [Android Studio](https://developer.android.com/studio) (IDE)
- [Kotlin](https://kotlinlang.org/)
- [Gradle](https://gradle.org/)
- [RecyclerView](https://developer.android.com/guide/topics/ui/layout/recyclerview)
- [Firebase](https://firebase.google.com)
- [API 21 - Android Lollipop](https://developer.android.com/about/versions/lollipop?hl=pt-br)



## Vídeo-1 Apresentação da Aplicação :dash:

> Link em vídeo da aplicação rodando. https://www.loom.com/share/2cbb9686bbc442de93fa1f238a52d546

## Vídeo-2 Apresentação da Aplicação :dash:

> Link em vídeo-2 da aplicação rodando.  https://www.loom.com/share/1605329bd5e54e60915623a4a59367d5

## Como rodar a aplicação :arrow_forward:

No terminal, clone o projeto:

```
git clone https://github.com/ricardosoareslacerda/loca_autos.git
```

- [Android Studio](https://developer.android.com/studio)
- Iniciar a ide Android Studio
- Abrir o projeto pelo android studio
- Instalar o disposito de emulação adicionando a SDK
- Aguardar a emulação iniciar para utilizar o app

## Desenvolvedores/Contribuintes :octocat:

Liste o time responsável pelo desenvolvimento do projeto
[<br><sub>Ricardo Lacerda</sub>](https://github.com/ricardosoareslacerda) | [<br><sub>Marcos Porto</sub>](https://github.com/maporto) |  [<br><sub>Juscelino Carvalho</sub>](https://github.com/JuscelinoCarvalho) |  [<br><sub>Gabriel Batalha</sub>](https://github.com/GabrielBatalhaDEV) |

## Licença

The [Google Play Licensing](https://developer.android.com/google/play/licensing) (MIT)

Copyright :copyright: Ano - Titulo do Projeto
