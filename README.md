# 🚨 Blitzalerta

Um app de alerta em tempo real para motoristas sobre blitzes de Lei Seca, Polícia Militar e Fiscalização de Trânsito.

## 🎯 Funcionalidades

- **Autenticação Segura**: Email, Google e Apple Login
- **Anonimato no Mapa**: Criadores de alerta aparecem como anônimos
- **Mapa em Tempo Real**: Localização GPS do motorista
- **Alerta Rápido**: 1 clique para marcar blitz na coordenada atual
- **Validação Comunitária**: Sistema de votos para confirmar/desmentir blitzes
- **TTL Automático**: Remove blitzes sem confirmação após 30-45 minutos
- **Notificações por Raio**: Alerta sonoro quando se aproxima de blitz (1-2 km)
- **Histórico e Estatísticas**: Rastreie padrões de blitzes na sua região

## 📁 Estrutura do Projeto

```
blitzalerta/
├── backend/              # API Node.js + Express
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── middleware/
│   │   └── services/
│   ├── .env.example
│   ├── package.json
│   └── server.js
├── mobile/               # React Native App
│   ├── src/
│   │   ├── screens/
│   │   ├── components/
│   │   ├── services/
│   │   ├── utils/
│   │   └── navigation/
│   ├── app.json
│   └── package.json
├── web/                  # React Web (opcional)
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   └── App.js
│   └── package.json
├── docs/                 # Documentação
│   ├── API.md
│   ├── ARCHITECTURE.md
│   └── DEPLOYMENT.md
└── .gitignore
```

## 🚀 Quick Start

### Backend

```bash
cd backend
npm install
cp .env.example .env
# Configure suas variáveis de ambiente
npm run dev
```

### Mobile

```bash
cd mobile
npm install
# Configure Firebase
npm start
```

## 🔐 Autenticação

- Firebase Authentication (Email, Google, Apple)
- Tokens JWT para API
- Dados do usuário anônimos no mapa

## 🗺️ Mapa em Tempo Real

- Google Maps API
- WebSocket (Socket.io) para atualizações em tempo real
- Ícones customizados por tipo de blitz
- Raio de 1-2 km para notificações

## 🔔 Notificações

- Firebase Cloud Messaging (FCM)
- Notificações push quando se aproxima de blitz
- Alerta sonoro personalizável
- Notificações silenciosas em background

## 🗳️ Sistema de Validação

- Votação comunitária (👍 Sim / 👎 Não)
- Reputação de usuários
- TTL de 30-45 minutos sem confirmação
- Remoção automática de blitzes expiradas

## 📊 Estatísticas

- Heatmap de blitzes por região
- Horários de pico
- Tipos mais comuns
- Histórico pessoal

## 📝 Licença

MIT

## 👨‍💻 Desenvolvedor

Tayrone Papalino

---

**Contribuições são bem-vindas!** 🎉
