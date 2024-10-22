To-Do List 📝
Este é um projeto simples de To-Do List desenvolvido em Django, onde você pode adicionar, listar, editar e excluir tarefas. O objetivo é demonstrar como construir um sistema básico de gerenciamento de tarefas utilizando o framework Django.

Funcionalidades:
🆕 Adicionar novas tarefas.
📋 Listar todas as tarefas.
✏️ Editar tarefas existentes.
❌ Excluir tarefas.
✅ Marcar tarefas como "concluídas" ou "pendentes".

Pré-requisitos:
Certifique-se de ter as seguintes ferramentas instaladas no seu ambiente de desenvolvimento:

Python 3.x
pip (gerenciador de pacotes Python)
virtualenv (opcional, mas recomendado)

Configuração do Projeto:
Siga as etapas abaixo para configurar o projeto localmente:

1. Clone o Repositório
Copiar código
git clone https://github.com/seu-usuario/todo-list-django.git
cd todo-list-django
2. Crie e Ative um Ambiente Virtual

No Windows:

Copiar código
python -m venv venv
venv\Scripts\activate

No macOS/Linux:

Copiar código
python3 -m venv venv
source venv/bin/activate

3. Instale as Dependências:
Instale o Django e outras dependências necessárias:

Copiar código
pip install -r requirements.txt

4. Execute as Migrações do Banco de Dados:
Crie as tabelas necessárias no banco de dados:

Copiar código
python manage.py migrate

5. Crie um Superusuário:
Para acessar a área administrativa do Django, crie um superusuário:

Copiar código
python manage.py createsuperuser

6. Execute o Servidor:
Inicie o servidor de desenvolvimento do Django:

Copiar código
python manage.py runserver
Abra seu navegador e acesse http://127.0.0.1:8000 para ver o sistema de To-Do List funcionando!

Estrutura do Projeto
todo_project/
│
├── todo_project/         # Configurações e URLs principais do projeto Django
│
├── tasks/                # App que contém a lógica do sistema de tarefas
│   ├── migrations/       # Migrações do banco de dados
│   ├── templates/        # Templates HTML para renderização
│   │   └── tasks/        # Arquivos HTML relacionados ao app de tarefas
│   ├── admin.py          # Registro do modelo Task na administração
│   ├── models.py         # Definição do modelo de dados Task
│   ├── views.py          # Lógica das views para tarefas (listagem, adição, edição, exclusão)
│   └── urls.py           # Definição das rotas do app tasks
│
├── db.sqlite3            # Banco de dados SQLite
├── manage.py             # Script de gerenciamento do Django
└── README.md             # Documentação do projeto

Principais Arquivos:
models.py: Define o modelo Task, que representa uma tarefa com um título, status (concluído ou pendente) e data de criação.
views.py: Contém as lógicas para listar, adicionar, editar e excluir tarefas.
templates/tasks/: Contém os templates HTML usados para renderizar as páginas.
urls.py: Define as URLs para acessar as funcionalidades do sistema.

Como Usar:
Acesse http://127.0.0.1:8000/ para ver a lista de tarefas.
Clique em "Adicionar nova tarefa" para criar uma nova tarefa.
Use os links Editar ou Excluir ao lado de cada tarefa para modificar ou removê-la.
Acesse http://127.0.0.1:8000/admin para gerenciar as tarefas através do painel administrativo do Django (é necessário login).

Personalização e Expansão:
Este projeto é um ponto de partida e pode ser facilmente expandido. Aqui estão algumas ideias de melhorias:

📅 Adicionar prazos para cada tarefa.
👥 Implementar autenticação para que diferentes usuários possam ter suas próprias listas.
📊 Implementar filtragem e ordenação de tarefas (por data de criação ou status).
📱 Melhorar o design e a responsividade do layout para dispositivos móveis.

Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

Contribuições
Sinta-se à vontade para abrir issues ou enviar pull requests para melhorias!

Contato
Se tiver dúvidas ou sugestões, entre em contato:

Email: carloscelestino.pydev@gmail.com
GitHub: https://github.com/carloscelestino1

Enjoy coding! 🚀