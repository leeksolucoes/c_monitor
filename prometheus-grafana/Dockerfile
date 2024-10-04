FROM nginx:alpine

# Crie e ajuste as permissões dos diretórios necessários
RUN mkdir -p /var/cache/nginx /run && \
    chown -R nginx:nginx /var/cache/nginx /run

# Copie a configuração do Nginx
COPY ./nginx/nginx.conf /etc/nginx/nginx.conf

# Execute o Nginx como o usuário 'nginx'
USER nginx

CMD ["nginx", "-g", "daemon off;"]
