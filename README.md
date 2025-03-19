# Comandos Essenciais para Desenvolvedores Fullstack em 2025

## Git

| Comando | Uso |
|---------|-----|
| `git init` | Inicializa um repositório Git |
| `git clone [url]` | Clona um repositório remoto |
| `git add [arquivo]` | Adiciona arquivos para staged |
| `git add .` | Adiciona todos os arquivos modificados para staged |
| `git commit -m "mensagem"` | Cria um commit com mensagem |
| `git commit --amend` | Modifica o último commit |
| `git push` | Envia commits para o repositório remoto |
| `git pull` | Atualiza repositório local com mudanças remotas |
| `git fetch` | Busca atualizações sem mesclar |
| `git branch` | Lista todas as branches |
| `git branch [nome]` | Cria uma nova branch |
| `git checkout [branch]` | Muda para outra branch |
| `git switch [branch]` | Muda para outra branch (Git moderno) |
| `git checkout -b [nome]` | Cria e muda para nova branch |
| `git merge [branch]` | Integra uma branch à atual |
| `git rebase [branch]` | Reaplica commits em outro branch |
| `git status` | Mostra arquivos modificados |
| `git log` | Mostra histórico de commits |
| `git log --graph --oneline` | Visualiza histórico em formato gráfico |
| `git stash` | Armazena mudanças temporariamente |
| `git stash pop` | Recupera mudanças armazenadas |
| `git reset --hard HEAD` | Descarta todas as mudanças locais |
| `git restore [arquivo]` | Restaura arquivo para versão anterior |
| `git cherry-pick [hash]` | Aplica commit específico na branch atual |

## Docker

| Comando | Uso |
|---------|-----|
| `docker ps` | Lista contêineres em execução |
| `docker ps -a` | Lista todos os contêineres |
| `docker images` | Lista imagens disponíveis |
| `docker build -t [nome] .` | Constrói uma imagem a partir do Dockerfile |
| `docker run [nome]` | Executa um contêiner |
| `docker run -d -p [porta]:[porta] [nome]` | Executa contêiner em background mapeando portas |
| `docker stop [id/nome]` | Para um contêiner |
| `docker rm [id/nome]` | Remove um contêiner |
| `docker rmi [imagem]` | Remove uma imagem |
| `docker-compose up` | Inicia serviços definidos no docker-compose.yml |
| `docker-compose down` | Para serviços definidos no docker-compose.yml |
| `docker-compose up -d --build` | Reconstrói e inicia serviços em background |
| `docker exec -it [id/nome] bash` | Acessa terminal de um contêiner |
| `docker logs [id/nome]` | Exibe logs de um contêiner |
| `docker logs -f [id/nome]` | Acompanha logs em tempo real |
| `docker network ls` | Lista redes Docker |
| `docker volume ls` | Lista volumes Docker |
| `docker system prune` | Remove recursos não utilizados |
| `docker compose config` | Valida e exibe configuração de compose |

## SSH

| Comando | Uso |
|---------|-----|
| `ssh [usuario]@[host]` | Conecta-se a um host remoto |
| `ssh -i [chave.pem] [usuario]@[host]` | Conecta usando arquivo de chave privada |
| `ssh-keygen -t rsa -b 4096` | Gera par de chaves RSA de 4096 bits |
| `ssh-keygen -t ed25519` | Gera par de chaves Ed25519 (mais seguro) |
| `ssh-copy-id [usuario]@[host]` | Copia chave pública para o servidor |
| `scp [arquivo] [usuario]@[host]:[caminho]` | Copia arquivo para servidor remoto |
| `scp [usuario]@[host]:[arquivo] [caminho]` | Copia arquivo do servidor remoto |
| `rsync -avz [diretório] [usuario]@[host]:[caminho]` | Sincroniza diretórios |
| `ssh -p [porta] [usuario]@[host]` | Conecta especificando porta |
| `ssh -L [porta-local]:[host]:[porta-remota] [usuario]@[host]` | Cria túnel SSH |
| `sshfs [usuario]@[host]:[dir-remoto] [dir-local]` | Monta sistema de arquivos remoto |

## Linux (Servidor)

| Comando | Uso |
|---------|-----|
| `ls -la` | Lista arquivos com detalhes |
| `cd [diretório]` | Muda de diretório |
| `mkdir -p [caminho/diretório]` | Cria diretórios recursivamente |
| `rm [arquivo]` | Remove arquivo |
| `rm -rf [diretório]` | Remove diretório recursivamente |
| `chmod +x [arquivo]` | Torna arquivo executável |
| `chmod 755 [arquivo]` | Define permissões (rwx para dono, rx para outros) |
| `chown [usuario]:[grupo] [arquivo]` | Muda proprietário de arquivo |
| `ps aux` | Lista processos em execução |
| `ps aux | grep [termo]` | Busca processos específicos |
| `kill [pid]` | Encerra processo por ID |
| `killall [nome]` | Encerra processos por nome |
| `systemctl start/stop/restart/status [serviço]` | Gerencia serviços systemd |
| `journalctl -u [serviço]` | Visualiza logs de serviço |
| `journalctl -f` | Acompanha logs do sistema em tempo real |
| `apt update && apt upgrade` | Atualiza pacotes (Debian/Ubuntu) |
| `dnf update` | Atualiza pacotes (Fedora/RHEL) |
| `top` / `htop` / `btop` | Monitora uso de recursos |
| `df -h` | Mostra espaço em disco |
| `du -sh [diretório]` | Mostra tamanho de diretório |
| `ncdu` | Analisador de uso de disco interativo |
| `tail -f [arquivo]` | Acompanha atualizações de arquivo de log |
| `grep -r "[padrão]" [diretório]` | Busca texto recursivamente |
| `find [diretório] -name "[padrão]"` | Encontra arquivos por nome |
| `tar -czvf [arquivo.tar.gz] [diretório]` | Compacta diretório |
| `tar -xzvf [arquivo.tar.gz]` | Descompacta arquivo tar.gz |
| `wget [url]` | Baixa arquivo da web |
| `curl -O [url]` | Baixa arquivo mantendo nome original |
| `crontab -e` | Edita tarefas agendadas |
| `ln -s [arquivo-origem] [link]` | Cria link simbólico |
| `nohup [comando] &` | Executa comando imune a desconexões |
| `tmux` | Inicia sessão de terminal multiplexada |
| `ufw allow [porta/serviço]` | Permite tráfego pelo firewall |

## C#

| Comando | Uso |
|---------|-----|
| `dotnet new console` | Cria novo projeto de console |
| `dotnet new webapi` | Cria novo projeto de API Web |
| `dotnet new mvc` | Cria novo projeto MVC |
| `dotnet new classlib` | Cria nova biblioteca de classes |
| `dotnet new blazor` | Cria novo projeto Blazor |
| `dotnet new react` | Cria projeto ASP.NET Core com React |
| `dotnet new sln` | Cria nova solução |
| `dotnet sln add [projeto.csproj]` | Adiciona projeto à solução |
| `dotnet build` | Compila o projeto |
| `dotnet run` | Executa o projeto |
| `dotnet watch run` | Executa com recarga automática |
| `dotnet test` | Executa testes |
| `dotnet add package [nome]` | Adiciona pacote NuGet |
| `dotnet add reference [projeto.csproj]` | Adiciona referência a projeto |
| `dotnet ef migrations add [nome]` | Adiciona migração Entity Framework |
| `dotnet ef database update` | Aplica migrações ao banco de dados |
| `dotnet publish -c Release` | Publica aplicação para produção |
| `dotnet tool install -g [ferramenta]` | Instala ferramenta global |
| `dotnet format` | Formata código conforme convenções |

## Python

| Comando | Uso |
|---------|-----|
| `python -m venv [nome]` | Cria ambiente virtual |
| `source [nome]/bin/activate` | Ativa ambiente virtual (Linux/Mac) |
| `[nome]\Scripts\activate` | Ativa ambiente virtual (Windows) |
| `deactivate` | Desativa ambiente virtual |
| `pip install [pacote]` | Instala pacote |
| `pip install -r requirements.txt` | Instala dependências do requirements.txt |
| `pip freeze > requirements.txt` | Gera arquivo de dependências |
| `python [script.py]` | Executa script Python |
| `python -m pytest` | Executa testes com pytest |
| `python -m black [arquivo/diretório]` | Formata código com Black |
| `python -m flake8 [arquivo/diretório]` | Analisa código com Flake8 |
| `python -m mypy [arquivo/diretório]` | Verifica tipos com mypy |
| `django-admin startproject [nome]` | Cria novo projeto Django |
| `python manage.py runserver` | Inicia servidor Django |
| `python manage.py makemigrations` | Cria migrações Django |
| `python manage.py migrate` | Aplica migrações Django |
| `python manage.py createsuperuser` | Cria admin Django |
| `python -m flask run` | Inicia aplicação Flask |
| `python -m uvicorn app:app --reload` | Inicia FastAPI com recarga |
| `python -m pipx install [pacote]` | Instala app Python isoladamente |
| `poetry init` | Inicia projeto Poetry |
| `poetry add [pacote]` | Adiciona dependência com Poetry |

## PHP

| Comando | Uso |
|---------|-----|
| `php -v` | Mostra versão do PHP |
| `php -S localhost:8000` | Inicia servidor PHP embutido |
| `php [arquivo.php]` | Executa script PHP |
| `php -l [arquivo.php]` | Verifica sintaxe PHP |
| `composer init` | Inicia novo projeto Composer |
| `composer install` | Instala dependências |
| `composer require [pacote]` | Adiciona dependência |
| `composer update` | Atualiza dependências |
| `composer dump-autoload` | Regenera autoloader |
| `php artisan serve` | Inicia servidor Laravel |
| `php artisan make:model [Nome]` | Cria modelo Laravel |
| `php artisan make:controller [Nome]Controller` | Cria controlador Laravel |
| `php artisan make:migration [nome]` | Cria migração Laravel |
| `php artisan migrate` | Executa migrações Laravel |
| `php artisan tinker` | Inicia REPL Laravel |
| `php artisan route:list` | Lista rotas Laravel |
| `php artisan optimize` | Otimiza aplicação Laravel |
| `php artisan test` | Executa testes Laravel |
| `php artisan make:livewire [Nome]` | Cria componente Livewire |

## React

| Comando | Uso |
|---------|-----|
| `npx create-react-app [nome]` | Cria projeto React tradicional |
| `npx create-next-app [nome]` | Cria projeto Next.js |
| `npx create-vite [nome] --template react-ts` | Cria projeto React com Vite e TypeScript |
| `npm start` | Inicia servidor de desenvolvimento |
| `npm run build` | Compila aplicação para produção |
| `npm test` | Executa testes |
| `npm run lint` | Executa linter |
| `npm run eject` | Ejeta configurações do create-react-app |
| `npx storybook init` | Inicializa Storybook no projeto |
| `npm run storybook` | Inicia servidor Storybook |
| `npx react-codemod rename-unsafe-lifecycles` | Migra lifecycles legados |
| `npm run analyze` | Analisa bundle (requer configuração) |
| `npx react-native init [nome]` | Cria projeto React Native |
| `npx expo init [nome]` | Cria projeto Expo (React Native) |
| `npm i @reduxjs/toolkit react-redux` | Instala Redux Toolkit |
| `npm i react-query` | Instala React Query |
| `npm i styled-components` | Instala Styled Components |
| `npm i sass` | Adiciona suporte a SASS |
| `npm i tailwindcss postcss autoprefixer` | Instala Tailwind CSS |
| `npx tailwindcss init -p` | Inicializa Tailwind CSS no projeto |

## Node.js / JavaScript

| Comando | Uso |
|---------|-----|
| `node [arquivo.js]` | Executa script Node.js |
| `node --inspect [arquivo.js]` | Executa com depurador |
| `npm init` | Inicia projeto Node.js |
| `npm install [pacote]` | Instala pacote |
| `npm i -D [pacote]` | Instala como dependência de desenvolvimento |
| `npm update` | Atualiza pacotes |
| `npm run [script]` | Executa script do package.json |
| `npm audit fix` | Corrige vulnerabilidades |
| `npm outdated` | Mostra pacotes desatualizados |
| `npx [comando]` | Executa pacote sem instalar |
| `yarn create [template] [nome]` | Cria projeto com template |
| `yarn add [pacote]` | Instala pacote com Yarn |
| `pnpm i [pacote]` | Instala pacote com pnpm |
| `nvm install [versão]` | Instala versão do Node.js com NVM |
| `nvm use [versão]` | Muda versão ativa do Node.js |
| `eslint --init` | Configura ESLint |
| `prettier --write [arquivo/diretório]` | Formata código com Prettier |
| `tsc --init` | Inicializa configuração TypeScript |

## Banco de Dados

| Comando | Uso |
|---------|-----|
| `mysql -u [usuario] -p` | Conecta ao MySQL |
| `mysqldump -u [usuario] -p [banco] > backup.sql` | Exporta banco MySQL |
| `psql -U [usuario] -d [banco]` | Conecta ao PostgreSQL |
| `pg_dump -U [usuario] [banco] > backup.sql` | Exporta banco PostgreSQL |
| `mongosh` | Conecta ao MongoDB |
| `mongodump --db [banco] --out [dir]` | Faz backup MongoDB |
| `mongoexport --db [banco] --collection [coleção] --out [arquivo.json]` | Exporta coleção para JSON |
| `redis-cli` | Conecta ao Redis |
| `redis-cli --scan --pattern "*"` | Lista todas chaves Redis |
| `sqlcmd -S [servidor] -U [usuario] -P [senha]` | Conecta ao SQL Server |
| `sqlite3 [arquivo.db]` | Abre banco SQLite |
| `prisma init` | Inicializa Prisma ORM |
| `prisma migrate dev` | Cria e aplica migração Prisma |
| `prisma db push` | Sincroniza schema com banco |
| `prisma studio` | Interface visual para banco Prisma |

## Ferramentas de Build e Package Managers

| Comando | Uso |
|---------|-----|
| `npm ci` | Instala dependências exatas do lockfile |
| `npm run build` | Executa script de build |
| `yarn install --frozen-lockfile` | Instala dependências exatas |
| `pnpm install --frozen-lockfile` | Instala dependências exatas |
| `webpack` | Executa webpack conforme configuração |
| `webpack --config [arquivo]` | Usa configuração específica |
| `vite` | Inicia servidor de desenvolvimento Vite |
| `vite build` | Compila projeto Vite para produção |
| `gulp [tarefa]` | Executa tarefa do Gulp |
| `rollup -c` | Executa Rollup com configuração |
| `esbuild [entrada] --outfile=[saída]` | Compila com esbuild |
| `turbo run build` | Executa build com Turborepo |
| `lerna run [script]` | Executa script em múltiplos pacotes |

## Ferramentas de Rede e API

| Comando | Uso |
|---------|-----|
| `ping [host]` | Testa conectividade |
| `curl [url]` | Faz requisição HTTP |
| `curl -X POST -H "Content-Type: application/json" -d '{"key":"value"}' [url]` | POST com JSON |
| `wget [url]` | Baixa recurso da web |
| `netstat -tulpn` | Lista portas em uso |
| `nslookup [domínio]` | Consulta DNS |
| `dig [domínio]` | Consulta DNS detalhada |
| `traceroute [host]` | Traça rota até o host |
| `tcpdump -i [interface]` | Captura tráfego de rede |
| `ss -tuln` | Lista portas em escuta |
| `nmap [host/rede]` | Escaneia portas e serviços |
| `openssl s_client -connect [host]:[porta]` | Testa conexão TLS |
| `httpie post [url] key=value` | Requisição POST com httpie |
| `ngrok http [porta]` | Expõe porta local na internet |

## Ferramentas de CI/CD e DevOps

| Comando | Uso |
|---------|-----|
| `aws s3 cp [local] s3://[bucket]/` | Copia para S3 (AWS CLI) |
| `aws ec2 describe-instances` | Lista instâncias EC2 |
| `aws lambda invoke --function-name [nome] output.json` | Invoca função Lambda |
| `az login` | Autentica no Azure CLI |
| `az webapp up --name [nome]` | Implanta app web Azure |
| `gcloud init` | Configura Google Cloud CLI |
| `gcloud app deploy` | Implanta app no App Engine |
| `heroku login` | Login no Heroku CLI |
| `heroku create` | Cria app Heroku |
| `heroku git:remote -a [app]` | Configura remote para app |
| `heroku logs --tail` | Acompanha logs Heroku |
| `firebase deploy` | Deploy para Firebase |
| `vercel` | Deploy para Vercel |
| `netlify deploy` | Deploy para Netlify |
| `terraform init` | Inicializa diretório Terraform |
| `terraform plan` | Mostra plano de execução |
| `terraform apply` | Aplica mudanças de infraestrutura |
| `kubectl get pods` | Lista pods Kubernetes |
| `kubectl apply -f [arquivo.yaml]` | Aplica configuração Kubernetes |
| `helm install [release] [chart]` | Instala chart Helm |
| `gh repo clone [repo]` | Clona repositório usando GitHub CLI |
| `gh pr create` | Cria Pull Request |

## Ferramentas para Testes e Qualidade

| Comando | Uso |
|---------|-----|
| `jest` | Executa testes Jest |
| `jest --coverage` | Executa testes com relatório de cobertura |
| `cypress open` | Abre interface Cypress |
| `cypress run` | Executa testes Cypress headless |
| `playwright test` | Executa testes Playwright |
| `vitest` | Executa testes Vitest |
| `npm run test:e2e` | Executa testes end-to-end |
| `npm run test:unit` | Executa testes unitários |
| `lighthouse [url]` | Audita desempenho de página |
| `sonar-scanner` | Executa análise SonarQube |
| `k6 run [script.js]` | Executa teste de carga |
