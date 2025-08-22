# Solução de Problemas

Problemas comuns e soluções para o Live AI.

## Problemas Comuns

### Serviço Não Inicia

**Problema**: O serviço não inicia ou não está acessível.

**Soluções**:

1. Verifique se o Docker está rodando
2. Confirme se a porta 8080 não está em uso
3. Verifique os logs do Docker: `docker-compose logs live-ai`

### Perda de Dados

**Problema**: Configurações e dados são perdidos após reinicialização.

**Soluções**:

1. Certifique-se de que os volumes persistentes estão configurados corretamente
2. Verifique se a pasta `./data` existe e tem permissões adequadas
3. Confirme o mapeamento de volume no `docker-compose.yml`

### Problemas com Chave de API

**Problema**: Chave de API não funciona ou é inválida.

**Soluções**:

1. Verifique sua chave de API em [https://live.1click.ai/](https://live.1click.ai/)
2. Confirme se a chave de API foi digitada corretamente
3. Certifique-se de que a chave de API tem permissões adequadas

### Problemas com Transmissão do YouTube

**Problema**: Não consegue conectar ao YouTube ou a transmissão falha.

**Soluções**:

1. Verifique se sua chave de transmissão do YouTube está correta
2. Confirme se a transmissão está programada e habilitada
3. Certifique-se de que o início automático está habilitado no YouTube Studio

## Obtendo Ajuda

Se você continuar enfrentando problemas:

1. Verifique o guia de [Configuração](CONFIGURATION_PT_BR.md)
2. Revise o guia de [Instalação](INSTALLATION_PT_BR.md)
3. Abra uma issue no repositório GitHub

## Logs

Para visualizar os logs do sistema:

```bash
# Logs do Docker
docker-compose logs live-ai

# Acompanhar logs em tempo real
docker-compose logs -f live-ai
```
