# Landing — Marketing, Vendas e IA

Página de vendas (estática) para serviços de marketing, vendas e IA.
Arquivo único auto-contido (`index.html`) + imagens + áudio.

## Ver localmente
Dê dois cliques em `index.html` (abre no navegador) ou rode um servidor:
```bash
python3 -m http.server 4321
# acesse http://localhost:4321/
```

## Onde editar (sem mexer no design)
Tudo no `index.html`:

- **Número de WhatsApp** — procure `const WHATSAPP =` (formato 55 + DDD + número).
- **Captura de leads** (Planilha Google + e-mail) — procure `const LEADS_ENDPOINT =`
  (URL do Google Apps Script terminada em `/exec`).
- **Mensagem que abre no WhatsApp** — procure `const msg =`.
- **Depoimentos (prints)** — imagens `resultado-1.jpg` … `resultado-6.jpg`.
- **Áudio de depoimento** — `depoimento-audio.m4a` (e o bloco `audio-card` no HTML).
- **Foto da seção "Quem está por trás"** — `especialista.jpg`.
- **Fundos** — `bg-hero-circuito.png` (hero), `bg-radar.png` e `bg-bussola.png` (seções).

## Publicação
Site 100% estático — pode ser hospedado em GitHub Pages, Vercel, Netlify
ou qualquer hospedagem. Para domínio próprio, aponte o DNS conforme o provedor.
