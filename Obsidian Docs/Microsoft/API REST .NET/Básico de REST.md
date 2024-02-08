
### Framework Swagger

Swagger é um framework para documentar APIs REST e mostrar as possíveis rotas disponíveis para serem usados pelos desenvolvedores.

![[Swagger.png]]
### usando JWT - Jason Web Token

JWT é um framework para autenticação onde ele deve receber informações de login e criar um token que deve ser utilizado durante o tempo que estiver ativo.

Os tokens tem um tempo curto de uso, que é o tempo que ele valida sua autenticação, depois é só Logar novamente.

![[JWT token.png]]
### Boas práticas no desenvolvimento de APIs REST

1. Paginação dos dados: se forem muitos dados de uma pesquisa é importante poder paginar o número de registros para auxiliar na busca
2. Filtros configurados: ter formas de filtrar os dados para encontrar mais rápido.
3. Separar corretamente os recursos lógicos: cada request deve ser de uma informação específica, não misturando tudo para uma unica coisa.
4. Tolerância a falhas: fazer com que a API consiga lidar corretamente com possíveis erros.
5. Cache de informações recorrentes: quando temos alguma info que precisamos buscar sempre, fazemos um sistema de cache que não precise sempre buscar o dado no banco de dados.
6. Conectividade com a API: achar formas que facilite o acesso as suas APIs de fora.
7. Definir Timeouts: para que não fique segurando o servidor permanentemente, dessa forma ele finaliza o processo caso não conclua em um tempo determinado.
8. Documentação da API: ache formas fáceis e práticas de documentar suas APIs para que qualquer um consiga utilizar ela.
9. Utilizar SSL: para melhor segurança ao seu projeto.
10. Versionamento de APIs: para caso algo dê de errado podemos avaliar a versão anterior.
11. Teste e Validação da API: para ver se a API está seguindo o fluxo corretamente.
12. Permitir exportações de infos em diferentes formatos (JSON, CSV, etc...)
13. Notificações: achar uma forma de notificar caso a API tenha tido um problema.
14. Monitore sua API: verificar como anda a utilização da API.