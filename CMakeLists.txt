cmake_minimum_required(VERSION 2.8)	 # Проверка версии CMake.
										# Если версия установленой программы
										# старее указаной, произайдёт аварийный выход.

project(compArchLab2)			# Название проекта

add_library(
	aklab2 
	STATIC 
	aklab2.cpp
)	# Создание статической библиотеки с именем aklab2

add_executable(
	main 
	main.cpp
)	# Создает исполняемый файл с именем main

target_link_libraries(main aklab2)		# Линковка программы с библиотекой
