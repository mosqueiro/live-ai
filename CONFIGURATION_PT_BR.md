# Configuração

Configure as configurações do seu sistema Live AI.

## Navegação

- [← Voltar ao README](README_PT_BR.md)
- [🔑 Obtendo Sua Chave de API Gratuita](OBTENDO_CHAVE_API.md)
- [📖 Guia de Instalação](INSTALLATION_PT_BR.md)
- [🎥 Configuração do YouTube Live](YOUTUBE_LIVE_PT_BR.md)
- [🔧 Solução de Problemas](TROUBLESHOOTING_PT_BR.md)

## Interface Web

A interface web em `http://localhost:8080` serve para você gerenciar o streaming ou enviar arquivos.

**Importante**: Todas as configurações devem ser feitas em [https://live.1click.ai/](https://live.1click.ai/)

### Gerenciador de Streaming

O gerenciador de streaming roda via web na porta 8080 onde o instalador estiver rodando.

#### Funcionalidades:

- **Interface Visual Fácil**: Interface web simples e intuitiva
- **Configurações do Locutor**: Veja as configurações do locutor como ele vai se comportar
- **Mídia de Fundo**: Mude as músicas ou vídeos de fundo que ficam girando na live
- **Acompanhamento de Mensagens**: Acompanhe as mensagens que chegam de doação através do QR code da sua live

![Interface do Gerenciador de Streaming](images/webui/1.png)

![Configuração do Locutor](images/webui/2.png)

![Gerenciamento de Mídia de Fundo](images/webui/3.png)

![Monitoramento de Mensagens](images/webui/4.png)

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
