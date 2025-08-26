# WebScraping-CMD

Scripts para raspagem de conteúdo web via linha de comando, utilizando `curl` e comandos nativos do sistema.

## Descrição

Este repositório contém scripts para automatizar a coleta de informações de páginas web específicas, exibindo os resultados diretamente no terminal. Os exemplos presentes buscam o último login de determinados jogadores na página de ranking do jogo Point Blank (Ongame).

- `busca.bat`: Script para Windows (CMD).
- `busca.sh`: Script para Linux/Mac (Bash).

## Como funciona

Os scripts acessam páginas específicas com `curl`, extraem as informações desejadas usando comandos de filtragem (como `find`, `grep` e `cut`), e formatam a saída no terminal destacando o resultado de cada usuário monitorado.

## Uso

### Windows (CMD)

1. Abra o Prompt de Comando como administrador.
2. Execute o script `busca.bat`:
   ```cmd
   busca.bat
   ```

### Linux/Mac (Bash)

1. Dê permissão de execução ao script:
   ```bash
   chmod +x busca.sh
   ```
2. Execute o script:
   ```bash
   ./busca.sh
   ```

## Dependências

- [curl](https://curl.se/)
- No Linux/Mac, comandos básicos como `grep` e `cut` (já presentes por padrão).

## Exemplo de saída

```
##################################################
########### Ultimo Login no PB ###################
##################################################
## Luffy   21/08/2025 as 19:44  #########
## Perseu  21/08/2025 as 19:32  #########
## Manolo  21/08/2025 as 19:31  #########
## Leozin  21/08/2025 as 19:29  #########
##################################################
```

## Observações

- Os scripts são adaptáveis para outras páginas e informações. Basta alterar as URLs e os filtros conforme necessário.
- Os resultados dependem da estrutura do site. Mudanças no layout do site podem exigir ajustes nos comandos.

## Licença

Este projeto está sob a licença MIT.