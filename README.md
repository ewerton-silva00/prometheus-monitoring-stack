# Stack de Monitoramento - Docker Compose

Este projeto consiste em prover um ambiente local de estudo das ferramentas abaixo:

**Componentes Base**:

- [`Prometheus`](https://prometheus.io/)
- [`AlertManager`](https://prometheus.io/docs/alerting/latest/alertmanager/)
- [`Grafana`](https://grafana.com/oss/grafana/)
- [`Grafana Loki`](https://grafana.com/oss/loki/)
- [`Grafana Promtail`](https://grafana.com/docs/loki/latest/clients/promtail/)

**Componentes Auxiliares**:

- [`cAdvisor`](https://github.com/google/cadvisor)
- [`Node Exporter`](https://github.com/prometheus/node_exporter)
- [`Karma`](https://github.com/prymitive/karma)

## Pré-requisitos

- [`Docker Engine`](https://docs.docker.com/engine/install/)
  - Estou usando a versão `20.10.11`.
- [`Docker Compose`](https://docs.docker.com/compose/install/)
  - Estou usando a versão `1.29.2`.

## Ferramentas Auxiliares (Opcionais)

- [`LogCLI`](https://grafana.com/docs/loki/latest/getting-started/logcli/)
- [`Pint`](https://github.com/cloudflare/pint)

## Como usar este projeto

Baixe este repositório conforme mostrado abaixo:
```bash
git clone https://github.com/ewerton-silva00/monitoring-stack.git
```

Acesse o diretório `monitoring-stack` e e execute o comando abaixo:
```bash
docker-compose up --detach
```

A partir disso todos os containers da stack serão inicializados e dentro de poucos segundos estão acessíveis via browser.

__Importante!__ Explore os arquivos de configurações para entender todo o cenário.

Bons estudos!

## Como acessar os serviços via browser

- `Prometheus`: [http://localhost:9090](http://localhost:9090)
- `AlertManager`: [http://localhost:9093](http://localhost:9093)
- `Grafana`: [http://localhost:3000](http://localhost:3000)
- `Grafana Loki`: [http://localhost:3100](http://localhost:3100)
- `Grafana Promtail`: [http://localhost:9080](http://localhost:9080)
- `Karma`: [http://localhost:8080](http://localhost:8080)
