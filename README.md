# Giropops Status
O **Giropops Status** é uma aplicação web Python/Flask + Redis que monitora a saúde de serviços HTTP: cadastra endpoints, dispara health checks, armazena histórico e expõe métricas no formato Prometheus. Um dashboard simples mostra o status em tempo real.

## Roadmap

O objetivo desse repositório é provisionar a infraestrutura da aplicação em 4 etapas

| Fase | Foco |
|:---:|---|
| 1 | Rodar a aplicação manualmente em um servidor Linux real (fase atual) |
| 2 | Empacotar em containers |
| 3 | Infraestrutura como código |
| 4 | Produção em cloud |

## O que já foi feito
- [x] VM local criada no VirtualBox (ou UTM) com Ubuntu Server LTS
- [x] EC2 t2.micro provisionada na AWS
- [x] Key pair SSH criada
- [x] `~/.ssh/config` com aliases para `vm` e `ec2`
- [x] `ssh-copy-id` funcionando nos dois ambientes
- [x] `rsync` testado entre as máquinas
- [x] Estrutura `/opt/giropops-status/{app,logs,config,backups}` criada nos dois ambientes
- [x] Código transferido para `/opt/giropops-status/app/` via `rsync`
