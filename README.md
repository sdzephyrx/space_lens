# alura_space
Exercicio das aulas do curso de Django da Alura.
Projeto criado para manipulação de conceitos de Django em ambiente web
Front-end disponibilizado por Alura cursos.

- Arquivo requeriments.txt mostra as dependencias necessarias do ambiente 
virtual para execução do projeto.
Comando para rodar no ambiente virtual para instalação dos pacotes:
  - pip install -r requirements.txt
  - echo "SECRET_KEY=`python generate_secret_key.py`" > .env
  - python manage.py migrate ( para importar o schema do banco )
  - python manage.py createsuperuser ( para criar o usuario admin do banco )

Apos o clone do projeto, use o seguinte comando para iniciar o servidor:
  - python manage.py runserver (para rodar o servidor)

Caso ocorra de não carregar as imagens, rodar o seguinte comando:
  - python manage.py collectstatic (para import de assets)