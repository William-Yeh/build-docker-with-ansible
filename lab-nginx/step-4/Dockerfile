# Dockerfile for building image that contains software stack provisioned by Ansible.
#


# pull base image
FROM williamyeh/ansible:mini-alpine3

MAINTAINER William Yeh <william.pjyeh@gmail.com>


#
# build phase
#

#ENV PLAYBOOK      playbook.yml
#ENV REQUIREMENTS  requirements.yml


#
# runtime spec
#

EXPOSE 80
VOLUME ["/var/log/nginx"]


#
# fix for Docker process execution model
#

ENTRYPOINT [ "nginx" ]
CMD [ "-g", "daemon off;  pid /dev/null;  error_log stderr;" ]
