
FROM nginx
RUN apt-get -y update
RUN apt-get -y install git
RUN mkdir -p /tmp/git-repo
RUN cd /tmp/git-repo/
RUN git clone https://github.com/SEkomposter/PFolio1
RUN cp PFolio1/index.html /usr/share/nginx/html
RUN chmod 644 /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]

EXPOSE 80
