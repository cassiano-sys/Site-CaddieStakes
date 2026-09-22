# Caddie Stakes Golf — landing page

Site institucional simples (uma página só, bilíngue PT/EN) para `caddiestakesgolf.com`. Sem build, sem dependências — é um único `index.html` autocontido (CSS e JS inline).

## Como publicar

1. **Criar um repositório novo no GitHub** (ex: `caddiestakesgolf-landing`), separado do `nassau-app`. Suba só o `index.html` (e este README, se quiser) na raiz — pelo editor web do GitHub mesmo, do jeito que já estamos fazendo com o app.

2. **Importar como um novo projeto na Vercel**: "Add New… → Project" → selecione o repositório `caddiestakesgolf-landing` → Framework Preset "Other" (site estático, sem build) → Deploy. Não precisa configurar nada além disso.

3. **Conectar o domínio raiz a este projeto**: dentro do novo projeto, em Settings → Domains, adicione `caddiestakesgolf.com` (e opcionalmente `www.caddiestakesgolf.com` redirecionando para ele).

4. **Mover o app para um subdomínio**: no projeto `nassau-app` (o app de verdade), em Settings → Domains, adicione `app.caddiestakesgolf.com`. Esse é o endereço que o botão "Entrar" / "Sign in" da landing page já aponta.

5. Depois disso, os dois ficam assim:
   - `caddiestakesgolf.com` → esta landing page (vitrine)
   - `app.caddiestakesgolf.com` → o app de verdade (login, rodadas, etc.)

## Pendências depois de publicar

- Atualizar o link/QR code do Manual (hoje aponta para `nassau-app-phi.vercel.app`) para `app.caddiestakesgolf.com`.
- Se quiser, também dá pra manter `nassau-app-phi.vercel.app` funcionando como está (a Vercel permite múltiplos domínios apontando pro mesmo projeto), sem quebrar nada pra quem já tem o atalho salvo.
