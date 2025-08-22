# Live AI - Streaming Inteligente do YouTube

Live AI é um software inovador de streaming do YouTube que usa inteligência artificial para automatizar e otimizar suas transmissões ao vivo.

**🔑 Obtenha sua chave de API em: [https://live.1click.ai/](https://live.1click.ai/)**

## Funcionalidades

- 🤖 **Integração com IA**: Usa inteligência artificial para melhorar a qualidade do streaming
- 📹 **Streaming Automático**: Transmissão automatizada para o YouTube
- 💾 **Dados Persistentes**: Configurações e dados salvos automaticamente
- 🐳 **Pronto para Docker**: Instalação e execução fácil com Docker

## Instalação Docker

### Pré-requisitos

- Docker e Docker Compose instalados

### Execução

1. Clone o repositório:

```bash
git clone https://github.com/mosqueiro/live-ai.git
cd live-ai
```

2. Execute com Docker Compose:

```bash
docker-compose up -d
```

O serviço estará disponível em `http://localhost:8080`

### ⚠️ **MUITO IMPORTANTE: Volumes Persistentes**

**⚠️ ATENÇÃO: Se você não configurar os volumes persistentes, TODOS os seus dados serão perdidos quando o container for reiniciado!**

Os dados da aplicação são salvos na pasta `./data` do host, mapeada para `/app/data` no container, garantindo que suas configurações sejam mantidas mesmo após reinicializações.

**Por que é crucial:**

- Sem volumes persistentes, suas configurações do YouTube serão perdidas
- Seus dados de streaming e histórico serão apagados
- Você precisará reconfigurar tudo novamente a cada reinicialização

## Downloads

Arquivos executáveis estão disponíveis na seção [Releases](https://github.com/mosqueiro/live-ai/releases) para download direto.

## Configuração

1. Acesse a interface web em `http://localhost:8080`
2. Configure suas credenciais do YouTube
3. Defina os parâmetros de streaming
4. Inicie sua transmissão ao vivo com IA!

## Instalação por Sistema Operacional

### Instalação macOS

1. Baixe e extraia o arquivo ZIP
2. Abra o Terminal e navegue até a pasta extraída
3. Execute: `./live-ai`

**Nota**: Os binários são assinados e notarizados pelo desenvolvedor para segurança.

### Instalação Linux

1. Baixe e extraia o arquivo ZIP
2. Abra o Terminal e navegue até a pasta extraída
3. Execute: `./live-ai`

**Nota**: Certifique-se de que o arquivo tem permissões de execução. Se necessário, execute: `chmod +x live-ai`

### Instalação Windows

1. Baixe e extraia o arquivo ZIP
2. Clique duas vezes em `live-ai.exe` ou execute pelo Prompt de Comando

## Versões Disponíveis

Na seção [Releases](https://github.com/mosqueiro/live-ai/releases) você encontrará 4 versões diferentes:

- **Docker** (Recomendado): Use o `docker-compose.yml` para instalação mais fácil e isolada
- **macOS**: Binário executável para macOS
- **Linux**: Binário executável para Linux
- **Windows**: Executável `.exe` para Windows

A versão Docker é a mais recomendada pois oferece isolamento completo e configuração automática dos volumes persistentes.

## Suporte

Para suporte e dúvidas, abra uma issue no repositório GitHub.

## Licença

Este projeto está licenciado sob a Licença MIT.
