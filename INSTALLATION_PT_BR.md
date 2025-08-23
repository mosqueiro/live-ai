# Guia de Instalação

Este guia cobre todos os métodos de instalação do Live AI.

## Navegação

- [← Voltar ao README](README_PT_BR.md)
- [🔑 Obtendo Sua Chave de API Gratuita](OBTENDO_CHAVE_API.md)
- [🎥 Configuração do YouTube Live](YOUTUBE_LIVE_PT_BR.md)
- [⚙️ Configuração](CONFIGURATION_PT_BR.md)
- [🔧 Solução de Problemas](TROUBLESHOOTING_PT_BR.md)

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

## Instalação Docker Apenas

O Live AI agora está disponível exclusivamente via Docker para a melhor experiência e segurança.

## Próximos Passos

Após a instalação, prossiga para:

1. [Obtendo Sua Chave de API Gratuita](OBTENDO_CHAVE_API.md) - Obtenha sua chave de API
2. [Configuração do YouTube Live](YOUTUBE_LIVE_PT_BR.md) - Configure sua transmissão ao vivo
3. [Configuração](CONFIGURATION_PT_BR.md) - Configure as configurações do sistema
