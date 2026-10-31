# Skyterm Fachada — distribuição

Repositório público de instaladores, manuais e orientações de atualização.
O código-fonte é mantido em repositório privado independente.

## Estado

Infraestrutura de distribuição em preparação. Este README não anuncia uma versão homologada ou uma atualização disponível. Somente releases publicadas e identificadas como aprovadas devem ser usadas em produção.

## Downloads

Consulte [Releases](https://github.com/rodrigobiagi/skyterm_fachada_update/releases).

- `standard-vX.Y.Z`: edição Padrão, com processamento local de IA.
- `partner-vX.Y.Z`: edição Parceiro; identidade e permissões próprias.

Cada entrega deve conter instalador, três manuais (instalação, white label e uso), manifesto e SHA-256. Pacotes grandes podem conter partes numeradas e o script `Reunir-instalador.ps1`. Baixe todas as partes na mesma pasta e execute o script; ele verifica o instalador remontado e não o executa. Reserve espaço também para o EXE completo.

Não trocar de edição durante uma atualização. Os termos Standard/Parceiro identificam a distribuição; a licença Full é uma modalidade de licença, não uma terceira distribuição.

## Atualizar e recuperar

Finalize análises e treinamentos, faça um backup operacional e guarde-o fora da pasta de dados. Confira os manuais e notas da versão antes de instalar.
Não há atualização automática implementada por esta preparação. Veja [Recuperação](RECUPERACAO.md).

Hashes conferem integridade, não identidade do fornecedor. Os pacotes desta etapa não devem ser tratados como manifestos assinados para atualização automática.

## Política de publicação

Versões publicadas não são sobrescritas. Correções recebem novo número. Instaladores anteriores e seus manuais permanecem disponíveis para recuperação, sujeita à compatibilidade dos dados.
Este repositório não recebe código privado, credenciais, chaves, fotos, inspeções, backups de clientes ou modelos privados.
