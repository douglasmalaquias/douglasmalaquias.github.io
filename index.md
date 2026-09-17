---
layout: default
---

# Bem-vindo ao meu Blog de Infraestrutura

Aqui compartilho meus resumos do SENAI, estudos sobre redes Wireless, CCNA e laboratórios de virtualização (Proxmox, VMware e Packet Tracer).

## Últimos Artigos

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span> - {{ post.date | date: "%d/%m/%Y" }}</span>
    </li>
  {% endfor %}
</ul>
