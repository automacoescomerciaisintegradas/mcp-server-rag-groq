# Configuração do DataButton MCP para Claude App

Este guia ajudará você a configurar o [DataButton MCP](https://databutton.com/mcp) para uso com o Claude App no Windows.

## Pré-requisitos

- Claude App instalado no seu computador
- Node.js v18+ instalado (opcional, já que estamos usando uvx)

## O que é o DataButton MCP?

O DataButton MCP permite que o Claude App interaja com suas ferramentas personalizadas e dados por meio do protocolo MCP (Model Context Protocol). Isso permite que:

- Claude interaja com suas aplicações criadas no DataButton
- Execute tarefas personalizadas
- Acesse APIs e ferramentas específicas

## Como configurar

1. **Execute o script PowerShell como administrador**

   Clique com o botão direito no arquivo `configurar_claude_databutton.ps1` e selecione "Executar como administrador".

   Este script irá:
   - Criar o diretório para o Claude App se não existir
   - Copiar o arquivo de configuração para o local correto
   - Adicionar o diretório do uvx ao PATH do sistema

2. **Reinicie o Claude App**

   Feche e reabra o Claude App para que as mudanças façam efeito.

3. **Verifique a integração**

   Ao abrir o Claude App, você deve ver uma indicação de que o DataButton MCP está disponível.

## Resolução de problemas

Se o DataButton MCP não aparecer no Claude App:

1. Verifique se o script foi executado com sucesso
2. Confirme que o arquivo `claude_desktop_config.json` está no diretório correto
3. Confirme que o arquivo `api_key.txt` contém sua chave da API DataButton
4. Reinicie o computador para garantir que as mudanças no PATH sejam aplicadas

## Mais informações

Para mais informações sobre o DataButton MCP, visite:
- [Documentação do DataButton MCP](https://docs.databutton.com/databutton-mcp-build-tools-for-ai)
- [Repositório do DataButton App MCP](https://github.com/databutton/databutton-app-mcp) 
