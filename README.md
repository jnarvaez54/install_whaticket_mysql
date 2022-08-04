## Versão Ubuntu 
### Passo a passo
Ao executar o comando abaixo, vai aparecer um menu para instalar ou atualizar.
Para instalar digite 1 e enter
Vai solicitar os seguintes dados
1. Senha mysql
2. Nome da empresa (em minúsculo), esse nome é para diferenciar as instalações, tanto do Whaticket, como dos recursos isolados via Docker.
3. Número máximo de conexões WhatsApp que essa instalação poderá usar
4. Número máximo de atendentes para essa instalação
5. Domínio do frontend, geralmente app.seusite.com.br
6. Domínio do backend, geralmente api.seusite.com.br
7. Porta do frontend, geralmente para a primeira instalação 3000, e a seguintes instalações que tiverem, 3001, 3002...
8. Porta do backend, geralmente para a primeira instalação 4000, e a seguintes instalações que tiverem, 4001, 4002...
9. Porta do redis, geralmente para a primeira instalação 5000, e a seguintes instalações que tiverem, 5001, 5002...
10. Porta do phpmyadmin, geralmente para a primeira instalação 6000, e a seguintes instalações que tiverem, 6001, 6002...
O acesso ao phpmyadmin é feito por IP do servidor, ex. http://111.111.111.111:6000
11. Porta do MYSQL, geralmente para a primeira instalação 7000, e a seguintes instalações que tiverem, 7001, 7002...

Seguindo todos os passos acima e não deixando faltar nenhuma da informações solicitadas, é só aguardar o instalador terminar a instalação.

Ao terminar a instalação é só logar com os dados padrão, caso não saiba veja na página do projeto [Whaticket aqui](https://github.com/owenbrasil/).

## INSTALAÇÃO 
FAZENDO DOWNLOAD DO INSTALADOR & INICIANDO A PRIMEIRA INSTALAÇÃO (USAR SOMENTE PARA PRIMEIRA INSTALAÇÃO):

```bash
sudo apt install -y git && git clone https://github.com/owenbrasil/install_mysql.git instalador && sudo chmod -R 777 ./instalador && cd ./instalador && sudo ./install_primaria
```

ACESSANDO DIRETORIO DO INSTALADOR & INICIANDO INSTALAÇÕES ADICIONAIS (USAR ESTE COMANDO PARA SEGUNDA OU MAIS INSTALAÇÃO:
```bash
cd && rm -rf instalador && git clone https://github.com/owenbrasil/install_mysql.git ./instalador && sudo chmod -R 777 ./instalador && cd ./instalador && sudo ./install_instancia
```
## Recursos 
- Multi instalador ilimitado [Whaticket](https://github.com/owenbrasil/install_mysql)
- Recursos isolados para cada instalação
- Instala Docker Mariadb (isolados)
- Instala Docker Redis (isolados)
- Instala Docker Phpmyadmin (isolados)
- instala nginx
- Configura os domínios com certificados de segurança
- Atualiza press ticket para última versão.

## Versão Debian
- [Whaticket-Installer](https://github.com/owenbrasil/)

## Instalação manual
- [Whaticket](https://github.com/owenbrasil/)
