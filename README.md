# desafio-k8s-ingress
4 Aplicações HTML com NGINX Ingress

Este projeto foi desenvolvido como parte de um desafio prático de Kubernetes, com o objetivo de demonstrar como criar e publicar quatro aplicações web simples utilizando containers Docker e orquestração com Minikube. 

Cada aplicação consiste em uma página HTML diferente, servida por um container NGINX personalizado. Para facilitar o acesso externo, foi configurado o NGINX Ingress Controller, permitindo que cada aplicação seja acessada por um caminho específico na URL do cluster. 

Durante o desenvolvimento, foram criados arquivos Dockerfile para cada aplicação, responsáveis por construir as imagens Docker contendo o servidor NGINX e a respectiva página HTML. Em seguida, foram definidos os manifestos Kubernetes necessários para realizar o deploy dos containers (Deployments) e expor cada aplicação dentro do cluster (Services). 

Por fim, foi criado um recurso Ingress que direciona as requisições recebidas para o serviço correspondente, de acordo com o caminho informado na URL. O resultado é um ambiente Kubernetes funcional no Minikube, onde é possível acessar cada uma das quatro aplicações web através de diferentes rotas, demonstrando na prática conceitos fundamentais de containers, deploys automatizados e roteamento de tráfego com Ingress. 
