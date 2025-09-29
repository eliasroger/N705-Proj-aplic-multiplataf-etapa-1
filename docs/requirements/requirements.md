# 📋 Requisitos do Sistema – Meu Lixo

## ✅ Requisitos Funcionais (RF)
- **RF01:** Exibir horários oficiais de coleta por bairro.  
- **RF02:** Registrar horário real de coleta informado pelo usuário.  
- **RF03:** Calcular previsão ajustada com base em feedbacks.  
- **RF04:** Enviar notificações push aos moradores cadastrados.  
- **RF05:** Permitir denúncia de descarte irregular com geolocalização.  
- **RF06:** Disponibilizar conteúdos educativos por categoria.  
- **RF07:** Gerenciar usuários (moradores, administradores, cooperativas).  
- **RF08:** Painel administrativo para visualização de relatórios.  
- **RF09:** Exportação de relatórios para PDF/Excel.  

## 🚫 Requisitos Não Funcionais (RNF)
- **RNF01:** Disponibilidade ≥ 99,5%.  
- **RNF02:** Resposta média inferior a 2 segundos em 90% das requisições.  
- **RNF03:** Segurança via HTTPS e autenticação JWT.  
- **RNF04:** Interface responsiva e acessível.  
- **RNF05:** Suporte multiplataforma (web e mobile).  
- **RNF06:** Uso de containers (Docker + Kubernetes).  
- **RNF07:** Escalabilidade horizontal suportada.  
- **RNF08:** Suporte a logs e auditorias de eventos.  

## ⚖️ Regras de Negócio
- **RN01:** Apenas administradores podem editar horários oficiais.  
- **RN02:** Feedbacks devem ser vinculados a um usuário e a um bairro.  
- **RN03:** Denúncias precisam conter descrição e localização geográfica.  
- **RN04:** Conteúdos educativos devem ter título, categoria e link válido.  
- **RN05:** Usuários comuns não podem excluir dados, apenas registrar.  
- **RN06:** Dados sensíveis (senha, token) devem ser armazenados de forma segura.  
- **RN07:** O sistema deve seguir LGPD quanto ao tratamento de dados pessoais.  

## 👤 Perfis de Usuários
- **Morador:** consulta horários, envia feedbacks e denúncias, acessa conteúdos.  
- **Administrador:** gerencia horários, conteúdos, usuários e relatórios.  
- **Cooperativa:** acessa relatórios e estatísticas de coleta/denúncia.  

## 📖 Histórias de Usuário
- **HU01:** Como morador, quero consultar o horário de coleta no meu bairro para organizar o descarte do lixo.  
- **HU02:** Como morador, quero registrar quando o caminhão passou para ajudar a prever horários futuros.  
- **HU03:** Como morador, quero denunciar pontos de lixo irregular com mapa para ajudar a prefeitura a resolver.  
- **HU04:** Como administrador, quero atualizar horários oficiais para manter a base de dados confiável.  
- **HU05:** Como administrador, quero visualizar relatórios de denúncias para planejar ações corretivas.  
- **HU06:** Como cooperativa, quero acessar estatísticas de coleta seletiva para otimizar minhas atividades.  
