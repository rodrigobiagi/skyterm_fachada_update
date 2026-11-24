# Histórico de distribuição

## 0.30.5 — 2026-11-24

- Revisão: Salvar e aprovar reúne a gravação dos campos e a decisão técnica. Ocorrências já validadas exibem Salvar alterações; Reabrir revisão retorna a Pendente. Histórico e conferência das marcações preservados.
- Biblioteca técnica: importação de TXT/Markdown longos em partes, sem perda de conteúdo. Títulos como ## Página 222 identificam a numeração impressa para conferência.
- Excluir material retira o documento das novas consultas, preservando original e versões históricas das referências utilizadas.
- Reavaliação da descrição com IA: o formato de resposta só permite as referências fornecidas pela Biblioteca técnica; sem fontes, a resposta não solicita citações. Aplicação e salvamento continuam humanos.

Inclui os manuais de instalação, configuração white label e uso atualizados.
Atualizações incrementais assinadas. Teste integral de atualização e recuperação: 0.30.4 → 0.30.5 → 0.30.4 em cada edição; demais pacotes com assinatura e integridade verificadas. Instaladores completos compilados localmente, sem anexos executáveis nesta release.

A avaliação quantitativa do YOLO permanece pendente: conferir pesos e classes; conjunto independente revisado; métricas por classe, máscaras, tempo e memória; comparação imagem inteira/recortes em RGB e térmica; ajustes ou novos treinos antes de ativar. Esta versão não conclui essa configuração nem treina ou ativa modelos automaticamente.

## 0.30.4 — 24/11/2026

- CPF/CNPJ reconhecidos automaticamente, com máscara e validação ao completar o preenchimento ou sair do campo. Não é mais necessário selecionar o tipo de documento.
- Fotografias mantêm tamanho e posição ao editar, salvar ou aprovar ocorrências. Campos técnicos e navegação ficam mais compactos em telas estreitas.
- Biblioteca técnica opcional em Configurações: importação de PDF/TXT/MD, conferência, ativação explícita e referências com fonte, edição, página e trecho. Sem biblioteca ativa, o funcionamento habitual é mantido.
- Inicializador reorganizado, com estados de OpenAI e Claude em linhas separadas e ações alinhadas.
- Ajuda e manuais de instalação, configuração white label e uso atualizados.
- Reavaliar descrição com IA para qualquer classificação: comparar a sugestão, aplicar ou manter o texto atual. A consulta é explícita; a revisão humana continua necessária para salvar/aprovar.
- Biblioteca consultada na análise, reavaliação e preparação da minuta. Digitalizações permitem transcrição manual ou OCR de uma página por solicitação explícita de IA.
- YOLO pode apresentar candidatos próprios como sugestões pendentes, com origem, conflitos e métricas de contribuição visíveis. Não há treino/ativação automática nem afirmação de ganho de acurácia; a avaliação quantitativa com conjunto independente permanece pendente.
- Atualização/recuperação integral a partir da 0.30.3 em ambas as edições.

## 0.30.3 — 24/11/2026

- Transferências concluídas deixam de manter o painel aberto. Histórico e downloads acessíveis pelo botão Transferências, sem duplicar o progresso na tela da operação.
- Listas de seleção em ordem alfabética pelo texto em português, preservando valores selecionados e códigos internos.
- Ocorrências com códigos curtos consistentes na revisão, edição, marcações, projeções e novos documentos, inclusive em registros antigos/importados.
- Removido Configurar IA do inicializador. As chaves são gerenciadas em Configurações > Inteligência artificial; o inicializador informa separadamente o cadastro de OpenAI e Claude.
- Ajuda e três manuais atualizados por edição.
- No Standard, reprocessamento substitui o conjunto ativo com preservação da versão anterior no histórico; falhas preservam os dados anteriores e pares são salvos juntos. Novos achados exigem revisão.
- Atualização/recuperação integral a partir da 0.30.2 nas duas edições; incrementais assinados e manuais conferidos.

## 0.30.2 — 23/11/2026

- Importação e exportação com progresso por etapa, histórico recolhível e identificação da inspeção. Ocultar o aviso mantém o pacote disponível para download; a remoção do arquivo é separada.
- Corrigidos pacotes consecutivos, retorno à tela, resultados antigos e bloqueio de fechamento durante transferências.
- CPF/CNPJ validados ao completar ou sair do campo, com mensagens junto ao preenchimento. Seletor CPF/CNPJ no cliente; documentos antigos inalterados preservados.
- Sistemas construtivos com seleção múltipla e orientações específicas para novas análises. Inspeções anteriores conservam a orientação até adoção explícita; filas em andamento, revisões e geometrias humanas preservadas.
- Corrigidos os links Criar chave de OpenAI e Claude. Ajuda e manuais atualizados.
- Atualização/recuperação integral verificada somente a partir da 0.30.1 nas duas edições; incrementais assinados com integridade conferida e seis manuais incluídos.

## 0.30.1 — 24/11/2026

- Correção de interface: o item Profissionais responsáveis do menu lateral de Configurações não quebra mais em duas linhas.
- Atualização/recuperação integral verificada a partir da 0.30.0 nas duas edições; incrementais assinados com integridade conferida. Manuais da versão incluídos.

## 0.30.0 — 23/11/2026

- Importação e exportação de inspeções em segundo plano, com barra de progresso e painel visível em qualquer tela.
- CPF e CNPJ com máscara e validação, incluindo o CNPJ alfanumérico; cadastros existentes preservados.
- Menu Ajuda com o conteúdo dos manuais e perguntas frequentes; correções de interface em janelas estreitas, contraste e Profissionais responsáveis.
- Análise avulsa sem travar a tela; exportação Detect não trata Indeterminado aprovado como fundo; escritas de outro site recusadas.
- Atualização/recuperação integral verificada a partir da 0.29.1 nas duas edições; incrementais assinados com integridade conferida. Manuais da versão incluídos.

## 0.29.1 — 23/11/2026

- Análises com Claude (Anthropic) passam a solicitar o contorno de cada ocorrência, como já ocorria com a OpenAI; antes, a revisão podia exibir apenas o retângulo automático da BBox.
- Requisições à OpenAI, prompts e dados existentes inalterados. Revisões humanas e geometrias preservadas.
- Atualização/recuperação integral verificada a partir da 0.29.0 na edição Standard; incrementais assinados com integridade conferida nas duas edições. Manuais da versão incluídos.

## 0.29.0 — 23/11/2026

- Provedor de IA configurável: OpenAI (padrão, GPT-5.6) ou Claude, da Anthropic (Claude Opus 5.5 ou Sonnet 5.5), escolhido separadamente para a análise de imagens (Standard) e para a redação do laudo (Standard e Parceiro).
- Nova seção Configurações > Inteligência artificial, também aberta pelo botão Configurar IA da janela do aplicativo: cadastrar, trocar, remover e testar chaves; modelo por tarefa; detalhe da imagem e segundas passadas com estimativa de chamadas. A troca de chave vale sem reiniciar.
- Chaves continuam criptografadas pelo Windows, não voltam ao navegador e não entram em backups nem em pacotes de intercâmbio. A chave OpenAI já cadastrada continua válida. Chaves Claude devem ser criadas dentro de um workspace do Claude Console.
- Cada análise e minuta registra o provedor e o modelo utilizados. Revisões humanas, geometrias, relatórios e dados existentes preservados.
- Atualização/recuperação integral verificada a partir da 0.28.32 em cada edição; incrementais assinados com integridade conferida e seis manuais atualizados.

## 0.28.32 — 22/11/2026

- Standard: fluxo unificado de criação, validação e configuração do treinamento RGB/térmico; dataset e tarefa preservados na passagem ao treino.
- Inspeções de teste podem ser excluídas dos próximos datasets sem apagar fotos ou revisões. Cópias idênticas são consolidadas quando as anotações coincidem; divergências ficam fora e são informadas para revisão.
- Botões e campos rotulados, busca de inspeções, estado de seleção, opções avançadas recolhidas e preset de teste curto.
- Revisões humanas, geometrias, relatórios e dados existentes preservados. Parceiro continua sem treinamento YOLO local.
- Atualização/recuperação integral verificada a partir da 0.28.31 em cada edição; incrementais assinados com integridade conferida e seis manuais atualizados.

## 0.28.31 — 22/11/2026

- Corrige os botões de confirmação e salvamento ao trocar entre regiões na projeção térmica na RGB.
- Coordenadas percentuais fracionárias válidas passam a ser aceitas sem arredondar a geometria; valores vazios ou fora de 0–100% continuam bloqueados.
- Atualiza o estado dos controles após salvar e ao terminar de arrastar um vértice.
- Manuais atualizados. Atualizador inalterado; teste integral de atualização e recuperação a partir da 0.28.30 em Standard e Parceiro.

## 0.28.30 — 22/11/2026

Projeções térmicas visíveis na revisão RGB, com camada e estados próprios; responsável obtido da inspeção sem campo repetido; editor reutilizado com retorno sem duplicação de abas; organização de imagens, ferramentas e decisões; lupa legível e redimensionável nos temas claro e escuro.

Sessenta incrementais assinados (30 bases por edição). Teste integral somente 0.28.29 → 0.28.30 → 0.28.29 em Standard e Parceiro; assinatura e integridade conferidas em todos os pacotes. Três manuais por edição. Instaladores completos distribuídos separadamente.

## 0.28.29 — 21/11/2026

- Projeção de máscaras térmicas revisadas sobre a RGB nas edições Standard e Parceiro, com alinhamento por referências do par e sem nova localização pela IA.
- Ajuste manual, identificação do revisor e aprovação explícita antes da inclusão em documentos. Origem térmica identificada; invalidação quando a origem muda. Originais, revisões e datasets preservados.
- Instaladores completos compilados localmente. Distribuição pública somente de incrementais assinados, manuais e metadados de integridade.
- Teste integral de atualização/recuperação somente a partir da 0.28.28 nas duas edições; assinatura e integridade de todos os pacotes verificadas. SAM2 continua desativado por padrão.

## 0.28.28 — publicada em 21/11/2026

- **Separar em nova ocorrência:** em Editar ocorrência, escolha uma marcação de uma ocorrência com dois ou mais segmentos. O segmento passa a ter código, classificação e informações próprios. Geometria e histórico são preservados; origem e destino voltam para revisão. Cancelamento não grava e conflitos entre janelas impedem sobrescrita.
- **Formulários padronizados:** Elemento, Sistemas envolvidos, Localização, Incerteza ou limitação, Classificação da ocorrência, Descrição e Observações/Justificativa. Classificações em ordem alfabética, mantendo códigos internos e registros anteriores.
- Inclusão e edição da incerteza/limitação, inclusive sua remoção. Alterar classificação ou limitação mantém a exigência de justificativa; elemento, sistema e localização continuam dispensados.
- **Lupa à direita, abaixo do cabeçalho**, respeitando o cabeçalho próprio das janelas de marcação. Barra de ferramentas da revisão com alturas e espaçamentos alinhados e quebra organizada.
- **Standard: dataset e modelo térmico independentes.** Exportação de caixas ou máscaras revisadas de imagens _T, separada da RGB _V; manifesto por modalidade e verificações de revisão, máscaras, divisão por inspeção e duplicatas.
- Seleção da modalidade e do dataset compatível no treinamento. Importação, registro de candidatos e ativação térmica separados do modelo RGB; treinamento não ativa automaticamente o resultado. É possível desativar a assistência térmica.
- O modelo térmico ativo refina marcações multimodais compatíveis na própria térmica, em pares ou arquivos _T isolados. Sem modelo térmico ativo, continua a análise multimodal. Não transfere coordenadas RGB, não mede temperatura pelas cores e preserva geometrias humanas. Parâmetros numéricos e dispositivo são compartilhados; os pesos são selecionados por modalidade.

## Validação e distribuição

- Testes dirigidos de revisão/edição, dataset, inferência, filas retomáveis, restrições da edição Parceiro, relatórios e laudos aprovados; interface conferida em notebook/desktop e temas claro/escuro. Dados fictícios; nenhuma chamada paga de IA.
- Standard: treinamento térmico real de uma época e inferência CUDA com dados fictícios aprovados. Esse teste valida o funcionamento do fluxo, não a qualidade diagnóstica. Nenhum modelo treinado com dados de clientes acompanha a distribuição; avalie seus candidatos antes de ativá-los.
- Instaladores completos Standard e Parceiro compilados e mantidos somente localmente. Fontes incorporadas, abertura dos executáveis e PDFs dos manuais conferidos.
- Teste integral de atualização e recuperação somente **0.28.27 → 0.28.28 → 0.28.27** nas duas edições. Atualizador inalterado.
- Seis manuais revisados: 128 páginas; 116 equivalentes à versão anterior fora do número da versão. Capas e páginas modificadas conferidas visualmente; PDFs incorporados conferidos por pixels.
- Assinatura e integridade verificadas para 28 bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.27. Cada release contém 60 anexos: 28 incrementais, 28 manifestos assinados, três manuais e lista SHA-256.
- Releases e bundles anteriores preservados. Sem nova configuração manual ou alteração do portal de licenças. Revisão humana e compatibilidade preservadas; SAM2 permanece desativado por padrão. A edição Parceiro mantém seu escopo sem treinamento/inferência local.

## 0.28.27 — publicada em 20/11/2026

- **Filtro exclusivo do relatório por classificação:** seção expansível com todas as categorias, quantidades revisadas e seleção múltipla. Permite emitir, por exemplo, somente Destacamento e Desplacamento.
- PDF, totais, marcações das fotos e galeria respeitam a classificação final da revisão. Pares elegíveis acompanham como referência; classificações excluídas não recebem marcações. Seleção sem achados elegíveis é recusada. Alterar o filtro exige nova prévia. O laudo e as análises originais permanecem independentes.
- Catálogo central para nomes, opções de classificação, vocabulário da IA, cores e considerações técnicas. Códigos legados e índices existentes dos modelos YOLO preservados; cadastrar uma categoria não treina automaticamente um modelo.
- **Revisão do par acima das imagens**, com detalhes expansíveis e navegação de ocorrências na coluna direita.
- Etapas da inspeção com cores de conclusão/etapa atual; logo proporcional uniforme, mantendo cabeçalho de 122 px e logo de 64 px até 260 px de largura.
- Botões de ocorrência uniformes em duas colunas no painel estreito; espaçamento corrigido entre o pacote de importação e Conferir pacote.

## Validação e distribuição

- Testes dirigidos de classificação, relatórios/galeria, proteção da prévia, laudos, importação, dataset/YOLO e revisão aprovados. Interface conferida em notebook e desktop, temas claro/escuro, com dados fictícios e sem chamadas pagas de IA.
- Instaladores completos Standard e Parceiro compilados e mantidos somente localmente; fontes incorporadas e abertura dos executáveis conferidas.
- Teste integral de atualização e recuperação somente **0.28.26 → 0.28.27 → 0.28.26** nas duas edições. Atualizador inalterado.
- Seis manuais atualizados: capas e páginas modificadas revisadas visualmente; 123 das 125 páginas equivalentes à versão anterior fora do número da versão. PDFs incorporados conferidos por pixels.
- Assinatura e integridade dos incrementais para 27 bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.26. Cada release contém 58 anexos: 27 incrementais, 27 manifestos assinados, três manuais e lista SHA-256.
- Releases e bundles anteriores preservados. Não há nova configuração manual ou atualização do portal de licenças. Revisão humana e geometrias preservadas; SAM2 permanece desativado por padrão.

## 0.28.26 — publicada em 20/11/2026

- Cabeçalho global com **122 px de altura** nas telas principais.
- Logo com **64 px de altura** e largura adaptável, limitada a **260 px**, preservando suas proporções.
- Logo, subtítulo e navegação alinhados; a disposição compacta permanece dentro dos mesmos 122 px.

## Validação e distribuição

- Validação funcional simplificada conforme solicitado: conferência visual e das medidas em 1366 × 768 e 1024 × 768, além da revisão do diff. Baterias amplas de funcionalidades não foram repetidas para esta alteração visual.
- Compilações Standard e Parceiro verificadas, com conferência das fontes incorporadas e abertura dos executáveis.
- Teste integral de atualização e recuperação somente **0.28.25 → 0.28.26 → 0.28.25** nas duas edições. Atualizador inalterado.
- Seis manuais com a versão atualizada: capas conferidas visualmente e 125 páginas comparadas com a edição anterior, excluindo apenas a grafia do número da versão. PDFs incorporados aos instaladores conferidos por pixels.
- Assinatura e integridade conferidas para 26 bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.25. Cada release contém 56 anexos: 26 incrementais, 26 manifestos assinados, três manuais e lista SHA-256.
- Instaladores completos mantidos somente localmente. Releases e bundles anteriores preservados. Não há configuração manual nova nem alteração no portal de licenças, dados, revisão humana, geometrias ou relatórios. SAM2 permanece desativado por padrão.

## 0.28.25 — publicada em 20/11/2026

- **Cabeçalho uniforme:** logo, subtítulo, menu e versão mantêm tamanho e posição nas telas principais. A barra de rolagem deixa de deslocar o cabeçalho; janelas menores usam o mesmo padrão de duas linhas. O modo ampliado da revisão mantém seu comportamento de ocultação explícita.
- **Navegação com contexto:** Inspeções permanece destacada na revisão vinculada e na importação; Análise avulsa identifica a revisão independente. Configurações possui título e navegação local consistentes, com indicação acessível da seção ativa.
- **Ações mais diretas:** Excluir inspeção fica ao lado de Abrir inspeção, com menor destaque visual e confirmação preservada. Ações da foto reúne reprocessar e excluir na Standard; a Parceiro apresenta exclusão direta, sem menu de um único item.
- **Manuais atualizados:** instalação, uso e configuração white label acompanham os novos caminhos da interface.

## Após atualizar

- Não há configuração manual nova nem atualização do portal de licenças. Dados, originais, geometrias, revisão humana, lupa, editores de ponto/caixa/máscara e documentos históricos são preservados. SAM2 continua desativado por padrão.

## Validação e distribuição

- 40 testes Python pertinentes aprovados: contexto de navegação nas duas edições, exclusão, aparência, marca e layout da revisão. Sem chamadas pagas de IA ou uso de dados reais.
- Conferência visual com dados fictícios: oito rotas em notebook 1366 × 768 e desktop 1920 × 1080, temas claro/escuro e janela compacta 1024 × 768. Cabeçalho e navegação com medidas iguais entre telas; filtros e menus conferidos. Não constitui auditoria completa com leitores de tela.
- Seis manuais comerciais, 125 páginas, revisados visualmente; PDFs incorporados aos instaladores conferidos por comparação de pixels.
- Teste integral somente **0.28.24 → 0.28.25 → 0.28.24** nas duas edições: aplicação, abertura, recuperação, integridade restaurada e preservação de arquivos não gerenciados. Atualizador inalterado; matriz integral histórica não repetida.
- Assinatura e integridade verificadas para 25 bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.24. Cada release contém 54 anexos: 25 incrementais, 25 manifestos assinados, três manuais e lista SHA-256.
- Instaladores completos compilados e mantidos somente localmente. Releases e bundles anteriores preservados.

## 0.28.24 — publicada em 20/11/2026

- **Mais espaço para as imagens:** cabeçalho compacto, informações auxiliares recolhidas e fotografias ajustadas à área disponível. O modo ampliado preserva os atalhos para a inspeção e para Fotos e Revisão.
- **Par estável:** RGB sempre à esquerda e térmica à direita, mesmo ao trocar a imagem ativa. Cabeçalhos alinhados e indicação explícita de qual imagem recebe a marcação.
- **Navegação persistente:** identificação, filtro e botões anterior/próxima permanecem visíveis acima do painel de ocorrências. A navegação leva ao início do cartão; botões sem destino ficam desabilitados.
- **Pendências consistentes:** o filtro Com qualquer pendência reúne decisões, campos técnicos incompletos e máscaras desatualizadas, usando os mesmos dados salvos dos indicadores. Aguardando decisão é um filtro separado. A confirmação de fotos sem ocorrências continua acessível pelo cartão e pelos indicadores.
- **Legibilidade e acessibilidade:** textos auxiliares maiores, modos de visualização com estado selecionado exposto às tecnologias assistivas e legendas das marcações dimensionadas para a tela. Claro, Escuro e Sistema preservados.

## Após atualizar

- Sem configuração manual nova ou atualização do portal de licenças. Filtrar e navegar não salvam campos nem aprovam ocorrências. Dados, originais, geometrias, revisão humana, lupa, editores de ponto/caixa/máscara e documentos históricos permanecem preservados. SAM2 continua desativado por padrão.
- O ajuste de legendas é exclusivo da visualização da revisão; mantém as dimensões da imagem e as coordenadas. A renderização padrão dos relatórios e entregas permanece preservada.

## Validação e distribuição

- 71 testes Python pertinentes aprovados, além de 35 casos de edição por ponteiro e verificações JavaScript dos indicadores. Sem chamadas pagas de IA ou uso de dados reais.
- Conferência da revisão com dados fictícios em notebook 1366 × 768 e desktop 1920 × 1080, nos temas claro e escuro: par, imagem ativa, filtros, navegação, campos não salvos, lupa, área ampliada e janelas de nova/edição de ocorrência.
- Seis manuais comerciais, 125 páginas, revisados visualmente; PDFs incorporados aos instaladores conferidos por comparação de pixels.
- Teste integral somente **0.28.23 → 0.28.24 → 0.28.23** nas duas edições, incluindo aplicação, abertura, recuperação, integridade restaurada e preservação de arquivos não gerenciados. Atualizador inalterado; matriz integral histórica não repetida.
- Assinatura e integridade verificadas para 24 bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.23. Cada release contém 52 anexos: 24 incrementais, 24 manifestos assinados, três manuais e lista SHA-256.
- Instaladores completos compilados e mantidos somente localmente. Releases e bundles anteriores preservados.

## 0.28.23 — publicada em 15/11/2026

- Cadastro e edição da inspeção organizados em identificação, profissionais e dados da inspeção. Campos opcionais **WhatsApp ou telefone do cliente** e **CPF/CNPJ**, com máscaras, validação de tamanho e preservação na exportação/importação. Telefones aceitam DDD com dez ou onze dígitos; CPF onze e CNPJ quatorze. Sem inclusão automática desses campos nos PDFs.
- Responsável pela inspeção e responsável pela revisão/relatório exibem somente o nome. Operador de drone exibe nome e ID SARPAS na própria seleção, sem repetição. Responsável técnico pelo laudo mantém os dados profissionais. **Informações complementares dos documentos** estão no **Resumo**, expandidas por padrão.
- Revisão com ferramentas e indicadores compactos, mais espaço para as imagens, motivos claros para pendências e acesso direto ao campo que precisa de preenchimento. Rótulos **Aprovar marcação** e **Aprovar ocorrência** distinguem as decisões. Ajustes de contraste nos temas Claro, Escuro e Sistema; navegação principal renomeada para **Análise avulsa**.
- Laudo organizado em cinco etapas: **Conferir dados → Preparar minuta → Revisar conteúdo → Conferir PDF → Emitir entrega**. Resumo das fotos incluídas e excluídas segue a regra efetiva do PDF. Estados de minuta salva, atualizada e desatualizada ficam explícitos; confirmações humanas e histórico continuam preservados.
- **Pausa por falta de créditos na preparação da minuta**, com etapas concluídas preservadas e botão **Retomar preparação**, inclusive após fechar e reabrir o aplicativo. Somente etapas compatíveis são reutilizadas; dados, revisão, instruções, modelo ou contexto diferentes exigem nova preparação. Uma chamada interrompida sem resultado válido precisa ser refeita. A minuta anterior só é substituída após sucesso integral.

## Após atualizar

- Não há configuração manual nova nem atualização necessária do portal de licenças. Cadastros antigos, originais, revisões humanas, geometrias e documentos históricos permanecem preservados. SAM2 continua desativado por padrão.
- Preparar e retomar a minuta consomem créditos nas chamadas necessárias. Salvar textos, conferir o PDF e emitir não fazem nova chamada à IA. A retomada é uma ação explícita depois de regularizar o saldo ou limite.

## Validação e distribuição

- Testes pertinentes de laudo, cadastro, contatos, portabilidade e revisão aprovados; bateria final de 24 testes Python, seis cenários JavaScript do laudo e verificações de indicadores e máscaras. Falta de créditos, reinício, retomada, entradas incompatíveis e concorrência simulados sem chamadas pagas.
- Interface conferida com dados fictícios em notebook, desktop e formulário estreito, nos três temas. Fluxo de pausa/reinício/retomada, salvamento, prévia e emissão conferido. O aceite do aplicativo instalado e dos links em leitores de PDF permanece com o responsável.
- Seis manuais comerciais, 123 páginas, atualizados e revisados visualmente; conteúdo incorporado aos instaladores conferido.
- Teste integral de atualização, abertura, recuperação e nova abertura somente **0.28.22 → 0.28.23 → 0.28.22**, nas duas edições. Atualizador inalterado; matriz integral histórica não repetida.
- Assinatura e integridade verificadas para 23 bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.22. Cada release contém 50 anexos: 23 incrementais, 23 manifestos assinados, três manuais e lista SHA-256.
- Instaladores completos compilados e mantidos somente localmente. Releases e bundles anteriores preservados.

## 0.28.22 — publicada em 15/11/2026

- Relatório, laudo e pacote de entrega utilizam a mesma seleção fotográfica: fotos com ocorrências aprovadas ou corrigidas e revisão concluída, acompanhadas da referência RGB/térmica quando aplicável. Fotos isoladas sem ocorrências e fotos com apenas ocorrências rejeitadas não entram no registro fotográfico. Os estados de revisão humana e referência do par continuam distintos.
- Uma única barra de progresso junto à ação acionada: preparar minuta, abrir prévia ou finalizar revisão e gerar entrega. Exibe etapas e contagens disponíveis; fica indeterminada quando não há total conhecido. Os controles são liberados novamente após conclusão ou erro.
- Menor retenção de imagens decodificadas durante a geração do PDF, com limpeza dos arquivos temporários. Na amostra sintética de 64 imagens 4K com marcações, o pico do processo isolado caiu de 541,2 MB para 182,2 MB; as 72 páginas permaneceram visualmente idênticas. Esse resultado não representa a memória total do aplicativo com YOLO nem estabelece requisitos mínimos de hardware.
- Mantidos o PDF otimizado e os links para imagens em alta resolução, já disponíveis na 0.28.21 também para o laudo. Ao incluir imagens com marcações, extraia todo o ZIP e preserve a pasta **imgs** e **Abrir_imagens.html**. Os links locais no PDF dependem do leitor; no navegador, use a galeria offline. O ZIP pode continuar grande pelas imagens em alta resolução.

## Após atualizar

- Se a seleção de fotos de uma minuta existente mudar, prepare uma nova minuta explicitamente e confira uma nova prévia. A geração com IA consome créditos; documentos e entregas históricos permanecem intactos.
- Não há configuração manual nova nem atualização necessária do portal de licenças. Originais, dados, revisões humanas e geometrias preservados. SAM2 permanece desativado por padrão.

## Validação e distribuição

- 98 testes Python pertinentes das correções aprovados; na preparação final da versão, oito testes focados e seis cenários JavaScript passaram. Sem chamadas pagas de IA nos testes.
- Seis manuais comerciais, 119 páginas, atualizados e revisados visualmente; os manuais incorporados aos instaladores foram conferidos.
- Testes integrais de atualização, abertura e recuperação: **0.28.21 → 0.28.22 → 0.28.21**, nas duas edições. Atualizador inalterado; matriz integral histórica não repetida.
- Assinatura e integridade verificadas para 22 bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.21. Cada release contém 48 anexos: 22 incrementais, 22 manifestos assinados, três manuais e lista SHA-256.
- Instaladores completos compilados e mantidos somente localmente. Releases e bundles anteriores preservados. Faça o backup operacional habitual antes de atualizar.
- Os fluxos de progresso passaram em testes automatizados de sucesso e falha; PDFs foram renderizados e comparados. O aceite interativo da tela instalada e da abertura dos links em leitores de PDF permanece com o responsável.

## 0.28.21 — publicada em 14/11/2026

- Indicadores de revisão na tela do par RGB/térmico, atualizados após salvar, com decisões pendentes, campos técnicos e acesso à pendência. Alterações não salvas, referência do par e revisão humana são estados distintos. Posição de navegação separada das contagens da inspeção.
- Revisão concluída — minuta desatualizada: campos atuais separados das pendências da minuta anterior. Orientação para preparar uma nova minuta, com geração por IA explícita e nova conferência. Bloqueios de emissão preservados.
- PDF otimizado; ao incluir marcações na entrega, imagens em alta resolução em imgs e galeria offline Abrir_imagens.html por Localização. Links relativos no PDF para leitores compatíveis; no navegador, usar a galeria. Extrair o pacote inteiro e manter sua estrutura. Originais preservados; ZIP pode continuar grande.
- Correção da seleção e arraste de vértices na criação de máscara, sem duplicar pontos. Ctrl + arraste preservado.
- 56 testes Python finais pertinentes, 35 casos de ponteiro e teste do JavaScript dos indicadores aprovados, sem chamadas pagas de IA. Seis manuais comerciais, 119 páginas, revisados visualmente. PDF fictício comparado: 2.074.966 → 680.211 bytes; redução varia conforme as imagens.
- Atualização, abertura e recuperação integrais somente 0.28.20 → 0.28.21 → 0.28.20 nas duas edições. Atualizador inalterado. Assinatura e integridade verificadas para 21 bases por edição (0.27.0 a 0.27.3 e 0.28.4 a 0.28.20). 46 anexos por release: 21 incrementais, 21 manifestos, três manuais e SHA-256.
- Conferência interativa da tela e dos links em leitores de PDF permanece pendente: a automação do navegador foi interrompida por não identificar a URL com segurança. Links, galeria e preservação de campos conferidos em testes automatizados; PDFs revisados visualmente.
- Sem configuração manual ou atualização do portal de licenças. Instaladores completos somente locais. Fazer backup operacional antes de atualizar; versões anteriores preservadas.

## 0.28.20 — publicada em 12/11/2026

- Standard: pausa do lote por falta de créditos ou bloqueio financeiro da API. Interrompe novos envios e preserva resultados das chamadas já iniciadas. Limites temporários recebem tentativas limitadas com espera.
- Fila, imagens e configurações persistem após fechar o aplicativo. Retomar processamento continua apenas as pendentes, sem refazer análises concluídas ou substituir revisões humanas. Pares RGB/térmicos preservados. Progresso separado por situação, acesso ao faturamento e descarte da fila pendente sem excluir resultados salvos.
- Recuperação disponível para lotes iniciados na 0.28.20; falhas antigas exigem selecionar novamente apenas fotos não concluídas. Filas ficam no computador de origem e não integram a exportação de inspeção. A 0.28.19 não retoma essas filas. Chamadas interrompidas antes de salvar a resposta podem precisar ser repetidas e gerar consumo.
- Parceiro sincronizado, preservando revisão, importação e documentos; análise de fotos permanece exclusiva da Standard. Sem ajuste manual de configuração ou atualização do portal de licenças.
- 114 testes pertinentes e retomada após reinício conferida na interface com dados fictícios, sem chamadas pagas de IA. Atualização, abertura e recuperação integrais somente 0.28.19 → 0.28.20 → 0.28.19 nas duas edições. Atualizador inalterado; matriz integral histórica não repetida.
- Vinte bases por edição, 0.27.0 a 0.27.3 e 0.28.4 a 0.28.19, com assinatura e integridade verificadas. Cada release contém 44 anexos: vinte incrementais, vinte manifestos, três manuais e lista SHA-256. Seis manuais revisados visualmente, 107 páginas.
- Instaladores completos somente locais. Faça backup operacional antes de atualizar. Bundles e releases anteriores preservados.

## 0.28.19 — publicada em 12/11/2026

- Ctrl + clique e arrastar permite mover a máscara inteira em Nova ocorrência e Editar ocorrência, preservando forma e tamanho dentro da imagem. Edição de vértices, lupa, salvamento explícito e revisão humana preservados.
- Destacamento passa a aparecer como **Desplacamento**; Descolamento aparente passa a aparecer como **Destacamento**. São categorias distintas, aplicadas automaticamente a registros existentes e novos, com os mesmos vínculos, modelos e histórico. Concreto desplacado permanece separado. Não é necessário executar script sobre as inspeções.
- Minutas afetadas precisam ser atualizadas e passar por nova prévia. Textos livres, documentos emitidos e instruções editoriais não são reescritos; confira as referências aos nomes anteriores. Sem ajuste manual de configuração ou atualização do portal de licenças.
- 174 testes e 10 subtestes, 22 casos de eventos de arraste e quatro verificações finais de classificação aprovados. Fluxo visual conferido com dados fictícios. Atualização, abertura e recuperação integrais somente 0.28.18 → 0.28.19 → 0.28.18 nas duas edições. Atualizador inalterado; matriz integral histórica não repetida.
- Dezenove bases por edição, 0.27.0 a 0.27.3 e 0.28.4 a 0.28.18, com assinatura e integridade verificadas. Cada release contém 42 anexos: dezenove incrementais, dezenove manifestos, três manuais e lista SHA-256. Seis manuais revisados visualmente, 106 páginas.
- Instaladores completos somente locais. Faça backup operacional antes de atualizar. Ao retornar à versão anterior, voltam os nomes e os controles daquela versão.

## 0.28.18 — publicada em 11/11/2026

- Corrigida a lupa da tela de revisão que abria sem mostrar a fotografia. Os temas preservam imagem ampliada, zoom e acompanhamento do cursor. Validação com RGB e térmica nos temas Claro, Escuro e Usar tema do sistema.
- Lupa de Nova ocorrência e Editar ocorrência, marcações humanas, revisões e documentos preservados. Sem ajuste manual de configuração ou atualização do portal de licenças.
- Quatro testes direcionados de aparência e preparação do build aprovados. Atualização, abertura e recuperação integrais somente 0.28.17 → 0.28.18 → 0.28.17 nas duas edições. Atualizador inalterado; matriz integral histórica não repetida.
- Dezoito bases por edição, 0.27.0 a 0.27.3 e 0.28.4 a 0.28.17, com assinatura e integridade verificadas. Cada release contém 40 anexos: dezoito incrementais, dezoito manifestos, três manuais e lista SHA-256. Seis manuais revisados visualmente, 104 páginas.
- Instaladores completos somente locais. Faça backup operacional antes de atualizar. Ao retornar à 0.28.17, a falha visual da lupa da revisão pode reaparecer.

## 0.28.17 — publicada em 11/11/2026

- Geração de laudos extensos em lotes automáticos, reunidos em uma única minuta. Escopos pequenos mantêm uma chamada. Fotos não são reenviadas nem reanalisadas.
- Conclusões e recomendações individuais preservam os vínculos com as ocorrências revisadas. Cobertura exata dos IDs, exclusões de recomendações e revisão humana mantidas. Resumos parciais alimentam a análise integrada, sem substituir os textos individuais.
- Etapas válidas concluídas ficam salvas neste computador e podem ser reaproveitadas em nova tentativa com os mesmos dados, instruções, contexto, modelo e revisão. Falhas ou alterações concorrentes preservam a minuta anterior. Não há repetição automática de chamadas.
- Progresso identifica lote e consolidação. A interface explica tempo e consumo da API; novas chamadas consomem créditos. Salvamento aceita minutas maiores, mantendo o formato e o limite de 1.000 ocorrências.
- Manual de uso inclui legenda dos 12 Elementos, identificação visual, distinção de Sistemas envolvidos e orientações de laudos em etapas. Seis manuais revisados visualmente, 104 páginas.
- 492 testes e 10 subtestes aprovados, mais 60 testes direcionados após o ajuste final. Rotas da aplicação verificadas com 35 ocorrências, falha, retomada, preservação da minuta e prévia de 26 páginas, com IA simulada.
- Atualização e recuperação integrais somente 0.28.16 → 0.28.17 → 0.28.16 nas duas edições. Atualizador inalterado. Dezessete bases por edição, 0.27.0 a 0.27.3 e 0.28.4 a 0.28.16, com assinatura e integridade verificadas. Cada release contém 38 anexos: dezessete incrementais, dezessete manifestos, três manuais e lista SHA-256.
- Instaladores completos somente locais. Sem ajuste manual de configuração ou atualização do portal de licenças. Ao retornar à 0.28.16, voltam o fluxo de geração e o limite de salvamento anteriores. Faça backup operacional e confira a minuta completa e uma nova prévia antes de emitir.

## 0.28.16 — publicada em 11/11/2026

- Elemento, Sistemas envolvidos e Localização podem ser alterados sem justificativa, inclusive em ocorrências aprovadas. Os três campos continuam necessários para emitir o laudo.
- Alterações efetivas de Classificação da ocorrência ou Incerteza ou limitação exigem explicação da nova decisão. Salvar sem mudança nesses campos dispensa nova justificativa. Geometrias realmente alteradas continuam exigindo confirmação humana; alterações somente de metadados deixam de ser sinalizadas como mudanças de geometria.
- Descrição editável acima de Observações/Justificativa nas ocorrências dos dois lados do par RGB/térmico. Texto existente, edições e remoção são persistidos; formulários anteriores preservam a descrição. Histórico e proteção contra sobrescrita mantidos.
- Novas sugestões de Elemento pela IA usam a lista atual de 12 opções. Cerâmico e argamassado são sistemas envolvidos. Sem identificação segura, a seleção fica para o revisor. Valores antigos continuam legíveis e não são convertidos automaticamente.
- Cabeçalho completo em Revisão e Análise avulsa, com logo e subtítulo no padrão de Inspeções. Ampliar/Restaurar área de revisão permanece disponível.
- Dezesseis bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.15. Cada release inclui dezesseis incrementais, dezesseis manifestos assinados, três manuais e lista SHA-256. Instaladores completos somente locais.
- 478 testes e 10 subtestes aprovados, mais onze testes direcionados após o último ajuste do cartão de Elemento. Atualização e recuperação integrais somente a partir da 0.28.15 nas duas edições; demais bases verificadas por assinatura e integridade. Atualizador inalterado. Seis manuais revisados visualmente, 98 páginas.
- Sem ajuste manual de configuração ou atualização do portal de licenças. Após modificar dados das ocorrências, atualize a minuta e confira nova prévia. Ao retornar à 0.28.15, voltam as regras anteriores de justificativa e apresentação dos campos/cabeçalho.

## 0.28.15 — publicada em 11/11/2026

- Correção da emissão do laudo com responsável pela revisão da inspeção, preservando autores e datas históricos. Campos técnicos ausentes aparecem no checklist, com imagem e ocorrência identificadas.
- Indicadores calculados pela revisão atual, antes ou depois da minuta: Elemento, Sistemas envolvidos e Localização, contagens de ocorrências e campos, links diretos e pendências documentais. Fotos pendentes excluídas e referências do par identificadas separadamente.
- Botão Fotos e Revisão ao lado de Voltar à inspeção; atualização dos indicadores ao retornar após corrigir dados. Confirmações humanas permanecem obrigatórias.
- Contraste corrigido em avisos temporários, cartões de segmentos e status da licença nos temas Claro, Escuro e Sistema. Fotografias, marcações e documentos preservados.
- Quinze bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.14. Cada release inclui quinze incrementais, quinze manifestos assinados, três manuais e lista SHA-256. Instaladores completos somente locais.
- 467 testes e 10 subtestes aprovados, mais seis testes direcionados após a atualização das referências de cache. Atualização e recuperação integrais somente a partir da 0.28.14 nas duas edições; demais bases verificadas por assinatura e integridade. Atualizador inalterado. Seis manuais revisados visualmente, 92 páginas.
- Sem ajuste manual de configuração ou atualização do portal de licenças. Após completar campos técnicos, prepare nova minuta e confira a prévia. Ao retornar à 0.28.14, os novos indicadores e as correções de validação/contraste deixam de estar disponíveis.

## 0.28.14 — publicada em 11/11/2026

- Configurações > Aparência com Claro, Escuro e Usar tema do sistema. Preferência individual, propagada às janelas de ocorrências sem recarregar nem descartar edições. Fotos, paletas térmicas, marcações e apresentação dos documentos preservadas.
- Confirmação de fotos sem ocorrências acessível; cabeçalhos compactos, área de revisão ampliável e divisão ajustável no desktop. Controles adaptados a fotos vazias e singular de pendente corrigido.
- Inspeção com indicadores recolhíveis; ações de documentos antes dos campos complementares; formulário de ocorrência com campos roláveis e ações acessíveis.
- Responsável pela execução retirado de Empresa / Introdução e dos novos documentos. Valor legado preservado; mantidos os responsáveis vinculados à inspeção, revisão/relatório e laudo.
- Quatorze bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.13. Cada release inclui quatorze incrementais, quatorze manifestos assinados, três manuais e lista SHA-256. Instaladores completos somente locais.
- 455 testes e 10 subtestes aprovados, mais 13 testes direcionados após o ajuste final do aviso de referência. Atualização e recuperação integrais somente a partir da 0.28.13 nas duas edições; demais bases verificadas por assinatura e integridade. Atualizador inalterado. Seis manuais revisados visualmente.
- Sem ajuste manual de configuração ou atualização do portal de licenças. Documentos históricos preservados. Ao retornar à 0.28.13, essa versão ignora o tema e pode exibir novamente o responsável institucional legado em novos documentos.

## 0.28.13 — publicada em 11/11/2026

- Cadastro com campos obrigatórios conforme profissão/função; ID SARPAS obrigatório para operadores, inclusive profissionais que acumulam a função. Outro exige especificação; sem Analista. CPF e contatos opcionais.
- Responsável pela inspeção carrega nome e SARPAS; operador pode ser o mesmo ou outro profissional. Revisor emite o relatório; responsável técnico pelo laudo independente, podendo ser a mesma pessoa com perfil compatível. ART/RRT/TRT conforme cadastro.
- Autoria, geometrias humanas e documentos históricos preservados. Importação remapeia os responsáveis sem duplicação. Novos perfis continuam armazenados após recuperação, mas sua edição e os novos vínculos exigem a 0.28.13.
- Treze bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.12. Cada release inclui treze incrementais, treze manifestos assinados, três manuais e lista SHA-256. Instaladores completos somente locais.
- 453 testes e 10 subtestes aprovados; atualização e recuperação integrais somente a partir da 0.28.12 nas duas edições. Demais bases verificadas por assinatura e integridade; atualizador inalterado. Seis manuais revisados visualmente.
- Sem ajuste manual de configuração ou atualização do portal de licenças. Confira os cadastros e selecione os responsáveis na inspeção.

## 0.28.12 — publicada em 11/11/2026

- Responsável pela revisão definido na inspeção, sem preencher o nome em cada ocorrência ou confirmação de foto sem ocorrências. Confirmação humana e histórico de autores/datas preservados.
- Emissor igual ao revisor por padrão, com opção de profissional distinto. Nome do revisor na Identificação do objeto inspecionado, sem repetição nas fichas. Documentos históricos preservados; importação transporta os dois responsáveis.
- Interface com Resumo, Fotos e revisão e Documentos, próxima ação conforme pendências, Mais ações para manutenção/exclusão, lupa inicialmente afastada dos controles e apresentação consistente no editor. Ajuda contextual de processamento e contagem de máscaras corrigida.
- Doze bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.11. Cada release inclui doze incrementais, doze manifestos assinados, três manuais e lista SHA-256. Instaladores completos somente locais.
- 441 testes e 10 subtestes aprovados. Atualização e recuperação integrais somente a partir da 0.28.11 nas duas edições; demais bases verificadas por assinatura e integridade. Atualizador inalterado.
- Nas inspeções existentes, selecione o Responsável pela revisão antes de novas confirmações. Sem alteração manual de configuração ou atualização do portal de licenças.

## 0.28.11 — publicada em 10/11/2026

- Confirmação humana de fotos sem ocorrências com nome e data permite inclusão nos documentos. Reprocessamento invalida a confirmação, preservando o histórico. Referências do par permanecem distintas de revisão humana; fotos com ocorrências pendentes continuam excluídas.
- Cada imagem ou par é seguido das respectivas fichas. Localização em negrito abaixo das imagens e como primeiro campo da ocorrência. Ordem natural crescente dentro do conjunto; conjuntos seguem a primeira localização, sem ordem global estrita entre fichas de conjuntos diferentes.
- Correspondência espacial ausente como Não informada; N/A explícito como Não se aplica.
- Onze bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.10. Cada release contém onze incrementais, onze manifestos assinados, três manuais e lista SHA-256. Instaladores completos permanecem locais.
- 435 testes e 10 subtestes aprovados. Atualização e recuperação integral somente a partir da 0.28.10 nas duas edições; demais bases verificadas por assinatura e integridade. Atualizador inalterado.
- Sem atualização do portal de licenças ou ajuste manual de configuração. Documentos históricos preservados. Ao retornar à 0.28.10, fotos isoladas confirmadas sem ocorrências deixam de ser elegíveis naquela versão, sem apagar fotos ou dados.

## 0.28.10 — publicada em 10/11/2026

- Relatório e laudo incluem a imagem pareada sem ocorrências como referência quando a outra está completamente revisada e possui ocorrência aprovada ou corrigida, nos dois sentidos RGB/térmica.
- Referência identificada e sem marcações; não conta como ocorrência nem confirma ausência de problemas. Fotos com ocorrências pendentes continuam excluídas. Pacote de fotografias usa a mesma regra.
- Atualização direta das dez bases 0.27.0 a 0.27.3 e 0.28.4 a 0.28.9. Cada release contém dez incrementais, dez manifestos assinados, três manuais e lista SHA-256. Instaladores completos permanecem locais.
- Teste integral de atualização e recuperação somente a partir da 0.28.9, nas duas edições. Demais bases: assinatura e integridade dos pacotes; matriz integral histórica não repetida.
- Sem atualização do portal de licenças ou ajuste manual de configuração. Minutas anteriores podem exigir atualização; documentos históricos emitidos permanecem preservados.

## 0.28.9 — publicada em 08/11/2026

- Botão único Editar ocorrência abre a imagem correspondente em janela própria, com ponto, caixa, máscara, ocorrências existentes, seleção de segmento e lupa.
- Formulário preenchido com classificação, elemento, localização, sistemas envolvidos/Outro, descrição e observações/justificativa. Geometria e dados são salvos juntos; códigos e demais segmentos preservados.
- Mudanças em ocorrências aprovadas exigem nova revisão. Proteção contra sobrescrita por janelas antigas; atualização da tela principal mantém campos ainda não salvos.
- Nove bases por edição: 0.27.0 a 0.27.3 e 0.28.4 a 0.28.8. Cada release inclui nove incrementais, nove manifestos assinados, três manuais e lista SHA-256. Instaladores completos permanecem locais.
- Sem atualização do portal de licenças ou ajuste manual de configuração.

## 0.28.8 — publicada em 08/11/2026

- Relatório e laudo com fichas em ordem natural crescente por Localização: torre, fachada, passada e andar. Sufixo após o andar ignorado; campos vazios ao final; identificadores e vínculos preservados.
- Standard: parâmetros YOLO em Configurações > Processamento, com descrições, listas, validação numérica e confiança por classificação. Aceita 0.25 ou 0,25 e recusa 25 para confiança. Preferências por usuário e aplicação nas próximas análises; sem edição manual de arquivos.
- Atualização direta e retorno nas bases 0.27.0 a 0.27.3 e 0.28.4 a 0.28.7, nas duas edições. Cada release inclui oito incrementais, oito manifestos assinados, três manuais e lista SHA-256. Instaladores completos permanecem locais.
- Não requer atualização do portal de licenças. Revisão humana, geometrias e histórico emitido preservados.

## 0.28.7 — publicada em 07/11/2026

- Janela unificada para criar e complementar ocorrências por Ponto, Caixa ou Máscara, com Localização e Sistemas envolvidos.
- Exibição das ocorrências existentes da imagem ativa, destaque do complemento, opção de mostrar/ocultar e lupa móvel com tamanho e zoom ajustáveis.
- Atualização direta e retorno verificados em cópias isoladas das bases 0.27.0, 0.27.1, 0.27.2, 0.27.3, 0.28.4, 0.28.5 e 0.28.6, nas edições Standard e Parceiro.
- Cada release inclui sete incrementais assinados, sete manifestos, três manuais e uma lista SHA-256. Os 36 anexos foram conferidos por tamanho e hash remoto. Instaladores completos permanecem fora do GitHub.
- O código F001, F002 etc. identifica a ocorrência; a classificação é um campo separado e permanece associada ao registro.

## 0.28.5 — publicada em 04/11/2026

- Laudo de inspeção de fachadas com cobertura, manutenção, documentação, ensaios opcionais e providências por prioridade. Mapa de danos e memorial podem acompanhar o PDF e o ZIP.
- Atualização direta e retorno verificados nas edições Standard e Parceiro a partir de 0.27.0, 0.27.1, 0.27.2, 0.27.3 e da compilação local 0.28.4. Os dez downloads públicos e as assinaturas foram conferidos.
- Categorias novas podem aparecer como indeterminadas na reversão; voltar à 0.28.5 recupera o termo exato dos registros preservados.
- Cada release inclui cinco incrementais, cinco manifestos assinados, três manuais e a lista SHA-256.

## 0.27.3 — publicada em 31/10/2026

- Versão de continuidade para testar o aviso de atualização ao iniciar a 0.27.2; sem nova mudança funcional.
- Comportamento da 0.27.2 aprovado pelo responsável. Publicação da 0.27.3 autorizada.
- Atualização e retorno dos seis caminhos aprovados em cópias isoladas; consulta pública, assinatura e download integral verificados sem autenticação.
- Incrementais diretos desde 0.27.0, 0.27.1 e 0.27.2 nas duas edições.
- Instaladores completos compilados localmente; distribuição pelo responsável. Nenhum completo ou parte anexado às novas releases.
- Releases contêm apenas incrementais assinados, manuais e hashes, sem links para instaladores completos.

## 0.27.2 — publicada em 31/10/2026

- Consulta de atualizações na inicialização, em segundo plano.
- Janela de aviso com Atualizar agora e Mais tarde quando houver pacote compatível.
- Abertura do atualizador pela janela principal com confirmação e fechamento seguro do aplicativo ocioso.
- Operações em andamento impedem o fechamento; cancelar UAC mantém o aplicativo utilizável. Outras sessões exigem fechamento manual.
- Standard compilado pelo responsável, com link OneDrive nas notas.
- Deltas diretos das bases 0.27.0 e 0.27.1 validados nas duas edições, incluindo retorno. Publicação autorizada pelo responsável.
- Consulta pública, assinatura e download dos quatro pacotes verificados sem autenticação.

## 0.27.1 — publicada em 31/10/2026

- Versão visível no título da janela desktop para conferir atualização.
- Validação do pacote incremental 0.27.0 para 0.27.1 e retorno.
- Standard compilado pelo responsável, com link do instalador no OneDrive nas notas da release.
- Atualização real e retorno validados localmente nas duas edições; pacotes assinados publicados nas releases.
- Sem alteração de formato de dados ou protocolo de licença. Disponível aos clientes compatíveis desde a 0.27.0, por autorização do responsável.
- Consulta pública, assinatura e download integral dos dois deltas verificados sem autenticação.

## 0.27.0 — publicada em 31/10/2026

- Instalador completo inicial com utilitário independente de atualização e recuperação.
- Próximas atualizações podem conter somente arquivos modificados, com manifesto assinado e verificação de integridade.
- Retorno à versão anterior dos arquivos do programa; dados e fotos não são restaurados pelo atualizador.
- Consulta manual, separada por edição, sem credencial GitHub no cliente.
- Instalações anteriores a 0.27.0 precisam do instalador completo. Não há pacote incremental inicial.
- Publicação autorizada após confirmação de teste funcional pelo responsável. Arquivos conferidos por tamanho e SHA-256.
- Manifestos preservam o estado da preparação original; aceite posterior registrado nas notas das releases.

## 31/10/2026 — preparação do canal

- Definida separação entre código privado e distribuição pública.
- Convenção de versões separadas para Padrão e Parceiro.
- Definida preservação das entregas anteriores e orientação de recuperação.
- Nenhum instalador homologado ou atualização automática anunciado nesta etapa.
