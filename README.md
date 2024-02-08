# StarSchema

Foi proposto o seguinte problema:

* O esquema possui a tabela Professor, Departamento, Curso, Disciplina e Aluno;
* A tabela Professor tem relacionamento 1:N com a tabela Departamento e a tabela Disciplina;
* A tabela Curso tem relação com N:M com Disciplina;
* A tabela Disciplina tem relação N:M com a tabela Pre_Requisito e a tabela Aluno.

Transforme este esquema tradicional para o StarSchema indicado para o Power BI.

Para transformar um ER (modelo de entidade-relacionamento) como o da foto em um modelo Star Schema para o Power BI, com a tabela fato sendo "Professor":

1. **Identifique as tabelas de dimensão**: No seu caso, as tabelas "Departamento", "Curso", "Disciplina" e "Aluno" podem ser consideradas como tabelas de dimensão.
2. **Defina a tabela fato**: A tabela “Professor” será a sua tabela fato. Inclua chaves estrangeiras referenciando as tabelas de dimensão.
3. **Estabeleça as relações**: Assegure-se que todas as relações entre a tabela fato e as tabelas de dimensão sejam do tipo um para muitos (1:M).
4. **Inclua medidas na tabela fato**: Estas podem ser contagens, somas ou outras agregações dos dados relacionados às entradas específicas na tabela “Professor”.
5. **Importe para o Power BI**: Importe este modelo para o Power BI e construa suas visualizações com base nas tabelas de dimensão e medidas na tabela fato.
