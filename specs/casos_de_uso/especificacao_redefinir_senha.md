| Caso de uso       | Redefinir senha                                    |
|-------------------|----------------------------------------------------|
| Objetivo          | Permitir ao usuário redefinir sua senha.           |
| Requisitos        | **[RF416]**                                        |
| Atores            | Usuário                                            |
| Condição de entrada | O usuário acessa a opção "Esqueci minha senha" na tela de login. |
| Fluxo principal   | 1. O sistema solicita o e-mail de recuperação.<br>2. O usuário informa o e-mail.<br>3. O sistema envia um link de redefinição.<br>4. O usuário acessa o link e define uma nova senha.<br>5. O sistema salva a nova senha e confirma a alteração. |
| Fluxos alternativos | Nenhum                                           |
| Fluxos de exceção | O sistema exibe erro caso o e-mail não esteja cadastrado. |
