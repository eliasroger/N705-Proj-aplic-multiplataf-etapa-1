# 🗄 Modelo de Dados – Meu Lixo

## 📖 Descrição Geral
O sistema utiliza abordagem híbrida:  
- **PostgreSQL:** dados estruturados e críticos (usuários, bairros, horários).  
- **MongoDB:** dados dinâmicos e colaborativos (feedbacks, denúncias, conteúdos).  

## 🧩 Entidades Relacionais (PostgreSQL)
- **Usuário:** id, nome, email, senha_hash, perfil, bairro_id.  
- **Bairro:** id, nome, horário_oficial.  
- **Horário Previsto:** id, bairro_id, horário_previsto, ultima_atualizacao.  

## 🗂 Entidades Não Relacionais (MongoDB)
- **Feedback:** bairro_id, usuario_id, horario_real, data_registro.  
- **Denúncia:** usuario_id, bairro_id, descricao, coordenadas, data_registro.  
- **Conteúdo Educativo:** titulo, categoria, url, data_publicacao.  

## 📊 Diagrama ER
Usuário (1) ─── (N) Feedback
Usuário (1) ─── (N) Denúncia
Bairro (1) ─── (N) Horário Previsto


## 📘 Dicionário de Dados
| Entidade | Atributo | Tipo | Descrição |
|----------|----------|------|-----------|
| Usuário | id | INT (PK) | Identificador único |
| Usuário | nome | VARCHAR | Nome do usuário |
| Usuário | email | VARCHAR | E-mail único |
| Usuário | senha_hash | VARCHAR | Senha criptografada |
| Usuário | perfil | ENUM | Morador, Admin, Cooperativa |
| Bairro | id | INT (PK) | Identificador único |
| Bairro | nome | VARCHAR | Nome do bairro |
| Bairro | horario_oficial | TIME | Horário oficial da coleta |
| Horário Previsto | id | INT (PK) | Identificador único |
| Horário Previsto | horario_previsto | TIME | Horário estimado |
| Horário Previsto | ultima_atualizacao | TIMESTAMP | Última atualização |
