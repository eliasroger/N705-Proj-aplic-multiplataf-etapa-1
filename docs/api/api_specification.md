# 🔌 Especificação de APIs – Meu Lixo

## 🔐 Autenticação
- **Método:** Bearer Token (JWT).  
- **Login:** `POST /api/auth/login`  

Entrada:
```json
{ "email": "usuario@exemplo.com", "senha": "123456" }

Saída (200):
{ "token": "jwt_token...", "usuario": { "id": 1, "nome": "João", "perfil": "morador" } }

#📌 Endpoints
1. Horários

GET /api/horarios/{bairro_id} → retorna horários.

POST /api/horarios/atualizar (admin).

2. Feedback

POST /api/feedback → registra horário real.

GET /api/feedback/estatisticas/{bairro_id} → estatísticas de atraso.

3. Denúncias

POST /api/denuncia → cria denúncia com geolocalização.

GET /api/denuncia/{bairro_id} → lista denúncias por bairro.

4. Conteúdo Educativo

GET /api/conteudo → lista conteúdos.

POST /api/conteudo (admin) → cadastra novo conteúdo.

🚦 Códigos de Resposta

200 OK – sucesso

201 Created – recurso criado

400 Bad Request – erro na requisição

401 Unauthorized – falha de autenticação

403 Forbidden – sem permissão

404 Not Found – recurso não encontrado

500 Internal Server Error – erro no servidor

