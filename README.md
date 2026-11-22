# Landing page do app Resultado Play Bicho

Página estática em https://app.playbicho.com para as campanhas do Meta levarem o
usuário a baixar o app na Play Store (Android) ou instalar o site no iPhone.

- `index.html`: a página. Eventos para o Tag Manager (GTM-M342VRLW):
  `lp_app_view` e `lp_app_download_click` (posicao, plataforma, utm_campaign).
- O link da Play Store carrega `utm_source`, `utm_medium` e `utm_campaign` da URL
  do anúncio no parâmetro `referrer`.
- Deploy: Dokploy constrói o `Dockerfile` (nginx, porta 80) a cada push na `main`.
