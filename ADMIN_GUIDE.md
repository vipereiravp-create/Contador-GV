# Contador-GV - Guia de Configuração

## 🚀 Como funciona

O contador regressivo agora **sincroniza as configurações automaticamente** entre todos os usuários que acessam o link.

### Fluxo de Sincronização:
1. **Admin configura** título, data e imagem no painel Admin
2. **Clica "Salvar alterações"** - configuração é salva localmente
3. **Clica "📤 Compartilhar config"** - copia o JSON atualizado
4. **Faz commit** do arquivo `config.json` no GitHub (ou solicita atualização)
5. **Todos os visitantes** veem a mesma configuração em tempo real (sincroniza a cada 5 segundos)

---

## 📋 Credenciais de Admin

- **Usuário:** `admin`
- **Senha:** `q2l9w5n8`

---

## 🔄 Sincronização em Tempo Real

- ✅ Página verifica atualizações a cada 5 segundos
- ✅ Se detectar mudanças, recarrega automaticamente
- ✅ Indicador na tela mostra: "✓ Sincronizado" ou "◯ Modo local"

---

## 📝 Como Compartilhar Configurações

### Método 1: Via GitHub (Recomendado)
1. Clique em "📤 Compartilhar config" no painel admin
2. Copie o JSON exibido
3. Acesse [config.json](config.json) no repositório
4. Clique em ✏️ (editar)
5. Cole o novo JSON
6. Commit com mensagem: "Update event config"

### Método 2: Link com Parâmetros (Simples)
```
https://vipereiravp-create.github.io/Contador-GV/?title=Seu%20Evento&date=2026-12-25
```

---

## 🎨 Personalizações

### Título do Evento
- Campo: "Título do evento"
- Máximo: 60 caracteres
- Exemplo: "Rolê de Natal - OGB"

### Data do Evento
- Campo: "Data do evento"
- Formato: YYYY-MM-DD
- Exemplo: 2026-12-25

### Imagem de Fundo
- Campo: "Imagem de fundo"
- Tipos aceitos: PNG, JPG, GIF
- Salva localmente (localStorage)
- Máximo: tamanho do arquivo do navegador

---

## 🔒 Segurança

- Credenciais **não aparecem** na tela
- Senha armazenada apenas no código fonte
- Recomenda-se alterar a senha se publicar código

---

## ⚡ URLs Úteis

- **Site Público:** https://vipereiravp-create.github.io/Contador-GV/
- **Arquivo de Config:** https://vipereiravp-create.github.io/Contador-GV/config.json
- **Repositório:** https://github.com/vipereiravp-create/Contador-GV

---

## 📱 Compatibilidade

- ✅ Desktop (Chrome, Firefox, Safari, Edge)
- ✅ Mobile (responsivo)
- ✅ Tablets
- ✅ Sem dependências externas (HTML/CSS/JS puro)

---

**Última atualização:** 2026-09-01
