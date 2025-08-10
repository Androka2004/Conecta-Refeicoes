| Caso de uso       | Confirmar recebimento de refeição pelos colaboradores |
|-------------------|-------------------------------------------------------|
| Objetivo          | Permitir ao gestor de obra registrar no sistema a confirmação de recebimento da refeição pelos colaboradores da obra. |
| Requisitos        | **[RF208]**                                            |
| Atores            | Gestor de obra                                        |
| Condição de entrada | O gestor de obra acessa a seção de controle de refeições da obra. |
| Fluxo principal   | 1. O gestor seleciona o colaborador ou a lista de colaboradores.<br>2. O gestor indica a refeição recebida (ex.: almoço, jantar).<br>3. O sistema registra a confirmação de recebimento.<br>4. O sistema atualiza o status da refeição para “Recebida”.<br>5. O sistema exibe mensagem de confirmação ao gestor. |
| Fluxos alternativos | 1A. Se o colaborador não estiver na lista, o gestor pode pesquisar manualmente e adicionar ao registro.<br>1B. O gestor pode confirmar todas as refeições de uma vez (confirmação em lote). |
| Fluxos de exceção | O sistema informa erro se não houver conexão ou se o registro não puder ser salvo. |
