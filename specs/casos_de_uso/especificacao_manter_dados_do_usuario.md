| Caso de uso       | Manter dados do usuário                            |
|-------------------|----------------------------------------------------|
| Objetivo          | Permitir ao usuário alterar informações como telefone, e-mail e e-mail de recuperação. |
| Requisitos        | **[RF400]**                                        |
| Atores            | Usuário                                            |
| Condição de entrada | O usuário está autenticado no sistema e acessa o menu de perfil. |
| Fluxo principal   | 1. O sistema exibe os dados atuais do usuário.<br>2. O usuário edita os campos desejados.<br>3. O sistema valida os dados inseridos.<br>4. O sistema atualiza os dados no banco e exibe mensagem de sucesso. |
| Fluxos alternativos | Nenhum                                           |
| Fluxos de exceção | O sistema exibe mensagem de erro caso os dados inseridos sejam inválidos. |
