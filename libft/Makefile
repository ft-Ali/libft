# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: alsiavos <alsiavos@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/11/08 13:57:01 by alsiavos          #+#    #+#              #
#    Updated: 2023/11/16 16:32:22 by alsiavos         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a 

CC = cc

FLAGS = -Wall -Wextra -Werror -I.

AR = ar

RM = rm -f

FILES = ft_strdup.c \
		ft_atoi.c \
		ft_bzero.c \
		ft_isalnum.c \
		ft_isalpha.c \
		ft_isascii.c \
		ft_isdigit.c \
		ft_isprint.c \
		ft_memchr.c \
		ft_memcmp.c \
		ft_memcpy.c \
		ft_memmove.c \
		ft_memset.c \
		ft_strchr.c \
		ft_strlcat.c \
		ft_strlcpy.c \
		ft_strlen.c \
		ft_strncmp.c \
		ft_strnstr.c \
		ft_strrchr.c \
		ft_tolower.c \
		ft_toupper.c \
		ft_calloc.c \
		ft_putstr_fd.c \
		ft_putchar_fd.c \
		ft_itoa.c \
		ft_putnbr_fd.c \
		ft_substr.c \
		ft_putendl_fd.c \
		ft_strmapi.c \
		ft_strtrim.c \
		ft_striteri.c \
		ft_strjoin.c \
		ft_split.c \

OBJS = ${FILES:.c=.o}


BONUS	=	ft_lstadd_back.c ft_lstadd_front.c ft_lstclear.c ft_lstdelone.c \
		ft_lstiter.c ft_lstlast.c ft_lstmap.c ft_lstnew.c ft_lstsize.c \

BOBJS	=	$(BONUS:.c=.o)
.c.o: 	
		${CC} ${FLAGS} -c $< -o ${<:.c=.o}

${NAME}: 	${OBJS}
		ar rcs ${NAME} ${OBJS} 

all: 		$(NAME)

clean:
	$(RM) $(OBJS) $(BOBJS)

fclean: clean
	$(RM) $(NAME)

re: clean all

bonus:	$(OBJS) $(BOBJS)
		ar rcs $(NAME) $(OBJS) $(BOBJS)

.PHONY:		all clean fclean re bonus