##
## EPITECH PROJECT, 2018
## Makefile
## File description:
## Makefile -- project
##

SRC 		= 	main.c \
				src/utils.c \
				src/generator.c \
				src/linked_list.c \
				src/make_imperfect.c \

OBJ		=	$(SRC:.c=.o)

NAME 		=	generator

RM 		=	rm -f

RM_TRASH=	*.o *~ *.gcno *.gcda libmy.a *.gch *.data

CFLAGS	= 	-pedantic -Wall -Wextra -W -g -O2 -lm

all:	$(NAME)

$(NAME):	$(OBJ)
	gcc $(OBJ) -o $(NAME) $(CFLAGS)

clean:
	$(RM) $(RM_TRASH)
	cd include && $(RM) $(RM_TRASH)
	cd src && $(RM) $(RM_TRASH)
	make fclean -C bonus/generator

fclean: clean
	$(RM) $(NAME)

re: fclean all
