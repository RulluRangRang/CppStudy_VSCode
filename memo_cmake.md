# 1. Cmake 설치 
- URL: https://cmake.org/download/
- Add Cmake to the system PATH for the current user에 체크 후 설치
- Cmake 버전 체크

        $ cmake --version

# 2. GCC 설치(MSYS2)
- URL: https://www.msys2.org/
- 참고: https://www.devdungeon.com/content/install-gcc-compiler-windows-msys2-cc

- MSYS2 업데이트(msys2 실행 후)
```
$ pacman -Syu
```


# 3. Cmake 프로젝트 설정
- 참고: https://junstar92.tistory.com/204
- cpp 파일 작성
- CmakeLists.txt 아래와 같이 작성 

```
cmake_minimum_required(VERSION 3.23.2)
 
# set the project name
project(cmake_study)
 
# add the executable
add_executable(${PROJECT_NAME} cmake_study.cpp)
```
- build 폴더 생성해주기
```
PS> mkdir build
```

- build 폴더 경로에서 cmake 명령
```
PS> cmake ..
```

# TODO 
Compiler를 MSVC에서 GCC로 변경하여 cmake 처리하기