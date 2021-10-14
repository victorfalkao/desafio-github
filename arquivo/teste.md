# COMANDOS BÁSICOS GITHUB
- Criar nova chave

ssh-keygen -t ed25519 -C "your_email@example.com"

- Iniciar o agente 

eval "$(ssh-agent -s)"

- Navegue até a pasta onde está armazenada a chave e execute o comando

ssh-add -K ~/.ssh/id_ed25519

- Copiar a chave pública para colar no github 

cat id_ed25519.pub

- Configurar o GIT

git config --global user.email "your-email"
git config --global user.name "your-email"

- Mandar arquivo para stage

git add nome_do_arquivo
git add * (para adicionar todos)

- COMMIT

git commit -m "uma mensagem"

- Mostrar caminho do repositório remoto

git remote add origin caminho_do_repositório

- Enviar arquivos para o github

git push origin master

- Baixar arquivos do github

git pull origin master
