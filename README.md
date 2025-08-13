# sqlserver-mcp-dotnet-tool-scripts
Exemplo de uso do MCP do SQL Server (via dotnet tool) com um server de banco de dados containerizado e com consulta a dados de regiões do Brasil. Inclui Docker Compose para criação do ambiente de testes.

Um pouco mais sobre o MCP Server do SQL Server:
- [**Anúncio no blog oficial**](https://devblogs.microsoft.com/azure-sql/introducing-mssql-mcp-server/)
- [**Instruções de uso da versão criada em .NET 8**](https://github.com/Azure-Samples/SQL-AI-samples/blob/main/MssqlMcp/dotnet/README.md)

Criei uma versão deste MCP que pode ser instalada como uma .NET Global Tool e que foi publicada no NuGet. Basta apenas executar a instrução a seguir em Windows, Linux ou macOS, em um ambiente que conte pelo menos com o .NET 8 previamente instalado

```bash
dotnet tool install --global mcpsqlserver-preview-202508d --version 1.0.0
```

O comando a seguir mostrará se a ferramenta foi corretamente instalada:

```bash
dotnet tool list -g
```

Como podemos observar no resultado seguinte:

```
ID do Pacote                      Versão      Comandos
----------------------------------------------------------
mcpsqlserver-preview-202508d      1.0.0       mcpsqlserver
```

