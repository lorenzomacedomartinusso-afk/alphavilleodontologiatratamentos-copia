# Alphaville Odontologia: site

## O projeto
Site do consultório Alphaville Odontologia (Alameda Rio Negro, 967, Sala 129, Edifício Alpha Premium, Alphaville, Barueri). Vai substituir a landing page atual (alphavilleodontologia.com.br), com uma página por tratamento para que cada campanha do Google Ads caia na página certa. Foco comercial: implante e prótese. A emergência 24h continua sendo a porta de entrada e segue em destaque na home.

Fase atual: protótipo para aprovar o design. Conteúdo definitivo e tags do Google Ads entram depois.

Quem pede as mudanças é o Lorenzo, que não é programador. Responda em português simples: antes de editar, descreva o plano em poucas linhas; depois, diga o que mudou e o que ele deve conferir no celular.

## Prioridade: celular
A maior parte do tráfego vem do celular. Pense cada mudança primeiro em 390 px de largura e confira também em 360 px e em 1440 px. Área de toque mínima de 44 px e contraste de texto mínimo de 4,5:1.

## Estrutura
- HTML estático publicado na Vercel: index.html, sobre-o-doutor.html, pacientes.html, faq.html, contato.html, tratamentos.html e tratamentos/*.html.
- Estilos compartilhados em style.css, pages.css e design-system.css (o padrão visual novo). Menu e rodapé vêm de components.js; FAQ e carrosséis, de pages.js.
- Nunca rode generate_treatments.js nem os scripts fix_*.js, extract_urls.js, fetch_css.js e find_blob.js: eles reescrevem páginas e apagariam o trabalho feito à mão.
- Não apague arquivos e não adicione biblioteca, framework ou dependência sem perguntar.
- Imagem nova em WebP, com no máximo 1600 px no lado maior; a imagem do primeiro bloco carrega com prioridade e as outras com loading="lazy".

## Padrão visual
A referência é tratamentos/implantes-dentarios.html do segundo bloco para baixo (o primeiro bloco está sendo redesenhado). O padrão fica em design-system.css; use as variáveis e classes de lá em vez de cores e fontes soltas.
- Fontes: Outfit, com títulos em peso leve, e Cormorant Garamond itálico para a palavra de destaque do título.
- Cores: azul-marinho #010E30; dourado #F9BD7B para destaques sobre fundo escuro; dourado escuro #E0A04E; bronze #C09A6B para linhas e detalhes; creme #FDF6ED e #F8EFE2 nos cartões; fundo claro #F5F7FA; textos #1A2332 e #5A6475.
- Texto dourado sobre fundo claro usa #8A6A3F (rótulos) ou #A8814F (destaques grandes), porque #C09A6B não tem contraste suficiente.
- Cor nova, fonte nova ou estilo inline repetido só com aprovação.

## Regras de conteúdo
1. Depoimento só real: avaliação do Google copiada sem edição, com primeiro nome e inicial do sobrenome, mês e ano e link para o perfil. Nunca invente nem "melhore" depoimento. Avaliações de familiares não entram.
2. Cada número com o dono certo: 29 anos e 10.000+ pacientes são do Dr. Eduardo; 15+ anos em implantodontia e 5.000+ implantes são do Dr. Luis.
3. "Especialista" só para especialidade registrada no CRO, com nome e número do profissional.
4. Sem promessa de resultado ("sem dor", "você não sente nada", garantias). Sedação e anestesia aparecem como recursos de conforto.
5. Toda frase sobre o 24h tem de ser verdade às 3h de um domingo.
6. Sem preço, desconto, "gratuito" ou condição de pagamento.
7. Foto de paciente só com autorização assinada, sem nome de paciente conhecido.
8. Rodapé com nome e CRO do responsável técnico e da clínica (dados a confirmar).

## Pessoas e fatos (não invente além disto)
- Dr. Eduardo Martinusso, CRO 61.226: dono do consultório, 29 anos de experiência, clínico geral com foco em dentística estética e endodontia. Responde o WhatsApp e faz as avaliações.
- Dr. Luis Marcos Carrijo, CRO-SP 84.569: especialista em implantodontia, formado pela USP, 30 anos de carreira, mais de 15 em implantodontia, mais de 5.000 implantes, cirurgia guiada e carga imediata. Faz as cirurgias de implante.
- Dra. Clery Saad Abboud, CRO 44.596: laserterapia e acupuntura.
- Implante: o paciente chama no WhatsApp, faz a avaliação com o Dr. Eduardo e a cirurgia com o Dr. Luis; tem suporte 24h no pós-operatório.
- WhatsApp 5511978201000, sempre com mensagem pronta que diga o tratamento.
- Atendimento particular, sem convênio.
