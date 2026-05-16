# Case, clínica de estética high-ticket São Paulo

Estudo de caso real, com dados anonimizados, de operação de growth em clínica de estética premium no Rio que estava perto de fechar e fechou quatro meses depois com um milhão e novecentos mil em contratos.

## Contexto inicial

Clínica de estética com posicionamento high-ticket, ticket médio entre quinze e quarenta mil reais por paciente, dependendo do tratamento. Quatro anos de operação, base de pacientes pequena, presença digital sem direção, mídia paga sangrando sem retorno claro, equipe interna sem cultura de copy ou de funil. Receita mensal em curva descendente havia oito meses. Caixa para mais doze a dezesseis semanas de operação no ritmo atual.

A diretora da clínica veio com pedido direto: salvar o negócio em até cento e vinte dias, ou fechar.

## Diagnóstico

Em uma semana de auditoria, ficaram claros seis problemas, ordenados pelo impacto.

Primeiro, o pixel do Meta Ads estava disparando eventos genéricos de PageView mas não estava registrando Lead, e o evento de Purchase nunca tinha sido implementado. A clínica vinha gastando em campanhas otimizadas para tráfego em vez de conversão por dois anos. Custo por aquisição real era invisível.

Segundo, a estratégia de copy era baseada em listar procedimentos. Anúncios diziam "harmonização facial a partir de R$ X" e levavam para landing page com mais procedimentos listados. Em segmento de alto ticket, paciente não compra procedimento. Compra confiança no profissional, garantia de resultado e contexto emocional de transformação.

Terceiro, a base de leads tinha quatro mil contatos não nutridos, nenhuma sequência de e-mail, nenhuma régua de relacionamento. Lead que entrava esfriava em setenta e duas horas e era perdido.

Quarto, o time comercial não tinha script de venda, não tinha CRM em uso, e tratava todo lead como igual, sem priorização.

Quinto, a clínica tinha um diferencial real (médico com formação rara e equipamentos de geração mais recente que a concorrência local) que nunca tinha sido usado em copy. O que pesa em decisão de alto ticket nunca era dito ao paciente.

Sexto, a precificação tinha barreira psicológica brutal. Tickets de quinze a quarenta mil reais em pagamento à vista eram inviáveis para o público real da clínica, que tinha dinheiro mas não tinha o dinheiro disponível em uma transferência única.

## Solução implementada

Quatro frentes em paralelo, executadas em janela de doze semanas.

Frente um, infraestrutura de tracking. Reescrita do container de GTM, implementação de evento Lead com parâmetros customizados, implementação de Purchase com valor monetário real, configuração de CAPI do Meta para reduzir perda por bloqueador de pixel. Tempo: duas semanas.

Frente dois, reposicionamento de copy. Toda campanha foi reescrita do zero. Em vez de listar procedimentos, copy passou a falar sobre o medo de envelhecer mal, o cuidado de não ficar com cara de "fez", a busca por confiança no espelho. O médico da clínica virou personagem central, com narrativa, fotos profissionais, conteúdo de bastidor. Em entrevista clínica gravada, ele explicava por que recusa paciente quando o procedimento solicitado não vai entregar o resultado pedido. Esse vídeo virou peça de funil de mais alto desempenho. Tempo: três semanas.

Frente três, nutrição e funil. Sequência de quatorze e-mails ao longo de vinte e um dias, mais sequência de WhatsApp segmentada por intenção. Lead frio ia para conteúdo educacional, lead morno ia para prova social, lead quente ia para agendamento. Time comercial foi treinado com script de descoberta e qualificação. CRM mínimo implementado em planilha estruturada antes da migração para HubSpot. Tempo: três semanas.

Frente quatro, e essa foi a virada do jogo, financiamento. Parceria com financeira especializada em saúde e estética. Paciente passou a poder fechar contrato em até trinta e seis vezes com aprovação em vinte e quatro horas. A barreira psicológica do "à vista" desapareceu. Tempo: duas semanas para fechar parceria e integrar no fluxo.

## Resultado em doze semanas

| Métrica | Antes | Depois | Variação |
|---|---|---|---|
| Custo por lead | R$ 47,00 | R$ 4,00 | menos 91% |
| Taxa de qualificação de lead | 8% | 31% | mais 287% |
| Taxa de fechamento (qualificado para contrato) | 12% | 34% | mais 183% |
| Ticket médio fechado | R$ 11.000 | R$ 18.500 | mais 68% |
| Receita do período | R$ 280 mil (3 meses anteriores) | R$ 1.900 mil (4 meses) | mais 578% |

Da receita total de um milhão e novecentos mil, aproximadamente um milhão veio de um evento único da clínica que reuniu pacientes em janela de três dias, com agendamento concentrado. Os outros novecentos mil vieram de contratos financiados ao longo dos quatro meses.

## Decisões técnicas que importam

Três decisões fora do óbvio, que costumam não aparecer em case mais cosmético.

Primeira, escolha de não usar lookalike de Meta nos primeiros sessenta dias. A base de pacientes históricos era pequena demais (menos de mil) e enviesada (concentrada em um perfil de tratamento específico). Lookalike geraria audiência sintética que não refletia o público-alvo real. Optei por interesse comportamental refinado por exclusão, e o custo por lead caiu mais rápido com isso do que cairia com lookalike forçado em base ruim.

Segunda, decisão de não disparar campanha de remarketing até o pixel ter três semanas de dados de qualidade. Remarketing em base mal capturada cria audiência poluída que prejudica algoritmo a longo prazo. Esperei o dado estabilizar antes de ligar remarketing, o que sacrificou volume de curto prazo em troca de eficiência sustentada.

Terceira, decisão de centralizar comunicação em WhatsApp em vez de e-mail. Público brasileiro de alto ticket em estética abre WhatsApp em vinte minutos, abre e-mail em três dias. Toda a régua de nutrição foi desenhada para WhatsApp com fallback de e-mail, e a taxa de resposta entre lead e abordagem comercial caiu de quarenta e oito horas para cento e vinte minutos em média.

## Aprendizados

Em alto ticket de saúde e estética, o que vende não é o procedimento, é a confiança no profissional. Toda copy que esquece isso queima orçamento.

Financiamento muda o mercado endereçável de forma que nenhuma otimização de criativo consegue replicar. Em quatro meses, sessenta e três por cento dos contratos fechados não teriam fechado sem a opção de parcelamento. Foi a alavanca de maior efeito isolado em todo o projeto.

Tracking ruim mente sobre o que está funcionando. Antes de discutir criativo, copy ou audiência, o primeiro trabalho de qualquer auditoria é confirmar que o dado da plataforma reflete o evento real. Sem isso, toda decisão posterior é palpite com cara de análise.

## Stack utilizada

Meta Ads, Google Ads, Google Tag Manager, GA4, HubSpot CRM (a partir da semana oito), WhatsApp Business API via Twilio, ActiveCampaign para nutrição por e-mail, Looker Studio para dashboard executivo, Photoshop e Premiere para criativo, Notion para gestão do projeto.

## Por que este case está aqui

Porque growth marketing real raramente é tecnologia. É raciocínio de negócio aplicado com método. Quem contrata Head de Growth quer alguém que saiba decidir entre lookalike ou interesse refinado em base ruim, que saiba quando esperar o pixel calibrar, que saiba reconhecer quando o problema não é mídia paga e sim falta de financiamento. Esse repositório serve para mostrar essa camada de decisão, que não cabe em bullet point de currículo.

## Contato

Christian Belga, csbelga em gmail. LinkedIn em https://www.linkedin.com/in/christianbelga
