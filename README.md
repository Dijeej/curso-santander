# curso-santander
Este repositório é voltado para as atividades da bolsa de estudos do Becas Santander.

## Git e Versionamento
### Criando repositórios
  * `git clone 'link do repositório'` clonagem de repositório.
  * `git init` dentro de uma pasta para torna-la um repositório.
### Salvando mudanças
  * `git status` para mostrar estado da branch, se há mudanças na origem e/ou no local.
  * `git add 'nome do arquivo'` para preparar um arquivo modificado para atualizar a branch.
  * `git diff 'nome do arquivo'` para verificar mudanças do arquivo original e modificado. `--staged` caso tenha recebido `git add`.
  * `git commit` para gerar um instantaneo das alterações preparadas e comentários dessa modificação.
  * `git log` para ver todas as alterações realizadas na branch.
  * `git restore` para remover alterações `--staged` para remover da área de preparação.
  * `git push 'nome da branch'` para adicionar as alterações confirmadas pelo `git commit`.
  * `git pull` para pegar os dados do repositório remoto e mesclar com o local.
