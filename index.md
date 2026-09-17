\---

layout: default

\---



\# Bem-vindo ao meu Blog de Infraestrutura



Aqui compartilho meus resumos do SENAI, estudos sobre redes Wireless, CCNA e laboratórios de virtualização (Proxmox, VMware e Packet Tracer).



\## Últimos Artigos



<ul>

&#x20; {% for post in site.posts %}

&#x20;   <li>

&#x20;     <a href="{{ post.url }}">{{ post.title }}</a>

&#x20;     <span> - {{ post.date | date: "%d/%m/%Y" }}</span>

&#x20;   </li>

&#x20; {% endfor %}

</ul>

