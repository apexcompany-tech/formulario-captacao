# Formulário de captação · Apex

Página estática, sem build (`index.html`), no ar em https://acougue.apexcompanymkt.com (GitHub Pages). É o formulário do anúncio
da assessoria: o dono de açougue preenche nome, WhatsApp, Instagram, faturamento e se já investe em anúncios.

Quem atualiza é o `build_github.py` (workspace da Apex, `comercial/formulario_captacao/`), depois o commit + push aqui.

**Envio:** cada cadastro vai pro webhook do n8n "[Apex] Formulário açougue → planilha", que grava na planilha
"Leads Formulário - Apex Açougue" (temporário, até o CRM ter o campo pra esse formulário).

**Pixel:** "Apex Company" (2684529388382589): PageView ao abrir e Lead no envio. A página continua fora do Google (`noindex`);
o `robots.txt` é aberto pro robô da Meta conseguir revisar o anúncio.
