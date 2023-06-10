FROM nginx:alpine
# remove default nginx configuration file
RUN rm /etc/nginx/conf.d/default.conf
# replace with custom one
COPY nginxproxy/nginx.conf /etc/nginx
# you need to overwrite the default nginx configurations
# --------- /only for those using react router ----------
# expose port 80 to the outer world
#EXPOSE 8080
# start nginx 
CMD ["nginx", "-g", "daemon off;"]
