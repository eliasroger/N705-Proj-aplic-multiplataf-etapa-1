# 🔌 Especificação de APIs – Meu Lixo

## 🔐 Autenticação
- **Método:** Bearer Token (JWT).  
- **Login:** `POST /api/auth/login`  

Entrada:
```json
{ "email": "usuario@exemplo.com", "senha": "123456" }

Saída (200):
{ "token": "jwt_token...", "usuario": { "id": 1, "nome": "João", "perfil": "morador" } }
