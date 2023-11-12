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
  * `git fetch` para verificar as modificações antes de adiciona-las no repositório local.
### Branches
  * `git branch 'nome da branch'` para criar uma nova branch.
  * `git log --oneline --decorate` para verificar em qual branch estamos.
  * `git checkout 'nome da branch'` para mudar a branch trabalhada.
  * `git merge 'nome da branch'` para mesclar alterações de outra branch, git merge deve ser feito na branch que será atualizada.

## Algorítimos
### Exercício Completo (Pseudocódigo)
```
INICIO principal
  VAR opcao_selecionada: STRING
  VAR valor: INTEIRO
  VAR saldo: INTEIRO
  VAR encerrar_programa: BOOLEANO

  DEFINIR encerrar_programa -> Falso

  ENQUANTO encerrar_programa IGUAL_a Falso
    CHAMAR MOSTRAR_MENU -> opcao_selecionada
    SE opcao_selecionada IGUAL_A a
      MOSTRAR "Seu saldo é: ", saldo
    OU_SE opcao_selecionada IGUAL_A b
      MOSTRAR "Digite o valor a depositar: "
      ESPERAR_DIGITACAO -> valor
      SOMAR valor, saldo -> saldo
      MOSTRAR "Deposito efetuado"
    OU_SE opcao_selecionada IGUAL_A c
      MOSTRAR "Digite valor a retirar: "
      ESPERAR_DIGITACAO -> valor
      SE valor MAIOR_QUE saldo
        MOSTRAR "Saque não permitido, saldo insuficiente"
      SENAO
        SUBTRAIR valor, saldo -> saldo
      FIM SE
      MOSTRAR "Saque efetuado"
    OU_SE opcao_selecionada IGUAL_A d
      DEFINIR Verdadeiro -> encerrar_programa
    SENAO
      MOSTRAR "Opcao inválida, tente novamente"
    FIM SE
  FIM ENQUANTO
FINAL

INICIO MOSTRAR_MENU
  VAR opcao_selecionada: STRING
  MOSTRAR "Menu de operacao"
  MOSTRAR "[a] Mostrar Saldo"
  MOSTRAR "[b] Efetuar Depósito"
  MOSTRAR "[c] Efetuar Saque"
  MOSTRAR "[d] Finalizar"
  ESPERAR_DIGITACAO -> opcao selecionada
  RETORNAR opcao_selecionada
FIM MOSTRAR_MENU
```