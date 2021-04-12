# POC Sigo

Aqui estão algumas informações e detalhes da POC SIGO.

# Repositórios

As aplicações da POC SIGO podem ser encontradas nos seguintes repositórios:

- Aplicação de frontend: [https://github.com/glaubercezar/sigo-web](https://github.com/glaubercezar/sigo-web)
- Microsserviço API Gateway: [https://github.com/glaubercezar/sigo-api-gateway](https://github.com/glaubercezar/sigo-api-gateway)
- Microsserviço de gestão: [https://github.com/glaubercezar/sigo-gestao](https://github.com/glaubercezar/sigo-gestao)
- Microsserviço de normas: [https://github.com/glaubercezar/sigo-normas](https://github.com/glaubercezar/sigo-normas)

# SendGrid

O serviço de gestão está configurado para acionar o serviço externo SendGrid para o envio de emails de alertas.

# Google Cloud

A POC utiliza a plataforma Goolge Cloud para cumprir com os requisitos de Disponibilidade, Escalabilidade, etc.

## Google Cloud Run

A aplicação de frontend é implantada no ambiente Cloud Run, com deploy automatizado através do Cloud Build a cada push de commits para a branch master.

## Google Cloud App Engine

Os microsserviços estão configurados para o ambiente App Engine standard, com isso as instâncias são criadas e executadas conforme a demanda.

### Deploy via command line:
Com o Google Cloud SDK através da CLI as aplicações são criadas e implantadas facilmente:

```sh
gcloud app deploy
```

