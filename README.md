# Aprendendo usar o Docker

#### Passo a passo seguindo o tutorial no site da DigitalOcean

Segue o link: https://www.digitalocean.com/community/tutorials/how-to-build-a-node-js-application-with-docker-on-ubuntu-20-04

#### Eu utilizo o Ubuntu 18.04 como OS

    Foi criado um server com express e arquivos statics em HTML.

    Foi criado uma imagem docker, um container docker com nodejs e fiz um push para o dockerHub

#### Eu segui todo o passo o passo sobre Docker do site, que foram esses a seguir.

_Para conseguir usar todos os passos abaixo é preciso ter o docker instalado em sua maquina. para isso só ir na documentação_

---

Documentação para instalação do docker com passo a passo para cada OS :
https://docs.docker.com/engine/install/

---

Criar um arquivo **Dockerfile** e sua configuração

Criar um arquivo **.dockerignore** para ignorar pastas e não serem utilizadas/duplicadas. Como a pasta node_modules que já é recriada pelos cmd no Dockerfile.

Construir uma imagem com o Dockerfile rodando no terminal **docker build .** (com o ponto no final)

---

    docker build .

 <li>Docker vai construir uma imagem buscando do directory indicado com o (.) 
e vai iniciar um container com a imagem criada no passo anterior rodando o cmd</li>

---

**_docker run --name "dar um nome ao container(sem as aspas duplas)
" -p " qual porta? Primeira porta é no seu host e a segunda é no container docker ex: 80:8080
" -d " -d para cotinuar executando mesmo se fechar o terminal"
E por ultimo qual sua imagem_**

#### Exemplo completo para o ultimo comando

    docker run --name nodejs-image -p 80:8080 -d nomedocontainer

### Outros comandos docker

---

    Rodar docker ps para listar os container ativos

---

    Rodar docker ps -a para listar todos os container existentes

---

    Rodar docker stop nomedocontainer _ para parar um container

---

    Rodar docker push para enviar uma imagem para seu DockerHub

    Rodar docker pull + nomedocontainer para baixar uma imagem do dockerhub

---

#### Esse foi meu passo a passo em busca de aprender como utilizar o docker

<p>Caso tenha algum erro de informção, pode fazer um pull request para me corrigir. Ficarei grato pela correção e atenção</p>

Meus contatos:
[![Linkedin Badge](https://img.shields.io/badge/-Henrique_Marques-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/hmarques98/)](https://www.linkedin.com/in/hmarques98/)
[![GitHub Badge](https://img.shields.io/badge/-Henrique_Marques-black?style=flat-square&logo=GitHub&logoColor=white&link=https://www.linkedin.com/in/hmarques98/)](https://github.com/hmarques98)
[![Outlook Badge](https://img.shields.io/badge/-Meu_Email-0AA6F0?style=flat-square&logo=GMail&logoColor=black&link=mailto:marquesprogrammer@hotmail.com)](mailto:marquesprogrammer@hotmail.com)
