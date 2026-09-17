---
layout: post
title: "LAN, MAN, WAN e Topologias: O mapa da infraestrutura 🗺️"
date: 2026-09-18
tags: [Fundamentos, Redes, CCNA, LAN, WAN, Topologias]
---

Antes de sair configurando roteadores, é crucial entender o mapa do terreno. Nas operações de rede, a forma como os equipamentos estão distribuídos fisicamente e logicamente dita como faremos o *troubleshooting* quando algo parar.

O escopo das redes se divide basicamente pela sua **abrangência**:

*   **LAN (Local Area Network):** A rede interna. Pode ser o laboratório, o escritório ou um galpão. É onde gerenciamos switches, Wi-Fi e VLANs com alta velocidade.
*   **MAN (Metropolitan Area Network):** Redes que conectam filiais dentro da mesma cidade (ou a rede do seu provedor de internet local).
*   **WAN (Wide Area Network):** A conexão de longa distância. É onde entram os links dedicados, roteamento BGP, MPLS e SD-WAN conectando a empresa ao mundo.

### A Topologia que domina o mercado

Embora a gente estude topologias em Anel ou Barramento, a realidade corporativa hoje é a **Topologia Estrela** (e Estrela Estendida). Tudo converge para um switch central (Core). Se um cabo quebrar, apenas aquele equipamento perde conexão. Já em redes Wireless modernas, a topologia **Mesh** (Malha) vem ganhando força para garantir redundância.

**Para aprofundar:**
*   [Recomendação de Vídeo: Entendendo LAN, WAN e Topologias na prática - Cole o Link aqui]
