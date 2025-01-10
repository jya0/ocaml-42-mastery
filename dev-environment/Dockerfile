# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Dockerfile                                         :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: jyao <jyao@student.42abudhabi.ae>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2025/01/10 10:30:00 by jyao              #+#    #+#              #
#    Updated: 2025/01/10 10:57:51 by jyao             ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

### ARGs declaration and initialisation
ARG UBUNTU_VER_LATEST=latest
ARG UBUNTU_VER_PENULTIMATE=jammy


### Base image
FROM ubuntu:${UBUNTU_VER_PENULTIMATE}

### Metadata about the image specified here in the Dockerfile
LABEL \
	author="jya0 <jyao@student.42abudhabi.ae>" \
	maintainer="jya0 <jyao@student.42abudhabi.ae>" \
	version="1.0" \
	description="This Dockerfile builds a dev environment to write and test OCAML code."

### Installation phase

###### OCAML setup
RUN <<EOF
apt update
apt install -y opam
opam init -y
eval $(opam env)
EOF