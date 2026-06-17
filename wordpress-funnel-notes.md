# WordPress/WooCommerce — Instruções de uso do template

Arquivo principal: `wordpress-funnel.html`

## Objetivo

Template V1 da página pública **Solução de Autenticação de Chamadas para Operadoras**, derivado da página interna `index.html`, mas com foco em funil comercial externo e uso futuro em WordPress/WooCommerce.

## Como portar para WordPress

### Opção inicial recomendada

1. Criar nova página no WordPress, por exemplo:
   - `/solucao-autenticacao-chamadas-operadoras/`
   - título: `Solução de Autenticação de Chamadas para Operadoras`
2. Adicionar um bloco **HTML personalizado** no Gutenberg/Elementor.
3. Colar o conteúdo do `wordpress-funnel.html`.
4. Se o tema remover `<html>`, `<head>` ou `<body>`, colar apenas:
   - `<style>...</style>`;
   - `<div class="zictec-auth-funnel">...</div>`;
   - `<script>...</script>`.
5. Subir assets usados para a Media Library ou manter caminhos equivalentes:
   - `assets/logo_blue.png`
   - `assets/hero.png`
6. Ajustar URLs dos assets se necessário.

## Isolamento de CSS

Todo o CSS visual está escopado sob `.zictec-auth-funnel`, para reduzir risco de afetar o tema WordPress/WooCommerce.

Evitar remover essa classe. Ela é o wrapper de segurança visual.

## Formulário / lead

Nesta V1, o botão **Gerar briefing**:

- atualiza a recomendação;
- gera um briefing local em texto;
- tenta copiar para a área de transferência;
- não envia ainda para CRM/Freshdesk/email.

Integrações possíveis na próxima etapa:

1. Substituir o botão por shortcode de formulário;
2. Conectar ao Contact Form 7 / WPForms / Fluent Forms;
3. Enviar para webhook Hermes/Jarvis;
4. Abrir ticket Freshdesk;
5. Enviar email para comercial;
6. Gravar lead no WooCommerce/CRM.

## Regra comercial implementada

- Cenário simples e fechado → CTA para produto WooCommerce.
- Cenário incerto, outro vendor, ABR incerto ou servidor incerto → validação técnica antes do checkout.
- Origem Verificada/campanhas → fluxo consultivo.
- Compra direta exige aceite de premissas antes de seguir para shop.

## SKUs/links usados

- `ZT_STIAS_API_A`
- `SAAS_STIAS_OOB_A`
- `ZT_STIAS_PROSBC_SETUP_CLIENT_A`
- `ZT_STIAS_PROSBC_CLIENT_A`
- `ZT_PROSBC_HW500_STIAS_SETUP_CLIENT_A`
- `ZT_PROSBC_HW500_STIAS_HYBRID_API_A` — usar link com cupom automático: `https://shop.zictec.com.br/checkout/?add-to-cart=302&apply_coupon=hybrid7800&lang=pt-br`
- cupom citado: `hybrid7800`

## Checklist de validação no WordPress

- Desktop: primeiro fold sem quebra estranha.
- Mobile: menu oculto, botões empilhados e formulário legível.
- Console sem erros JavaScript.
- Selects/radios mudam recomendação.
- Botão `Gerar briefing` mostra texto.
- CTAs apontam para produtos corretos.
- Compra direta bloqueia se o aceite não estiver marcado.
- CSS não altera header/footer do tema.
- Assets carregam da Media Library ou caminho equivalente.

## Próximo refinamento sugerido

Depois de colar no WordPress, a próxima etapa ideal é integrar o formulário a um destino real:

- webhook para Jarvis;
- Freshdesk;
- email comercial;
- ou plugin de formulário já usado no site.
