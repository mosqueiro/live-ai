# Guia de Instalação

Este guia cobre todos os métodos de instalação do Live AI.

## Instalação Docker (Recomendado)

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

Na seção [Releases](https://github.com/mosqueiro/live-ai/releases) você encontrará 3 versões executáveis:

- **macOS**: Binário executável para macOS
- **Linux**: Binário executável para Linux
- **Windows**: Executável `.exe` para Windows

**Versão Docker**: Disponível no repositório através do arquivo `docker-compose.yml` (Recomendado)

A versão Docker é a mais recomendada pois oferece isolamento completo e configuração automática dos volumes persistentes.

## Downloads

Arquivos executáveis estão disponíveis na seção [Releases](https://github.com/mosqueiro/live-ai/releases) para download direto.

## Próximos Passos

Após a instalação, prossiga para:

1. [Obtendo Sua Chave de API Gratuita](OBTENDO_CHAVE_API.md) - Obtenha sua chave de API
2. [Configuração do YouTube Live](YOUTUBE_LIVE_PT_BR.md) - Configure sua transmissão ao vivo
3. [Configuração](CONFIGURATION_PT_BR.md) - Configure as configurações do sistema
