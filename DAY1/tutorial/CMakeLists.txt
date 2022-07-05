cmake_minimum_required (VERSION 2.6) # Cmake 필요 버전 정의

Project (Tutorial) # 프로젝트 이름 정의

include_directories("include/my_math")

add_library(MathFunctions src/my_math/mysqrt.cpp)# 라이브러리 추가
Add_executable(Tutorial src/tutorial.cpp) # 실행파일 정의(main 함수가 포함된 코드)
Target_link_libraries(Tutorial MathFunctions) # 라이브러리 링크
