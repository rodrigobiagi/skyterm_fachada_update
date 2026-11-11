# Skyterm Fachada — distribuição

Repositório público de atualizações incrementais, manuais e orientações de recuperação.
O código-fonte é mantido em repositório privado independente.

## Estado

Versão atual: **0.28.13**, disponível para [Standard](https://github.com/rodrigobiagi/skyterm_fachada_update/releases/tag/standard-v0.28.13) e [Parceiro](https://github.com/rodrigobiagi/skyterm_fachada_update/releases/tag/partner-v0.28.13).

As releases publicadas identificam a versão de destino, a edição e as versões de origem compatíveis.

## Downloads

Consulte [Releases](https://github.com/rodrigobiagi/skyterm_fachada_update/releases).

- `standard-vX.Y.Z`: edição Padrão, com processamento local de IA.
- `partner-vX.Y.Z`: edição Parceiro; identidade e permissões próprias.

Cada nova entrega inclui pacotes de arquivos alterados, manifestos assinados por versão de origem, três manuais e a lista SHA-256. O responsável distribui os instaladores completos separadamente.

Não trocar de edição durante uma atualização. Os termos Standard/Parceiro identificam a distribuição; a licença Full é uma modalidade de licença, não uma terceira distribuição.

## Atualizar e recuperar

Finalize análises e treinamentos, faça um backup operacional e guarde-o fora da pasta de dados. Confira os manuais e notas da versão antes de instalar.
A versão 0.27.0 introduz um utilitário de atualização e recuperação, publicado após confirmação de teste funcional pelo responsável. Para versões anteriores, a primeira atualização exige instalador completo. Depois, o utilitário pode baixar pacotes incrementais compatíveis e assinados, mediante ação do usuário. Rascunhos e pré-releases não são oferecidos pelo aplicativo. Veja [Recuperação](RECUPERACAO.md).

Hashes dos instaladores completos conferem integridade. Os pacotes incrementais usam também manifesto assinado pelo fornecedor; essa assinatura não equivale à assinatura de código do Windows.

## Política de publicação

Versões publicadas não são sobrescritas. Correções recebem novo número. Instaladores anteriores e seus manuais permanecem disponíveis para recuperação, sujeita à compatibilidade dos dados.
Este repositório não recebe código privado, credenciais, chaves, fotos, inspeções, backups de clientes ou modelos privados.
