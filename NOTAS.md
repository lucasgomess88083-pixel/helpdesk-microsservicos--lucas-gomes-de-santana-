# Notas da Etapa 0

| Parte | Arquivos | Destino |
|---|---|---|
| Usuários | app/usuarios/* | serviço Usuários |
| Login e token | app/auth/* | serviço Usuários (emite JWT) |
| Validação do token | app/auth/dependencias.py, tokens.py | copiada nos 3 serviços |
| Inventário (tabela ativos) | app/inventario/* | serviço Inventário |
| Chamados | app/chamados/* | serviço Chamados |
| Notificações | app/notificacoes/* | bônus |
| Tela | app/web/* | gateway/static |

## FKs entre módulos (a remover)
- chamados.ativo_id -> ativos.id (Inventário)
- comentarios.autor_id -> usuarios.id (Usuários)
