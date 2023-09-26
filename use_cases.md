# Casos de uso para um gerenciador de matrículas em esportes

[Diagrama de casos de uso](https://lucid.app/lucidchart/675aef64-241e-4358-8ae2-89fec9fb228c/edit?viewport_loc=-37%2C-179%2C2613%2C1085%2C0_0&invitationId=inv_57e94931-0139-45d1-bef1-f46771f2f8a6)

## Ator: aluno

### Realizar cadastro
**Fluxo normal:**
1. Informar nome completo
2. Informar CPF
3. Informar e-mail
4. Informar data de nascimento
5. Informar senha
6. Informar matrícula da UFRN
7. Sistema vefirica se as informações são condizentes
8. O usuário possui acesso às turmas cadastradas no sistema, às turmas que ele está matriculado, aos participantes da turma em que está matriculado e às duas faltas

**Extensão:**
* 2a - Se o CPF for inválido, pedir novo CPF
* 3a - Se o e-mail for inválido, pedir novo e-mail
* 5a - Se a senha for inválida, pedir nova senha
* 6a - Se a matrícula for inválida, pedir nova matrícula
* 7a - Se as informações não existir na base de dados, retorna erro
* 7b - Se as informações não forem referentes a uma mesma pessoa, retorna erro

### Matricular em esporte
**Fluxo normal:**
1. [Sistema verifica se o aluno está autenticado](#)
2. Aluno acessa o informativo com as turmas disponíveis
3. Aluno solicita a matrícula em uma turma com vagas
4. Sistema verifica o atestado de aptidão física

**Extensão:**
* 1a - Se não estiver autenticado, pedir autenticação
* 4a - Se não houver atestado cadastro, pedir para cadastrar
* 4b - Se fizer mais de um ano que atestado foi cadastrado, pedir para cadastrar novamente





