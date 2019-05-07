---
layout: post
title:  "CVAT setup Manual"
date:   2019-05-07 10:05:42 +0900
categories: jekyll update
---

CVAT github : https://github.com/opencv/cvat
깃헙의 INSTALLATION 참고해서 설치

Docker의 경우 필자는 Oracle Virtual Machine 을 사용중인지라, 충돌을 피하기 위해서 Docker Tool Box를 통해서 Docker를 설치함

Docker Tool Box : https://docs.docker.com/toolbox/overview/


CVAT github의 INSTALLATION 설명에 따라 설치가 완료되면, 외부에서도 접속할 수 있도록 추가 설정이 필요함

1. CVAT github의 Advanced settings 설명에 따라서 docker-compose.override.yml 생성하기
2. Docker의 CVAT에 대한 포트값 확인 및 포트포워딩 확인 : https://min-it.tistory.com/20 https://blog.ggaman.com/997
3. netsh를 통해서 포트포워딩 설정 및 해당포트 방화벽 해제하기
 : 포트포워딩 https://www.tuwlab.com/ece/29011
 : 방화벽 해제 https://www.snoopybox.co.kr/1627


완료되면 외부에서도 Docker가 설치된 PC의 IP로 접속할 수 있다.

이후, CVAT 사용을 위해서는 관리자 생성이 필요하니
CVAT 깃헙의 Create superuser account를 참고해서 설정해주면 완료
 

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
