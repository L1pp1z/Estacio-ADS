Estudo do 3Semestre - Python (Utilizando Uv e Ruff)
UV é um gerenciador de pacotes do python, muito fácil de utilizar e mais rápido que o pip.
RUFF é pacote que ajuda a formatar o código seguindo regras de formatação profissional. Ele mostra como podemos escrever o código melhor e também possui função de ajustar o código automaticamente.

Para instalar o UV no sistema basta seguir o tutorial do vídeo:

https://www.youtube.com/watch?v=wD1Trf45ScI - Créditos ao Davi Lucciola

Exclui o .venv do Github, então ao clonar essa pasta basta apenas ter o uv instalado em sua maquina, baixar a versão que prefere do python, por aqui, utilizo a 3.12.13.

Para instalar essa versão utilize o comando no powershell:
uv python install 3.12.13 

Abra a pasta 3Semestre do vscode e dentro do terminal rode:
uv sync

Ele vai instalar as dependencias, criar seu próprio .venv, instalar o RUFF.
Para rodar o código, caso voce não mude a estrutura de pastas, utilize o seguinte comando:
uv run python -m pasta.nomedoarquivo

"pasta" -> Nome da pasta que esta dentro de src
"nomedoarquivo" -> Nome do arquivo que esta dentro dessa pasta, o .py precisa estar no nome do arquivo, mas não na linha de comando

Caso queira mexer na estrutura do projeto, lembre-se de mudar a pasta padrão, nesse caso 'src', no arquivo pyproject.toml.