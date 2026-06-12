# 🎬 Cinetwo

App de lista de filmes para casais. Adicione, organize e descubra filmes juntos — com sincronização em tempo real entre os dois celulares.
---

## ✨ Funcionalidades

### 📋 Lista de filmes
- Adicionar filmes com busca automática via TMDB (poster, gênero, ano)
- Marcar filmes como assistidos com data registrada automaticamente
- Filtros: Todos / Para assistir / Assistidos
- Cards com poster, ano, gênero e quem indicou

### 🎬 Informações do filme
- Sinopse, nota TMDB, duração e gêneros
- Onde assistir (streaming disponível no Brasil)
- Filmes recomendados baseados no TMDB

### 💘 CineMatch
- Modo Tinder para filmes — cada um avalia no próprio celular
- Desliza para direita ❤️ para curtir, para esquerda 👎 para pular
- Quando os dois curtirem o mesmo filme: **É um Match!**
- Notificação automática ao abrir o app se houver match pendente

### 🎲 Sorteio
- Sorteia aleatoriamente um filme da lista de não assistidos
- Animação de dado 3D ao sortear

### 📊 Estatísticas
- Tempo total, assistido e a assistir estimados
- Progresso da lista com anel animado
- Contador de dias sem assistir
- Ranking de quem indicou mais
- Gêneros favoritos do casal

### ⚙️ Configurações
- Personalizar nomes dos dois
- Alterar senha
- Modo escuro
- Instalar como app na tela inicial (PWA)

---

## 🛠 Stack

| Tecnologia | Uso |
|---|---|
| HTML / CSS / JS | Frontend — arquivo único |
| Firebase Realtime Database | Sincronização em tempo real |
| TMDB API | Informações, posters e recomendações de filmes |
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

---


## 🤝 Créditos

Desenvolvido por [João Guilherme](https://github.com/joaogdlima) para uso pessoal do casal.

Dados de filmes fornecidos pelo [TMDB](https://www.themoviedb.org).

---

*Feito com ❤️ e muito debate sobre o que assistir hoje*
