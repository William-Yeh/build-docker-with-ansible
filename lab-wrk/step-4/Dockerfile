# Dockerfile for building image that contains software stack provisioned by Ansible.
#


# pull base image
FROM williamyeh/ansible:mini-alpine3

MAINTAINER William Yeh <william.pjyeh@gmail.com>


#
# build phase
#

#ENV PLAYBOOK playbook.yml


#
# runtime spec
#

ENTRYPOINT [ "wrk" ]
