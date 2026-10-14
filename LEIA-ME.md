# Edição dinâmica Brabo com IA — pacote público

Material de estudo de Fernando Araújo / Brabo Space. Versão 2.0 pública.

## Comece aqui

Esta pasta contém uma skill (instruções para a IA) e cinco projetos verticais reunidos em um projeto Remotion. A skill não é um programa de edição nem instala ferramentas sozinha.

1. Extraia a pasta inteira, preservando subpastas.
2. Em um agente com suporte a skills locais, coloque `brabo-edicao-video-dinamica` no diretório de skills indicado por esse agente. O arquivo `SKILL.md` deve permanecer na raiz dela. Atualize a sessão conforme a ferramenta.
3. Se sua IA não carrega skills automaticamente, peça explicitamente que leia `SKILL.md` e os documentos relativos necessários. Dê acesso à pasta; somente mencionar um arquivo que a IA não consegue ler não o envia.
4. Forneça seu vídeo, transcrição/timestamps e direção visual. Informe plataforma, duração/FPS conhecidos e se quer preview ou render final. A IA deve verificar os dados do arquivo.

## Prompt para seu primeiro projeto

> Use a skill brabo-edicao-video-dinamica desta pasta. Leia meu vídeo e timestamps. Planeje as cenas pela intenção da fala, com entrada, ação, resultado e saída. Quero [formato], [estética] e [tipo de entrega]. Preserve minha voz. Use as referências como repertório e adapte as interfaces à minha fala. Confira o sincronismo e explique o que foi validado.

## Abrir as cinco referências

Instale Node.js com npm, compatível com as dependências do projeto. No terminal dentro de `referencias/projeto-remotion`, execute:

```sh
npm ci
npm run dev
```

Escolha ChatGPT, Automatizar-Processo, Bom-Gosto, Internet-Cansada ou Empresa-Light no Remotion Studio. Para conferir tipos: `npm run check`. Para preparar o bundle: `npm run build`. A primeira instalação exige internet; as mídias das cenas estão incluídas. Consulte os requisitos/licença do Remotion para seu uso.

Leia [o índice das referências](referencias/INDICE.md). Cada guia liga o código e os timestamps. Os MP4 incluídos são gravações-fonte; a composição aplica a edição. Não precisa renderizar para estudar. Não há arquivos de YouTube ou seus cortes neste pacote.

## Adaptar para seu conteúdo

Trabalhe numa cópia do projeto. Troque vídeo e transcrição, confirme metadados, refaça beats e eventos e só depois reaproveite componentes. Não basta trocar o MP4: a duração e as palavras do exemplo pertencem a outra fala. Use [a planilha de decupagem](assets/decupagem.csv), [o método visual](references/direcao-e-motion.md) e [a revisão](references/revisao.md).

## Sobre esta distribuição

As cinco composições preservam as cenas dos projetos existentes. Foram reunidas num entry point independente, com mídias relativas. Fontes especiais foram substituídas por alternativas do sistema, sem distribuir arquivos de fontes comerciais; isso pode alterar métricas e quebras. Os exemplos são repertório histórico: a skill pública descreve cuidados adicionais que devem ser aplicados aos novos trabalhos.

A imagem, a voz e a identidade de Fernando fazem parte do material demonstrativo. Para seu conteúdo, use suas próprias mídias e identidade. Marcas e bibliotecas de terceiros mantêm seus respectivos direitos; este pacote não concede direitos sobre elas. Não inclui credenciais, serviços pagos, node_modules ou configurações pessoais. A skill original no sistema foi preservada.


## Verificação desta versão

Skill validada pelo validador de skills; TypeScript e bundle do projeto independente aprovados. Imports locais e links da documentação conferidos. No exemplo Empresa Light, a interpolação de flash foi corrigida para aceitar seus três pontos. Não foi feita uma nova revisão integral dos cinco vídeos com áudio nem novos exports: este pacote entrega as fontes editáveis para estudo no Studio. Revise as quebras após a troca de fontes.
