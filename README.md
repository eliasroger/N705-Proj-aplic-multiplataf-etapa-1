# N705-Proj-aplic-multiplataf-etapa-1- "MEU LIXO"
# 📘 Projeto Meu Lixo

## 📖 Descrição do Projeto
O projeto **Meu Lixo** é uma aplicação multiplataforma (disponível em versão web e mobile) criada com o objetivo de apoiar a gestão de resíduos sólidos urbanos e melhorar a comunicação entre a população e os órgãos responsáveis pela coleta.  

A iniciativa busca fornecer informações precisas sobre os horários oficiais de coleta de lixo em diferentes bairros, permitir que os moradores registrem feedbacks sobre atrasos ou ocorrências, além de disponibilizar um canal direto para denúncias de pontos de descarte irregular.  

O sistema também oferece conteúdos educativos voltados para a reciclagem e boas práticas de descarte. Dessa forma, a solução contribui diretamente para o cumprimento da **ODS 11 – Cidades e Comunidades Sustentáveis**, auxiliando na construção de cidades mais organizadas, limpas e conscientes.

---

## 🚨 Problema Abordado e Justificativa
Nas cidades brasileiras, incluindo Fortaleza, o gerenciamento de resíduos enfrenta sérios desafios.  

Entre eles estão:
- A falta de informações claras para a população sobre os horários de coleta.  
- A ocorrência frequente de atrasos.  
- A existência de pontos de descarte irregular, que comprometem a saúde pública e o meio ambiente.  

A ausência de ferramentas tecnológicas integradas limita o envolvimento da população na resolução desses problemas.  

O sistema **Meu Lixo** surge para preencher essa lacuna, promovendo transparência, colaboração entre cidadãos e poder público, e fomentando práticas sustentáveis de descarte de resíduos.

---

## 🎯 Objetivos do Sistema
- Fornecer informações atualizadas sobre os horários de coleta por bairro.  
- Notificar automaticamente os moradores sobre a aproximação da coleta em sua região.  
- Permitir o registro de feedbacks por parte dos usuários, como atrasos na coleta ou ocorrências.  
- Oferecer um canal para denúncias de pontos de lixo irregular, utilizando geolocalização.  
- Disponibilizar conteúdos educativos relacionados à reciclagem, reutilização e descarte adequado.  
- Fornecer ferramentas de monitoramento e gestão para órgãos públicos e cooperativas.  
- Promover o engajamento da comunidade na gestão sustentável dos resíduos sólidos.  

---

## 📌 Escopo do Projeto
**Inclui:**  
- Consulta de horários oficiais de coleta.  
- Registro colaborativo de feedbacks.  
- Envio de denúncias com suporte a geolocalização.  
- Acesso a conteúdos educativos.  
- Notificações push.  
- Painel administrativo para gestão de dados.  

**Não inclui:**  
- Integração direta com sistemas internos da prefeitura.  
- Recursos de gamificação (como recompensas por participação).  
- Funcionamento offline completo.  

---

## 🏗️ Visão da Arquitetura
A arquitetura do sistema é composta por três grandes camadas: **frontend, backend e persistência de dados**.  

- O **frontend** é dividido em duas versões: **web (React)** e **mobile (React Native)**, responsáveis pela interação direta com os usuários.  
- O **backend**, construído com **Node.js e Express**, funciona como **API Gateway**, encaminhando as requisições para os serviços adequados (Horários, Feedback, Denúncias, Conteúdos e Notificações).  
- A camada de **persistência de dados** utiliza uma abordagem híbrida:  
  - **PostgreSQL** para dados estruturados e críticos (usuários, bairros, horários).  
  - **MongoDB** para dados colaborativos e não estruturados (feedbacks, denúncias, conteúdos multimídia).  

Essa divisão garante tanto a consistência necessária quanto a flexibilidade para informações dinâmicas.

### 📊 Diagrama de Arquitetura
![Diagrama de Arquitetura](./docs/images/meu_lixo_arquitetura.png)

---

## 🛠️ Tecnologias Propostas
- **Frontend Web:** React  
- **Mobile:** React Native  
- **Backend:** Node.js + Express  
- **Banco Relacional:** PostgreSQL  
- **Banco Não Relacional:** MongoDB  
- **Infraestrutura:** Docker, Kubernetes, AWS  
- **Notificações:** Firebase Cloud Messaging  
- **Prototipação:** Figma  
- **Diagramas:** Draw.io, DbDiagram  

---

## 🎨 Wireframes / Protótipos de Baixa Fidelidade
Foram desenvolvidos wireframes de baixa fidelidade para validar os fluxos principais de interação.  

As telas representam:  
- Login  
- Dashboard com consulta à próxima coleta  
- Tela de horários  
- Registro de feedbacks  
- Envio de denúncias com mapa  
- Acesso a conteúdos educativos  

Esses protótipos guiam a fase de desenvolvimento, garantindo que a interface seja simples e adequada ao público-alvo.

![Wireframes](./docs/images/Wireframes.png)

---

## 📅 Cronograma – Etapa 2 (N708)

| Fase | Atividade | Período |
|------|-----------|---------|
| 1 | Implementação do backend (APIs, banco de dados) | Semana 1–2 |
| 2 | Desenvolvimento do frontend web (React) | Semana 3–4 |
| 3 | Desenvolvimento do app mobile (React Native) | Semana 5–6 |
| 4 | Integração e testes de APIs | Semana 7 |
| 5 | Testes finais e ajustes de usabilidade | Semana 8 |
| 6 | Apresentação final | Semana 9 |

---

## 👥 Integrantes da Equipe
- Antônio Kauan Pereira do Carmo – 2318116  
- Carlos Eduardo Soares – 2317472  
- Elias Roger de Sousa – 2317680  
- Karla Briseno do Amaral – 2318110  
- Maria Fiama Sales Florencio – 2318777  
- Nathan Monteiro Silva – 2319297  



<img width="756" height="979" alt="ChatGPT Image 29 de set  de 2025, 14_58_30" src="https://github.com/user-attachments/assets/ad994413-251e-4685-8e0b-44626891518c" />
