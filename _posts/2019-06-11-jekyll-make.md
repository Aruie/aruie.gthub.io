---
layout: post
title:  "Jekyll 블로그를 시작해 봅시다"
date:   2019-06-11 15:37:56 +0900
categories: [jekyll, daily]
comments: true
---

# Jekyll 블로그?

요새 아이티에 종사하는 분들 보면
대부분 블로그 주소가 github.io 가 많은데
관심없던 시절엔 그냥 깃허브에서 제공하는 도메인 서비스인가 했었는데
블로그를 만들라고 제작해준거 일줄은...

사실 인터넷을 뒤져보면 쉽게만들기 쉽게만들기 이러지만
당연하게도 네이버나 이런 플랫폼처럼 친절하진 않아요...
IT 한정으로 쉽다 그러는 느낌?
안그래도 정리못하기로 유명해서 정리하는 감각좀 익힐겸 해서 
만들면서 첫번째 포스트를 만들어 보려합니다

어짜피 누굴 보여주기라기보단 나중에 찾기 편하게 기록용도로 쓰는거라
매우 불친절하니 이해좀...
Jekyll 이 뭔지 아직도 정확힌 모르겠지만 일단 설치부터 해볼게요

원래 새로운프로그램은 다 이해하려면 끝도없어서 
일단 설치부터 하고 보는겁니다

사실 그냥 서버에서 바로 해볼까했는데
푸쉬 하고 난뒤에 새로고침을 수백번은 눌러야 적용이....
실수하면 답이없겠다 싶어서 로컬에서 작업하고 올리려고요...


## 1. 루비 및 Jekyll 설치

일단 루비기반으로 작성된 것이라 루비를 설치해야하는데
윈도에선 이게좀... 윈도버전으로 받아봅시다

https://rubyinstaller.org/downloads/

요기 가셔서 그냥 WITH DEVKIT 으로 자신에 맞는걸로 받으시면 됩니다

그후 시작메뉴에서 
Start Command Prompt with Ruby 를 실행

```
gem install jekyll
gem install minima
gem install bundler
gem install jekyll-feed
gem install tzinfo-data
```
하나씩 하실거 없이 다섯줄 다 복사해서 붙이면 알아서 한줄씩 실행 굿

#2. 블로그 연동

보니 미리 만들어 놔야했네요 지금 가서 만듭시다...

github.com 에 들어가서 새 repository를 만듭시다

이름은 <이름>.github.io 로 꼭 해주셔야 합니다

그냥하면 허전하니 README.md 생성 체크...

해도 되지만! 우린 남에껄 가져와야...하는건 아닌데 그래야 이쁘죠

전 미적감각이 제로라...

github에서 jekyll theme로 검색하시고 원하시는걸 찾은후 Fork를 해주시면 내 저장소로 바로 오게됩니다
그후 Setting에 들어가서 Template repository 를 클릭
이후 새로 repository를 생성하면 템플릿으로 사용 가능합니다
이후 터미널 혹은 git bash 에서 
```
git clone https://github.com/<아이디>/<이름>.github.io
```

를 해주시면 됩니다 

그리고는 

```
jekyll serve 
```

를 실행하면 서버가 돌아간다는데 에러...

이후 뭔짓을해도 에러가 해결이안됨...

빈 폴더에서 새로 서버를 열면되는데

기존 템플릿을 가져오면 에러가 나네요 ㅠㅠ

스택오버플로 찾아보니 개발자 킷 설치하라는데

분명 합쳐진걸로 설치했....

내일 다시도전 ㅠ

