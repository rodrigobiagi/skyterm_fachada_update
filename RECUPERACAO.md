# Retorno à versão anterior

O retorno do programa e a recuperação dos dados são operações diferentes.
Reinstalar uma versão anterior não desfaz alterações realizadas nos dados por uma versão nova.

1. Encerre análises, treinamentos e a aplicação.
2. Preserve uma cópia operacional do estado atual, mesmo que haja problema.
3. Consulte as notas da release e confirme com o suporte a compatibilidade da versão anterior com os dados atuais.
4. Use somente o instalador homologado da mesma edição e identidade do produto. Confira os hashes e os manuais correspondentes.
5. Siga o procedimento de reinstalação testado para essa transição. Não selecione a exclusão de dados ao desinstalar.
6. Quando o formato dos dados não permitir retorno direto, restaure o backup pré-atualização conforme orientação. Essa restauração pode não incluir trabalhos posteriores ao backup; preserve-os antes.

As versões distribuídas devem permanecer arquivadas. Uma versão retirada de recomendação não será silenciosamente substituída por outros bytes com o mesmo número.
A partir da 0.27.0, atualizações incrementais compatíveis preservam uma cópia dos arquivos substituídos. O utilitário **Atualização e recuperação**, disponível também no menu Iniciar, pode retornar o programa à versão anterior. Em falha durante a troca, ele tenta restaurar os arquivos; depois de uma interrupção de energia, execute a recuperação antes de abrir o programa. A operação exige o Skyterm fechado e a integridade do backup local.

Essa recuperação não equivale a restaurar dados nem garante downgrade entre quaisquer duas versões. Reinstalações completas, alterações de formato ou backups corrompidos podem exigir assistência.
