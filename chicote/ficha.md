# Chicote — ficha e decisões da refatoração V12

Baseline: 9c6a77397bbb23e3867c0f918470944e85d89881.
Referência visual: taisgb/alexandre-magno-modelo, bloco V12 de style.css (blob 8a406cfb28089e2812d1c2f4615525c706b25a26).
Método: matheusmongarde/chicote, commit ce3d39d9d08b628fa03bc26ef2d350ee0266dde3.

## Ficha
Prévia conceitual para a Dra. Aline Galy, pediatria em Salvador. Público geral: responsáveis por crianças, navegação móvel inclusive aparelho fraco. Ação: escolher consultório e contatar a equipe. Provas existentes: CRM/RQE, três consultórios, opiniões na Doctoralia. Preservar conteúdo, fotografias reais, links de telefone, mapas, Instagram, Doctoralia, FAQ, menu e noindex.

## História e composição
Hero: “Por uma infância leve e desmedicalizada.” (frase original da profissional).
Metáfora: caderneta botânica de crescimento — páginas de papel quente, ilustração de broto, curvas e verdes suaves. Não simular consultório nem pacientes.
- Hero: texto à esquerda, retrato vertical à direita; em mobile fluxo único e CTA antes de credenciais e chips. CTA mínimo 50px; imagem na proporção real 600:785, sem zoom.
- Prova: painel de três informações centralizadas, empilhadas em tela estreita.
- Atendimentos: bento V12, primeira peça maior, quatro cards; broto ilustrativo original em SVG.
- Sobre: foto real e texto descritivo preservado.
- Consulta: sequência de três blocos com leve desnível no desktop, um eixo no mobile.
- Consultórios: três opções com mesma prioridade; endereço, telefone e rota.
- Redes, FAQ e CTA final: confiança, dúvidas e ação; rodapé com identificação e aviso de prévia.
- Costuras: painéis arredondados com recuo 8–16px, luz difusa e faixa de prova sobre a transição da hero. Gradientes cálidos/menta; três níveis de sombra; sem vidro translúcido sobre textos.
- Cabeçalho fixo desktop, menu móvel não fixo; botão flutuante preservado. Alvos 44–50px e textos de leitura 16–17px; movimento reduzido e conteúdo sempre visível.
- Fonte Allo e Fraunces/DM Sans preservadas; uso de noindex intencional por ser prévia não oficial.

## Prompts e imagens
Não há vaga de imagem necessária nesta refatoração: duas fotos originais preservadas byte a byte e uma ilustração botânica SVG criada por código. Não inserir imagem de paciente ou consultório fictício. Se a profissional fornecer novo retrato, manter rosto/corpo originais, enquadramento vertical com folga acima do cabelo, luz difusa e fundo neutro claro.

## Auditoria
Workflow .github/workflows/chicote.yml executa o script oficial com perfil geral/aparelho fraco, baseline congelado e versão atual, nas três larguras do método; relatórios e capturas são artefatos do Actions. Nota de portões /70 somente, rubrica /30 não preenchida sem revisão visual das capturas. Não atribuir nota antes da execução. Não substituir medidas por estimativas.
