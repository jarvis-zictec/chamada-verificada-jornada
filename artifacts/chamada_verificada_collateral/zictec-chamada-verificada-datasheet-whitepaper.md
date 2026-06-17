# Chamada Verificada ZICTEC: Datasheet técnico-comercial

**Fonte:** página Chamada Verificada ZICTEC validada em GitHub Pages  
**Data:** 17/06/2026  
**Uso recomendado:** material comercial, pré-venda, reunião executiva e alinhamento de escopo técnico.

## Resumo executivo

A jornada de Chamada Verificada da ZICTEC organiza a oferta de Autenticação de Chamadas, STIR/SHAKEN e preparação para Origem Verificada em pacotes claros. O objetivo é reduzir risco operacional, evitar compra incompleta e guiar o cliente entre consumo por SIP/ISBC, API REST, Client ProSBC, bundle híbrido e pacotes com servidor físico.

## Conceitos centrais

- **STIR/SHAKEN:** tecnologia/protocolo usado para assinatura e validação da origem da chamada.
- **Autenticação de chamadas:** envio das chamadas nas interconexões autenticadas conforme regras do ecossistema operacional e regulatório.
- **Origem Verificada:** camada brasileira de identificação/branded call, com marca, logo e campanha. Depende de Autenticação.
- **ABR Telecom:** referência institucional e operacional a ser usada na terminologia comercial.

## Benefícios para o cliente

1. **Menos risco na origem da chamada:** validação técnica, trilha de auditoria e critérios para reduzir uso indevido de números, falhas de autenticação e contestação.
2. **Pacote certo para a topologia atual:** separa ISBC Cloud, API REST, Client ProSBC, setup, licença, hardware e suporte.
3. **Base para Origem Verificada:** primeiro autenticação; depois identificação, marca e campanhas com dependências explícitas.

## Formas de consumir a solução

| Modalidade | Quando usar | O que entrega | Atenções |
|---|---|---|---|
| Starter AS-OOB SaaS | Cliente precisa de SIP/ISBC Cloud | ISBC Cloud compartilhado consumindo API ZICTEC | Setup promocionalmente isento; validar limites Light |
| API REST ZICTEC Tools | Cliente compatível quer consumo REST direto | API, relatórios, auditoria, CDR, volumetria e falhas | Não inclui ISBC/SIP nem Client ProSBC |
| Client ProSBC | Integração precisa rodar no ProSBC | Script/cliente proprietário licenciado por SBC | No primeiro SBC normalmente combina com setup |
| Bundle híbrido | Cliente ProSBC quer API + client | API REST SaaS + Client ProSBC | Bundle anual sem servidor não inclui setup |
| Pacotes com servidor | Cliente precisa base ProSBC funcional | Hardware, 500 sessões, setup/client e, no híbrido, API Tools | Suporte operacional e expansões ficam fora salvo contratação |

## Matriz de pacotes / SKUs

| Cenário | SKU / pacote | Valor referência | Leitura comercial |
|---|---:|---:|---|
| SIP via ISBC compartilhado | SAAS_STIAS_OOB_A | R$ 39.000,00 | Starter AS-OOB SaaS, plano Light, setup isento na promoção |
| API REST direto | ZT_STIAS_API_A | R$ 31.200,00 | Tools/relatórios/API para cliente compatível, sem SIP |
| Client ProSBC adicional | ZT_STIAS_PROSBC_CLIENT_A | R$ 12.000,00 | Licença anual por SBC, não inclui setup |
| Primeiro ProSBC sem servidor | ZT_STIAS_PROSBC_SETUP_CLIENT_A | R$ 18.400,04 | SETUP + Client 1 ano, 30% off sobre setup+client |
| Servidor + ProSBC funcional | ZT_PROSBC_HW500_STIAS_SETUP_CLIENT_A | R$ 33.864,44 | Hardware + 500 sessões + SETUP + Client |
| Híbrido completo 1º ano | ZT_PROSBC_HW500_STIAS_HYBRID_API_A | R$ 49.464,44 | Servidor + 500 sessões + Client + API Tools; cupom hybrid7800 |
| Setup avulso | ZTSHAKENDEPLOY | R$ 14.285,78 | Serviço de implantação/homologação, não é licença |

**Observação promocional:** o pacote ZT_PROSBC_HW500_STIAS_HYBRID_API_A usa o cupom promocional **hybrid7800** no shop, conforme jornada comercial publicada.

## Jornada de contratação

1. **Educar em 2 minutos:** diferenciar STIR/SHAKEN, Autenticação e Origem Verificada.
2. **Escolher objetivo:** cumprir regulação, operar com suporte, manter ProSBC atual, modernizar topologia ou ativar campanhas.
3. **Responder checklist técnico:** SBC/vendor, rotas, volumetria, status ABR, relatórios, campanhas e suporte.
4. **Receber pacote recomendado:** API REST, ISBC/SIP, Client ProSBC, bundle híbrido ou pacote com servidor.
5. **Checkout ou lead qualificado:** compra inicia validação; cenários complexos viram proposta formal.

## Checklist de kickoff

### Cliente e regulatório
- Razão social, CNPJ e responsável técnico.
- Status ABR Telecom: não iniciado, UAT/homologação ou produção.
- Credenciais/certificados disponíveis.
- Objetivo: Autenticação, Identificação/Origem Verificada ou ambos.

### Topologia e tráfego
- SBC/vendor, versão e capacidade.
- Rotas/interconexões e volumetria.
- IN-BAND, OUT-OF-BAND ou indefinido.
- Necessidade de ProSBC, licença, servidor físico ou expansão.

### Operação e aceite
- Relatórios/auditoria esperados.
- Suporte pós-go-live e SLA desejado.
- Premissas fora de escopo.
- Critério de homologação e aceite.

## Premissas e exclusões comerciais

- O ecommerce deve reduzir fricção, não prometer implantação automática universal.
- A compra inicia contratação/validação; produção depende de ambiente, rotas, credenciais, homologação e aceite.
- API REST Tools não é ISBC Cloud; Client ProSBC não é licença da API SaaS.
- SETUP é serviço, não licença. Para ProSBC, combinar com Client ou usar pacote fechado.
- Pacotes com servidor físico são variações vinculadas aos itens sem servidor; o que renova no segundo ano deve ficar explícito.
- Suporte operacional, banco de horas, transcoding, expansões e SLA dedicado ficam fora salvo contratação separada.

## Próxima ação recomendada

Usar o configurador comercial para gerar briefing de pré-venda e selecionar a rota adequada: compra direta, validação obrigatória ou proposta formal. Para reuniões comerciais, anexar este datasheet e a apresentação executiva como materiais de apoio.
