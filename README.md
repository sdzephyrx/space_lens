# Space Lens
Exercicio das aulas do curso de Django da Alura.
Projeto criado para manipulação de conceitos de Django em ambiente web
Front-end e CSS disponibilizado por Alura cursos.

- Arquivo requeriments.txt mostra as dependencias necessarias do ambiente 
virtual para execução do projeto.
Comando para rodar no ambiente virtual para instalação dos pacotes:
  - pip install -r requirements.txt
  - python scripts/secret_key_generator.py > .env
  - python manage.py migrate ( para importar o schema do banco )
  - python manage.py createsuperuser ( para criar o usuario admin do banco )

Caso ocorra de não carregar as imagens, rodar o seguinte comando:
  - python manage.py collectstatic (para import de assets)

Para o uso do S3 da amazon, é necessário uma conta, um bucket s3 e chaves de 
acesso válidas. Essas infos devem ser salvos no arquivo .env com as seguintes
variaveis:
  -AWS_ACCESS_KEY_ID 
  -AWS_SECRET_ACCESS_KEY
  -AWS_STORAGE_BUCKET_NAME
No arquivo setup/settings.py, é necessário a configuração das seguintes variaveis para o uso
do s3:
  -AWS_DEFAULT_ACL
  -AWS_S3_OBJECT_PARAMETERS
  -AWS_LOCATION
  -AWS_QUERYSTRING_AUTH
  -AWS_HEADERS

Apos o clone do projeto, use o seguinte comando para iniciar o servidor:
  - python manage.py runserver (para rodar o servidor)

