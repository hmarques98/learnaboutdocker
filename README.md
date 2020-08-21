# Aprendendo usar o Docker

## Passo a passo

### Seguindo o tutorial no site da DigitalOcean

    -- https://www.digitalocean.com/community/tutorials/how-to-build-a-node-js-application-with-docker-on-ubuntu-20-04


    -- Foi criado um server com express e arquivos statics em HTML.

    -- EU segui todo o passo o passo sobre Docker do site que foram eles.

        -- Criar um arquivo Dockerfile e sua configuração

        -- Criar um arquivo .dockerignore para ignorar pastas e não serem utilizadas/duplicadas. 
        Como a pasta node_modules que já é recriada pelos cmd no Dockerfile.

        -- Construir uma imagem com o Dockerfile rodando no terminal *docker build .*
            -- docker vai construir uma imagem buscando do directory indicado com o .

       Iniciar um container com a imagem criada no passo anterior rodando o cmd docker run --name "dar um nome ao container(sem as aspas duplas)" -p 
        "qual porta? 
        Primeira porta é no seu host e a segunda é no container docker" 80:8080 -d "-d para cotinuar executando mesmo se fechar o terminal" 
        e por ultimo qual sua imagem

            -- exemplo completo para o ultimo comando
                -- docker run --name nodejs-image -p 80:8080 -d nomedocontainer
        -- Rodar docker ps para listar os container ativos

        -- Rodar docker ps -a para listar todos os container existentes

        -- Rodar * docker stop nomedocontainer * para parar um container

        -- Rodar docker push para enviar uma imagem para seu DockerHub

        -- Rodar docker pull + nomedocontainer para baixar uma imagem do dockerhub

## Esse foi meu passo a passo em busca de aprender como utilizar o docker

    -- Caso tenha algum erro de informção, pode fazer um pull request para me corrigir. Ficarei grato pela correção e atenção

### Eu utilizo o Ubuntu 18.04 como OS
