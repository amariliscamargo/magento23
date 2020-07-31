# magento2 - teste 

## testando o magento 23

#### Para o sistema começar a funcionar, acesse por linha de comando a pasta principal onde se encontra o docker-compose.yml

Depois rodar o comando para o Elasticsearch funcionar:

sudo sysctl -w vm.max_map_count=262144

em seguida:

docker-compose up 

Aguarde, apos o docker dar o start vá no seu browser preferido e digite localhost para ver o sistema funcionando.

#### Para parar o magento:

docker-compose down


### Acesso ao admin 

* caminho para a area do administrador: http://127.0.0.1/index.php/admin

- Admin user: user
- password: password1234

### Versão do magento utilizada :   2.3.5

Repositorio da imagem utilizada:

https://devhub.io/repos/bitnami-bitnami-docker-magento


# Para o magento atualizar os modulos rodar os comando seguintes, dentro do container:

# upgrade magento install to include custom module
php /opt/bitnami/magento/htdocs/bin/magento setup:upgrade

# fix permissions
chown -R bitnami:daemon /opt/bitnami/magento/htdocs

# Na pasta app\design\amarilis esta o tema child que foi utilizado para "brincar" no sistema, após o usuario se logar ele vera a mensagem:
Oi! Eu sou um bloco estático exibido apenas para clientes cadastrados!

