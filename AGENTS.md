# Perfil do Usuário, BrandSystem Max v0.6 & Regras de Interação (UP_app)

## 1. Quem é o Usuário (Max Reis)
- **Nome:** Max Reis
- **Assinatura de Marca (`maX`):**
  - Logotipo composto por `"ma"` em tipografia **Outfit** (branco `#FFFFFF` no fundo escuro, grafite `#14181B` no fundo claro) + símbolo **`X` sólido geométrico** sempre em **Verde `#12B886`**.
  - Símbolo isolado (Avatar/Selo): Círculo escuro com borda luminosa azul/ciano e o **`X` sólido em `#12B886`** centralizado.
- **Rotina de Treino & Objetivos (Projeto Verão):**
  - **Propósito:** Perder calorias e gorduras localizadas (especialmente barriga), ganhar resistência, força e boa aparência/estrutura corporal.
  - **Academia (3x/semana com aparelhos e utilitários):**
    - **Segunda-feira:** Cardio (Esteira + Escada) + Core;
    - **Terça-feira:** Membros Superiores;
    - **Quarta-feira:** Membros Inferiores.
  - **Compensação em Casa (Calistenia):** Conversão imediata de qualquer treino de academia para peso corporal quando faltar, somado à rotina matinal de 15 min ("Todas as Manhãs" — estilo *BetterMe Men*) e guia de alimentação saudável + vitaminas essenciais.

---

## 2. Design System Oficial — BrandSystem Max (v0.6)
Fonte: `https://brandsystem-max.vercel.app/`

### Tokens `:root` Obrigatórios
```css
:root {
  --bg: #14181B;
  --bg2: #181D1E;
  --bg3: #1d2326;
  --line: #23292A;
  --txt: #F1F5F4;
  --dim: #8A94A2;
  --blue: #0E5FA4;
  --blue-l: #6BA6DA;
  --cyan-dark: #35D0E8; /* Assina no escuro (9.64:1 AA sobre #14181B) */
  --green: #12B886;     /* Secundária 30% e cor fixa do X da marca */
  --orange: #FF6B35;    /* Accent 10% pontual - CTA / Alerta / Queima */
  --display: "Fraunces", Georgia, serif;
  --body: "Montserrat", system-ui, sans-serif;
}
```

### Regras Estritas de Cor e Tipografia
- **Proporção 60 / 30 / 10:** Dominante Azul (`#0E5FA4` no claro / `#35D0E8` no escuro), Secundária Verde (`#12B886`), Accent Laranja (`#FF6B35`).
- **Regra WCAG AA no Modo Escuro (`#14181B`):**
  - **PROIBIDO** usar `#0E5FA4` ou `#5A6472` soltos sobre `#14181B` (reprovam no contraste). No escuro, usar sempre `#35D0E8` (ciano), `#12B886` (verde), `#FF6B35` (laranja), `#FFFFFF`/`#F1F5F4` (texto) e `#8A94A2` (apoio).
  - **Cores Aposentadas (Nunca usar):** `#0E4D64`, `#F0EEE6`, `#00B4D8`.
- **Variante Orgânica (Pergaminho / Papel Quente):**
  - Fundo `#FAF7F0`, Texto `#3A2E22`, Apoio `#6B5A48`, Assinatura `#0E5FA4`.
- **Tipografia:**
  - Títulos (`h1`, `h2`, `h3`, display): `Fraunces` (`text-wrap: balance`).
  - Corpo, rótulos e UI: `Montserrat` (`text-wrap: pretty`, números com `white-space: nowrap`).
- **Raios e Sombras:**
  - `radius-sm: 6px`, `radius-md: 10px`, `radius-lg: 14px`, `radius-full: 999px`.
  - Sombras: `0 1px 3px #0006` (sm), `0 6px 18px #0008` (md), `0 14px 40px #000a` (lg).

---

## 3. Regras de Interação, Prévia e Validação no Chat
1. Sempre exibir a prévia interativa **direto no Antigravity** (Artifact HTML `UserFacing: true` no painel lateral e widget `<agent-embed>` no chat) + link clicável `[index.html](file:///d:/UP_app/index.html)`.
2. Sempre fornecer o link direto `[Abrir Painel do Navegador](conversation://<conversation-id>)` quando um subagente precisar de confirmação.
