# PostgreSQL + C++
- 참고: https://www.youtube.com/watch?v=qDiC1Wja6Og
- 참고: https://en.wiki.imlint.org/Pqxx_tutorial

1. https://github.com/jtv/libpqxx 프로젝트 Clone

2. Visual Studio Open Folder
- Cmake 프로젝트가 있는 libpqxx 폴더 열기

3. Cmake 프로젝트 선택 후 마우스 우클릭
- Build All 실행
- Install 실행

4. out 폴더에 생성된 install 출력물
- C:\ProgramFiles\libpqxx-7.0.4 폴더로 복사

5. Visual Studio Dependencies, Includes, Libs 설정 추가
- Change configure to x64 Release and c++20 standard
- Add additional include directories C:\Program Files\libpqxx\include
- Add additional library directories C:\Program Files\PostgreSQL\13\lib and C:\Program Files\libpqxx\lib;
- Add additional dependencies libpq.lib; pqxx.lib; ws2_32.lib; wsock32.lib;

6. libpq.dll, libintl-9.dll 파일 복사
- PostgreSQL 설치 폴더에 bin 폴더에 있는 libpq.dll, libintl-9.dll 파일들을 현재 개발하는 프로젝트 폴더에 복사
- Debug/x64 폴더에도 동일하게 복사