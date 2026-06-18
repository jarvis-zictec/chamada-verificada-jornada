# Brainstorm — evolução do ecossistema Chamada Verificada / Origem Verificada

Data: 2026-06-18
Origem: brainstorm do Allan no thread Discord `apresentacao sobre chamada verificada`.
Status: anotação de planejamento futuro. **Não alterar a landing principal nem o funil atual para operadoras neste momento.**

## Contexto

`https://www.chamadaverificada.com.br` continua sendo a landing principal para **operadoras/prestadoras de voz**.

A ideia é evoluir o ecossistema com páginas complementares, separando claramente três entradas comerciais:

1. **Sou Operadora**
2. **Sou Empresa e quero identificar minha marca**
3. **Sou Call-Center e quero identificar as marcas que represento**

Os dois novos nichos têm dinâmica de atendimento, serviços e entrega totalmente distinta do cenário de operadoras.

## Entrada 1 — Sou Operadora

### Papel atual

Manter como está: foco em operadoras/prestadoras de voz que precisam tratar autenticação de chamadas, STIR/SHAKEN, integração com SBC/ProSBC/API/ISBC, ABR e jornada técnica de implantação.

### Guardrail

Não mexer no que já foi feito para o cenário de operadoras durante esta fase de brainstorm.

### Propriedades do cenário

- Pode envolver SBC, ProSBC, ISBC, API, servidor, setup técnico e autenticação direta.
- É o funil técnico-comercial atual.
- Continua sendo o eixo principal da landing `chamadaverificada.com.br`.

## Entrada 2 — Sou Empresa e quero identificar minha marca

### Proposta de posicionamento

Página complementar voltada a empresas que querem que suas chamadas apareçam com marca/campanha/finalidade reconhecível para o usuário final.

### Diferença essencial em relação a operadoras

Este fluxo **não usa SBC do cliente** e **não faz autenticação direta pelo cliente**.

A ZICTEC atua no ecossistema da ABR como uma camada operacional/representante, em papel semelhante ao de um call-center/gestor, para:

- gerir campanhas;
- orientar cadastro e adesão;
- contratar ou coordenar operadoras habilitadas;
- operacionalizar a jornada de Origem Verificada/Branded Call para empresas sem exigir que a empresa seja operadora.

### Possíveis serviços

- Diagnóstico de uso de chamadas pela empresa.
- Organização de marcas, números, campanhas e finalidades.
- Gestão operacional de cadastro/adesão no ecossistema ABR.
- Coordenação com operadoras/parceiros que façam autenticação/fornecimento dos números.
- Opcionalmente, revenda/fornecimento de rotas de terminação quando fizer sentido comercial e regulatório.

### Mensagem comercial inicial

Para empresas, a promessa não deve ser “implantar STIR/SHAKEN no seu SBC”. Deve ser algo como:

> Sua empresa quer que o cliente reconheça chamadas legítimas da sua marca. A ZICTEC organiza a jornada de campanha, números, operadora/parceiro e operação para tornar isso viável sem exigir infraestrutura de telecom própria.

## Entrada 3 — Sou Call-Center e quero identificar as marcas que represento

### Proposta de posicionamento

Página complementar voltada a call-centers/BPOs/contact centers que fazem chamadas em nome de múltiplas marcas e precisam organizar a identificação dessas marcas/campanhas.

### Diferença essencial em relação a operadoras

O foco também **não é SBC/autenticação direta do cliente**.

O foco é suporte operacional para:

- gestão de múltiplas marcas representadas;
- gestão de campanhas e finalidades;
- adesão/cadastro no ecossistema ABR;
- coordenação com operadoras/parceiros que autentiquem/forneçam os números;
- governança para evitar mistura entre marca, campanha, número e rota.

### Possíveis serviços

- Onboarding operacional de marcas atendidas pelo call-center.
- Padronização de documentação por marca/campanha.
- Gestão de inventário de números/campanhas.
- Suporte à adesão ABR e manutenção cadastral.
- Coordenação com operadoras/parceiros.
- Pacotes recorrentes de operação/gestão de campanhas.

### Mensagem comercial inicial

> Seu call-center representa várias marcas. A ZICTEC ajuda a organizar campanhas, marcas, números e adesão operacional para que a identificação da chamada seja tratada de forma governada e escalável.

## Papel futuro da ZICTEL

A ZICTEL, operadora do Allan, pode futuramente ser a principal parceira para:

- autenticação;
- fornecimento de números;
- terminação/rotas;
- operação regulada nos cenários de empresas e call-centers.

### Recorte geográfico inicial

- Atuação direta da ZICTEL nas áreas onde atua, especialmente SC.
- Fora dessas áreas, atuar via parceiros/operadoras habilitadas.

## Implicações para arquitetura comercial do site

Hipótese futura de navegação:

```text
chamadaverificada.com.br
├── Sou Operadora
│   └── Jornada atual: autenticação, SBC, ProSBC, API, ISBC, ABR
├── Sou Empresa e quero identificar minha marca
│   └── Jornada de Origem Verificada como serviço gerenciado / campanhas / operadoras parceiras
└── Sou Call-Center e quero identificar as marcas que represento
    └── Jornada de gestão multi-marca / campanhas / adesão ABR / suporte operacional
```

## Guardrails de conteúdo

- Não misturar a linguagem técnica de operadora com a de empresa/call-center.
- Não prometer autenticação direta para empresa/call-center se a execução depender de operadora/parceiro.
- Separar claramente:
  - autenticação técnica de chamadas;
  - identificação/Origem Verificada/Branded Call;
  - gestão operacional de campanhas;
  - fornecimento/terminação de números/rotas.
- Preservar a landing atual como referência para operadoras.

## Próximos passos sugeridos

1. Definir os três perfis/personas em uma matriz simples:
   - dor principal;
   - quem compra;
   - quem opera;
   - dependências regulatórias/técnicas;
   - oferta ZICTEC/ZICTEL/parceiro;
   - CTA principal.
2. Escrever wireframe/copy de baixa fidelidade para as duas novas páginas.
3. Mapear quais serviços viram produto/pacote recorrente e quais ficam consultivos.
4. Validar internamente com Allan onde a ZICTEL entra diretamente e onde precisa de parceiro.
5. Só depois publicar páginas novas, sem alterar o fluxo de operadoras já aprovado.
