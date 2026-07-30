# Mutual-Credit-AI — Draft Outline
> Working title: "Agents That Close the Loop: AI Liquidity Matching in Community Mutual Credit Networks"

## Pitch (3 frases)

Moedas complementares (Sardex, Mumbuca, bancos comunitários) retêm riqueza localmente e amortecem crises, mas morrem historicamente de iliquidez: saldos acumulam sem contrapartida e a rede congela. Esse é um problema de matching contínuo em grafo dinâmico — hoje tratável com agentes LLM + algoritmos de clearing de ciclos. Implantamos matching de IA (detecção de ciclos multi-hop + agente negociador) num circuito de feira agroecológica no Recife e medimos liquidez, saldos presos e retenção contra baseline sem matching.

## Contribuições pretendidas

1. Formalização da iliquidez de crédito mútuo como problema de clearing de ciclos em grafo dinâmico + matching assistido por agente.
2. Sistema real: agentes que propõem trocas multi-hop que nenhum participante enxerga (integração `code/gira`).
3. Estudo de campo em feira agroecológica (Global South, população não-tech) com métricas de rede (à la análise de rede do Sardex: 1.477 empresas/48k transações como referência metodológica).
4. Design constraint documentado: mecanismo que não "fortalece capitalismo por tabela" (caveat gira) — métricas de acesso e circulação, não só volume.

## Related work (seeds)

- Dini & Motta, LSE — Sardex micro-macro: https://eprints.lse.ac.uk/67135/7/Dini_From%20complimentary%20currency.pdf
- Análise de rede Sardex (robustez econômica × estrutura): https://www.researchgate.net/publication/388032585
- Mumbuca/Maricá — retenção municipal e multiplicador: https://pantheon.ufrj.br/handle/11422/15631
- Banco Palmas — literatura de bancos comunitários BR (buscar âncora)
- Clearing de ciclos: literatura de obligation netting / graph clearing (buscar âncora formal — Eisenberg-Noe adjacente)
- EAAMO agenda: https://arxiv.org/pdf/1810.09832

## Esqueleto

1. Intro — moedas complementares funcionam e morrem; a causa-mortis é computacional
2. Model — grafo de crédito mútuo, iliquidez formalizada, tetos de saldo (regra Sardex)
3. System — agentes de matching (arquitetura em code/gira/ROADMAP.md), onboarding por voz/WhatsApp
4. Field study — feira do Recife, protocolo test-to-kill do núcleo circuito
5. Results / 6. Discussion — inclui análise do caveat distributivo (cilada 4 do núcleo)

## TODO imediato

- [ ] Âncora formal de clearing de ciclos (rede de obrigações) — /research lit
- [ ] Fichar análise de rede do Sardex (metodologia a replicar)
- [ ] Definir métricas de "saldo preso" e liquidez antes do piloto (pré-registro)
