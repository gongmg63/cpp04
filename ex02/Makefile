CXX		=	c++
FLAGS	=	-Wall -Wextra -Werror -std=c++98
SRCS	=	main.cpp Animal.cpp Brain.cpp Cat.cpp Dog.cpp
OBJS	=	$(SRCS:.cpp=.o)
HEADER	=	Animal.hpp Brain.hpp Cat.hpp Dog.hpp
NAME	=	ex02

all : $(NAME)

$(NAME) : $(OBJS)
	$(CXX) $(FLAGS) $(OBJS) -o $(NAME)

%.o : %.cpp $(HEADER)
	$(CXX) $(FLAGS) -c $< -o $@

clean : 
	rm -rf $(OBJS)

fclean : 
	make clean
	rm -rf $(NAME)

re :
	make fclean
	make all

.PHONY : all clean fclean re
