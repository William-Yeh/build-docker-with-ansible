# Dockerfile for building image that contains software stack provisioned by Ansible.
#


# pull base image
FROM williamyeh/ansible:debian8-onbuild

MAINTAINER William Yeh <william.pjyeh@gmail.com>


#
# build phase
#

#ENV PLAYBOOK playbook.yml
RUN ansible-playbook-wrapper



#
# runtime spec
#

EXPOSE 80
ENTRYPOINT [ "nginx" ]
