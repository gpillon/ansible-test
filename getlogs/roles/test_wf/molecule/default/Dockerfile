{% if item.registry is defined %}
FROM {{ item.registry.url }}/{{ item.image }}
{% else %}
FROM {{ item.image }}
{% endif %}

# we install it with pip3
RUN dnf install -y python3-pip diffutils