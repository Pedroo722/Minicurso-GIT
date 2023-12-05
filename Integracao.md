Uma URL remota é outra forma de o Git dizer "o lugar onde seu código é armazenado". A URL poderia ser seu repositório no GitHub, ou a bifurcação de outro usuário, ou até mesmo em um servidor totalmente diferente.

Você pode fazer push apenas de dois tipos de endereço URL:

Uma URL HTTPS como https://github.com/user/repo.git
Uma URL SSH como git@github.com:user/repo.git
O Git associa uma URL remota a um nome, e o repositório remoto padrão geralmente é chamado origin.

Use o comando git remote add para corresponder uma URL remota com um nome. Por exemplo, você digitaria o seguinte na linha de comando:

git remote add origin <REMOTE_URL>
Isso associa o nome origin à REMOTE_URL.

Use o comando git remote set-url para alterar a URL de um repositório remoto.

Escolher uma URL para o seu repositório remoto
Existem várias maneiras de clonar repositórios disponíveis no GitHub.com.

Quando você visualiza um repositório conectado à sua conta, as URLs que podem ser usadas para clonar o projeto no computador ficam disponíveis abaixo dos detalhes do repositório.

Para obter informações sobre como definir ou alterar a URL remota, confira "Gerenciar repositórios remote".

Clonando com as URLs de HTTPS
As URLs de clone https:// estão disponíveis em todos os repositórios, independentemente da visibilidade. As URLs de clone https:// funcionam mesmo que você esteja protegido por um firewall ou um proxy.

Quando você usar git clone, git fetch, git pull ou git push em um repositório remoto usando URLs HTTPS na linha de comando, o Git solicitará seu nome de usuário e sua senha do GitHub. Quando o Git solicitar sua senha, insira seu personal access token. Como alternativa, você pode usar um auxiliar de credencial como o Gerenciador de Credenciais do Git. A autenticação baseada em senha do Git foi removida para dar lugar a métodos de autenticação mais seguros. Para obter mais informações, veja "Gerenciar seus tokens de acesso pessoal".

Dicas:

Você pode usar um auxiliar de credenciais para que o Git se lembre de suas credenciais de GitHub toda vez que falar com GitHub. Para obter mais informações, confira "Armazenar suas credenciais do GitHub no Git".
Para clonar um repositório sem se autenticar no GitHub na linha de comando, use o GitHub Desktop para a clonagem. Para obter mais informações, confira "Clonar um repositório do GitHub para o GitHub Desktop".