# Configuração

Configure as configurações do seu sistema Live AI.

## Interface Web

1. Acesse a interface web em `http://localhost:8080`
2. Configure suas credenciais do YouTube
3. Defina os parâmetros de streaming
4. Inicie sua transmissão ao vivo com IA!

## Configuração da Chave de API

**🔑 Obtenha sua chave de API em: [https://live.1click.ai/](https://live.1click.ai/)**

1. Visite o site para obter sua chave de API
2. Digite a chave de API na configuração do Live AI
3. Salve suas configurações

## Chave de Transmissão do YouTube

1. Siga o guia [Configuração do YouTube Live](YOUTUBE_LIVE_PT_BR.md)
2. Copie sua chave de transmissão do YouTube Studio
3. Digite a chave de transmissão na configuração do Live AI

## Variáveis de Ambiente

Para instalações Docker, você pode configurar estas variáveis de ambiente:

```yaml
environment:
  - STREAM_AUTO_START=true
  - API_KEY=sua_chave_api_aqui
  - YOUTUBE_STREAM_KEY=sua_chave_transmissao_aqui
```

## Dados Persistentes

Sua configuração é automaticamente salva na pasta `./data` quando usa Docker.

## Próximos Passos

- [Obtendo Sua Chave de API Gratuita](OBTENDO_CHAVE_API.md) - Obtenha sua chave de API
- [Configuração do YouTube Live](YOUTUBE_LIVE_PT_BR.md) - Configure sua transmissão ao vivo
- [Solução de Problemas](TROUBLESHOOTING_PT_BR.md) - Se encontrar algum problema
