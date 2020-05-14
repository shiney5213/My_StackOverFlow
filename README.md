# My_StackOverFlow

> 기억하면 좋은 코드, 문제해결방법들 
>
## Python
- [중첩 리스트 flatten](https://github.com/shiney5213/My_StackOverFlow/blob/master/1.%20python-list_flatten.ipynb) :  sum(list, [])  이용
- [paths.list_image](https://github.com/shiney5213/My_StackOverFlow/blob/master/2.%20python-fine_imga_in_dir.ipynb) : 폴더 내 있는 모든 이미지 찾기(imutils 패키지)
- [random](https://github.com/shiney5213/My_StackOverFlow/blob/master/3.%20python-list_random_shuffle_.ipynb) : random.shuffle(), random.sample(), random.randint() 등
- [if elif else문]([https://github.com/shiney5213/Study-Algorithm/blob/master/%EB%8B%A8%EA%B3%84%EB%B3%84%EB%A1%9C%ED%92%80%EC%96%B4%EB%B3%B4%EA%B8%B0/10.9_1002(%ED%84%B0%EB%A0%9B).ipynb](https://github.com/shiney5213/Study-Algorithm/blob/master/단계별로풀어보기/10.9_1002(터렛).ipynb)
  - 출력값 if(조건) else 출력값 if (조건) else 출력값 if(조건)
  - 예: -1 if (r==0 and r1==r2) else 1 if (r == r1+r2 or m==sum(R)) else 0 if (m > sum(R)) else 2



## WorkSpace
- [가상환경](https://github.com/shiney5213/My_StackOverFlow/blob/master/WorkSpace/1.virtualenv.md) : virtualenv, anaconda 사용
- [Colab](https://github.com/shiney5213/My_StackOverFlow/blob/master/WorkSpace/2.google_colab_import.md) : 내 파일 import (os.chdir()로 working directory 바꿔야 함.)
- [jupyter Notebook Extenstion](https://github.com/shiney5213/My_StackOverFlow/blob/master/WorkSpace/3.jupyter_notebook_extension.md): jupyter notebook의 다양한 확장기능 사용



## Linux
- Prosess
	- 진행중인 python ps 찾기: ps - ef |grep python
	- ps  kill : sudo kill PID / kill -9 PID
	- 모든 ps, 메모리 확인: top
	- 메모리 확인: df
-  이동/복사
  - dir전체 복사: cp -r 원래dir 목적지dir
  - dir전체 이동: mv -r 원래dir 목적지dir
- dir, file 크기 확인
	- 하위 dir, file 크기 모두 표시(kbyte) : du /dir
	- 선택한 dir, file 크기 확인(kbyte) : du -s /dir
	- 읽기편한단위로 확인(Mbyte): du -sh / dir
- dir, file 개수
	- 현 dir 내 dir 개수 : ls -l | grep ^d | wc -l      or        ls -A | wc -l     
	- 현 dir 내 파일 개수 : ls -l |grep ^- |wc -l    
	- 현 dir 내 하위 폴더 내 모든 파일 개수 : find . -type f | wc -l
	-   폴더 위치 지정 후 하위 폴더 내  파일 개수 세기 : find /폴더/경로 -type -f | wc -l
- 파일 삭제
	- 모든 파일 삭제 : rm \*
	- 특정 파일 삭제 :  rm filename
	- 특정 확장명 파일 삭제: rm \*.txt
- dir 삭제
	- dir 삭제: rm -r dir/
	- 강제로 삭제: rm -rf dir/
- 압축
	- 현재 폴더 전체 압축: zip dir.zip ./\*
	- 압축 풀기: unzip aaa.zip -d dirname
- 편집기 명령어
  - [vi, vim 명령어](https://hyeonstorage.tistory.com/274)
- 파일의 내용을 뒤에서부터 출력
  - 파일에 내용이 뒤에 추가될때마다 추가된 내용 보내줌: tail -f file
- nohup 
  - nohup file.py >tf.log  2>&1 &
- 포그라운드 -> 백그라운드
  - ctrl + z: stoped
  - jobs : 실행한 ps에 대해 확인하는 명령어
  - bg %1 : 백그라운드로 실행 ( 명령어 뒤에 &가 붙어서 실행됨)
- CUDA 버전 확인: nvcc --version
- Django Web Server 실행
  - python manage.py runserver  127.0.0.1:8000
  - 접속: ip주소:8000



# Reference

- vi, vim 명령어 : [https://hyeonstorage.tistory.com/274](https://hyeonstorage.tistory.com/274)

