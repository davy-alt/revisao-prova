GET /instrutores [x] - Retorna todos os usuários do tipo "instrutor".

GET /cursos/com-muitos-comentarios?min=3 [x] - Retorna cursos com mais de 3 comentários.

GET /usuarios/:id/cursos [x] - Retorna os cursos em que o usuário com :id está matriculado.

GET /usuarios/com-progresso-acima?min=80 [x] - Lista usuários com progresso acima de 80% em qualquer curso.

GET /usuarios/:id/comentarios [x] - Retorna todos os comentários feitos por um usuário específico.

📊 Cálculos e Estatísticas
GET /cursos/:id/media-progresso [x] - Calcula a média de progresso dos alunos no curso.

GET /cursos/:id/media-nota [x] - Retorna a média de notas dos comentários do curso.

GET /cursos/:id/duracao-total [x] - Retorna a duração total das aulas do curso.

GET /instrutores/:id/quantidade-cursos [x] - Retorna o número de cursos criados pelo instrutor.

GET /certificados/por-curso [x] - Retorna a quantidade de certificados emitidos por curso.

🧩 Transformações e Agrupamentos
GET /usuarios/agrupados-por-tipo [x] - Agrupa usuários por tipo (estudante/instrutor) e conta quantos há de cada tipo.

GET /cursos/ordenados-por-nota [x] - Lista cursos ordenados pela média de notas dos comentários.

GET /usuarios/com-multiplos-certificados [X] - Lista alunos com mais de um certificado.

GET /cursos/:id/alunos-progresso-alto?min=90 [X] - Lista os alunos do curso com progresso acima de 90%.

GET /usuarios/:id/status-cursos [X] - Transforma progresso em status (completo, em andamento, não iniciado).

🛠️ Simulações e Atualizações
PATCH /usuarios/:id/progresso/:cursoId [] - Simula avanço de 10% no progresso de um curso.

POST /cursos [] - Cria um novo curso com aulas e vincula a um instrutor.

POST /cursos/:id/comentarios [] - Adiciona um comentário a um curso.

POST /certificados [] - Gera certificado para alunos com progresso ≥ 90%.

DELETE /cursos/sem-comentarios [] - Remove cursos que não têm comentários.