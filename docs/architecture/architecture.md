# 🏗️ Arquitetura do Sistema – Meu Lixo

## 📖 Descrição da Arquitetura
A arquitetura do sistema é baseada em três camadas: frontend, backend e persistência de dados.  
O frontend (web e mobile) interage com o backend por meio de uma **API Gateway**.  
O backend é modularizado em serviços (Horários, Feedback, Denúncia, Conteúdo, Notificações).  
A persistência usa bancos híbridos: PostgreSQL (relacional) e MongoDB (não relacional).  

## 🧩 Componentes do Sistema
- **Frontend Web (React):** acesso via navegador.  
- **Aplicativo Mobile (React Native):** acesso mobile com foco em notificações.  
- **API Gateway (Node.js + Express):** central de roteamento e autenticação.  
- **Serviços de Backend:** Horários, Feedback, Denúncia, Conteúdo Educativo, Notificações.  
- **Banco Relacional (PostgreSQL):** usuários, bairros, horários.  
- **Banco Não Relacional (MongoDB):** feedbacks, denúncias, conteúdos multimídia.  
- **Painel Administrativo:** gerência de dados e relatórios.  

## 📐 Padrões Arquiteturais Utilizados
- **Arquitetura em Camadas (Layered).**  
- **RESTful APIs.**  
- **Event-Driven (para notificações).**  
- **Containerização (Docker + Kubernetes).**  
- **Segurança com JWT e HTTPS.**  

## 📊 Diagrama da Arquitetura
![Diagrama de Arquitetura](../../images/meu_lixo_arquitetura.png)
<img width="1320" height="472" alt="meu_lixo_arquitetura" src="https://github.com/user-attachments/assets/675bc1af-5916-4bb1-8587-98d08523fb97" />

## ⚙️ Decisões Técnicas e Justificativas
- **Node.js + Express:** alta performance e suporte a APIs escaláveis.  
- **React + React Native:** reutilização de componentes e multiplataforma.  
- **PostgreSQL + MongoDB:** balanceia consistência e flexibilidade.  
- **Docker + Kubernetes:** garante escalabilidade e portabilidade.  
- **Firebase Cloud Messaging:** envio de notificações em tempo real.  
