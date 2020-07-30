# magento2 - teste 

## testando o magento 23

Para o sistema começar a funcionar, acesse por linha de comando a pasta principal onde se encontra o docker-compose.yml
Depois rodar o comando para o Elasticsearch funcionar:

sudo sysctl -w vm.max_map_count=262144

em seguida:

docker-compose up 

No browser digite localhost para ver o sistema funcionando.

Para parar o magento:

docker-compose down


### Acesso ao admin 

* caminho para a area do administrador: http://127.0.0.1/index.php/admin

- Admin user: user
- password: bitnami1

### Versão do magento utilizada :   2.3.5

Repositorio da imagem utilizada:

https://devhub.io/repos/bitnami-bitnami-docker-magento
