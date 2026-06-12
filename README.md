# 🎬 Cinetwo

App de lista de filmes para casais. Adicione, organize e descubra filmes juntos — com sincronização em tempo real entre os dois celulares.

---

## ✨ Funcionalidades

### 📋 Lista de filmes
- Adicionar filmes com autocomplete via TMDB — poster, gênero e ano preenchidos automaticamente
- Filtrar por status (Total / A ver / Vistos) clicando direto nos números do header
- Filtrar por gênero com chips clicáveis (com emojis por gênero)
- Marcar como assistido com animação de confete 🎊
- Data registrada automaticamente ao marcar — editável depois
- Avaliação ⭐ 1-5 e comentário curto após marcar como assistido
- Notificação em tempo real quando o outro adiciona um filme
- Confirmação antes de excluir

### 🎬 Informações do filme
- Sinopse em português, nota TMDB, duração e gêneros
- Onde assistir no Brasil (streaming, aluguel ou compra)
- Trailer direto no YouTube
- Filmes recomendados pelo TMDB com botão de adicionar direto

### 💘 CineMatch
- Modo Tinder para filmes — cada um avalia no próprio celular
- Arrastar para direita ❤️ para curtir, para esquerda 👎 para pular
- Quando os dois curtirem o mesmo filme: popup de match
- Notificação automática ao abrir o app se houver match pendente

### 🎲 Sorteio
- Sorteia aleatoriamente um filme da lista de pendentes
- Animação de dado 3D
- Mostra poster, título, ano e quem indicou

### 📊 Estatísticas
- Tempo total, já assistido e a assistir (estimado por gênero ou duração real)
- Anel de progresso da lista
- Contador de dias sem assistir com emoji progressivo
- Ranking de quem indicou mais com avatares coloridos
- Gêneros favoritos do casal

### 📅 Histórico
- Último filme assistido com poster, data, avaliação e comentário
- Calendário mensal com os dias que assistiram filmes destacados
- Toque num dia para ver quais filmes foram assistidos naquele dia

### 📤 Compartilhar
- Botão no action sheet para compartilhar qualquer filme via WhatsApp
- Mensagem formatada com título, gênero, nota e quem indicou

### ⚙️ Configurações
- Personalizar nomes dos dois
- Alterar senha
- Trocar a foto do casal na tela de login
- Modo escuro
- Instalar como app na tela inicial (PWA)
- Apagar toda a lista

---

## 🛠 Stack

| Tecnologia | Uso |
|---|---|
| HTML / CSS / JS | Frontend — arquivo único |
| Firebase Realtime Database | Sincronização em tempo real |
| TMDB API | Informações, posters, trailers e recomendações |
| GitHub Pages | Hospedagem gratuita |

---

## 🔧 Configuração

### Pré-requisitos
- Conta no [Firebase](https://firebase.google.com) com Realtime Database criado
- Chave de API do [TMDB](https://www.themoviedb.org/settings/api)

### Variáveis no código

No `index.html`, localize e substitua:

```js
// Firebase
const firebaseConfig = {
  apiKey: "SUA_API_KEY",
  databaseURL: "https://SEU_PROJETO.firebaseio.com",
  projectId: "SEU_PROJETO",
  appId: "SEU_APP_ID"
};

// TMDB
const TMDB_KEY = 'SUA_CHAVE_TMDB';
```

### Regras do Firebase

No console do Firebase, defina as regras do Realtime Database:

```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

### Deploy

1. Faça um fork ou clone do repositório
2. Configure as variáveis acima
3. Ative o GitHub Pages em **Settings → Pages → Deploy from branch → main**
4. Acesse em `https://seu-usuario.github.io/cinetwo`

---

## 📱 Instalar como app

No **Android**: abra no Chrome → menu ⋮ → "Adicionar à tela inicial"

No **iPhone**: abra no Safari → botão ⎙ → "Adicionar à Tela de Início"

Ou acesse **Configurações ⚙️ → Instalar app** diretamente no Cinetwo para ver o passo a passo.

---

## 🤝 Créditos

Desenvolvido por [João Guilherme](https://github.com/joaogdlima) para uso pessoal do casal.

Dados de filmes fornecidos pelo [TMDB](https://www.themoviedb.org).
