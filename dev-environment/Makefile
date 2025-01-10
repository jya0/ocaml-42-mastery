# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: jyao <jyao@student.42abudhabi.ae>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2025/01/10 10:29:56 by jyao              #+#    #+#              #
#    Updated: 2025/01/10 10:42:28 by jyao             ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

DOCKERFILE_PATH = ./
DOCKERFILE_NAME = Dockerfile
DOCKERFILE_FILE = $(DOCKERFILE_PATH)$(DOCKERFILE_NAME)
IMAGE_NAME = ocaml-dev-env:latest

all:
	docker build -f $(DOCKERFILE_FILE) -t $(IMAGE_NAME) $(DOCKERFILE_PATH)

clean:
	docker rmi -f $(IMAGE_NAME)

fclean: clean

re: fclean all

.PHONY: all clean fclean re