---
layout: post
title: "Home Lab Base: Criando um ambiente de redes com Proxmox 🖥️"
date: 2026-09-17
tags: [HomeLab, Proxmox, Redes, Virtualizacao, Dicas]
---

No dia a dia das operações de rede, testar configurações de roteamento, firewalls ou novas topologias direto em produção é um risco que não podemos correr. Todo analista precisa de um ambiente de laboratório isolado e confiável.

Para montar o meu Home Lab, a escolha foi o **Proxmox VE**. Por ser um hypervisor *bare-metal* (instalado direto no hardware, sem precisar de um Windows por baixo), ele entrega muito mais performance e permite o gerenciamento de tudo via interface Web.

O objetivo aqui não é reinventar a roda com um tutorial longo, mas te dar o "caminho das pedras" rápido de como a estrutura funciona.

## O Passo a Passo (Visão Geral)

Se você vai subir o seu próprio servidor, o fluxo prático se resume a estas 4 etapas:

1. **A Base:** Fazer o download da ISO oficial no site do Proxmox e criar um pendrive bootável (ferramentas como o Rufus ou BalenaEtcher resolvem isso em minutos).
2. **Instalação:** Dar o boot na máquina que será o servidor e seguir o assistente. O ponto de atenção aqui é a **configuração da interface de rede**: você precisará definir um IP Estático (Gateway e DNS) que fará parte da sua rede local para não perder o acesso ao servidor depois.
3. **Acesso Web:** Com a instalação finalizada, o servidor pode ficar "sem monitor". Todo o acesso passa a ser feito pelo navegador através do endereço `https://<IP-DO-SERVIDOR>:8006`.
4. **Alimentando o Lab:** Dentro do painel Web, basta fazer o upload das ISOs (Windows, Linux, ou ferramentas como EVE-NG e GNS3) no armazenamento local (local storage) e começar a criar suas Máquinas Virtuais.

## Mão na massa: Tutoriais Recomendados

Como a comunidade já tem materiais incríveis e visuais sobre isso, separei aqui as melhores referências em vídeo para você acompanhar a instalação clique a clique sem dor de cabeça:

* **[Guia de Instalação do Proxmox (YouTube) - Substitua pelo link do seu vídeo favorito]**
* **[Como fazer o upload de ISOs e criar a primeira VM no Proxmox - Substitua pelo link]**

Montar essa base é o primeiro passo. Com o Proxmox rodando, o céu é o limite para simularmos nossos laboratórios de CCNA, firewalls e serviços de rede!

---
*Dica rápida de Infra: Sempre conecte seu servidor Proxmox no cabo de rede (Gigabit, se possível). Virtualização e rede de gerência via Wi-Fi não combinam!*
