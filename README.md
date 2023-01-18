# Sistema-Resilia
* Contexto

A Resilia está pensando em lançar um novo sistema de
acompanhamento e para isso precisa de ajuda para modelar um
banco de dados que vai armazenar seus cursos, turmas e alunos.

## Para apoiar nesse sistema recebemos a tarefa de realizar essa modelagem e responder algumas perguntas com nosso modelo:
> Existem outras entidades além dessas três?
* Sim, além das 3 entidades sugeridas, achei interessante incluir professor, disciplinas e histórico.


> Quais são os principais campos e tipos?
* Os principais são as IDs e matrículas, estes estão indicados no print com uma pequena chave ao lado porque são as chaves primárias. O tipo de dado utilizado nesses campos é o int.

> Como essas entidades estão relacionadas?
* Cursos e Turmas(N:1) porque um curso pode ter muitas turmas mas uma turma tem apenas um curso;

* Cursos e disciplinas(N:N) já que um curso pode ter diversas disciplinas e as disciplinas podem fazer parte de inúmeros cursos;

* Disciplina e professor(N:N) porque um professor pode ter a especialização e lecionar em mais de uma disciplina e uma disciplina pode ter mais de um professor;

* Professor e turma(N:N) porque um professor dá aula em mais de uma turma e uma turma pode ter mais de um professor;

* Turma e alunos(N:N) um aluno pode estar matriculado em mais de uma turma e uma turma tem mais de um aluno e

* Alunos e histórico(1:1) já que um aluno tem apenas um histórico e cada histórico pertence a um único aluno(Individual).



# Print para visualização do que foi dito:

![image](https://user-images.githubusercontent.com/89803121/213309480-be3a7e97-ce2a-4599-a124-b8d44d0c8b8c.png)

