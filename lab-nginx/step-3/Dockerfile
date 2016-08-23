# Dockerfile for building image that contains software stack provisioned by Ansible.
#


# pull base image
FROM williamyeh/ansible:mini-debian8

MAINTAINER William Yeh <william.pjyeh@gmail.com>


#
# build phase
#

#ENV PLAYBOOK playbook.yml



#
# runtime spec
#

EXPOSE 80
VOLUME ["/var/log/nginx", "/var/cache/nginx"]


#
# fix for Docker process execution model
#

ENTRYPOINT [ "nginx" ]
CMD [ "-g", "daemon off;" ]
