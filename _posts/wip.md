### 5. jekyll의 디렉토리 구조 파악하기
우리가 직접 블로그를 개발했다면, 디렉토리 구조를 마음대로 짰을텐데
현재는 jekyll이 정한 디렉토리 구조로 되어있습니다.
앞으로 이렇게 이미 짜놓은 디렉토리 구조를 많이 접할텐데, 구조를 파악하면 개발 속도가 금방 빨라집니다.

* _config.yml 설정파일입니다. 블로그 제목이나 이메일 등을 수정하면 실제 블로그에 적용이 됩니다. 각자 설정에 맞게 수정해보세요.
* _includes/ 여러 페이지에서 반복할 코드의 템플릿이 포함된 디렉토리입니다. footer, header등을 넣을 수 있습니다.
* _posts/ 이 디렉토리 밑에 글을 쓰면 됩니다. jekyll이 정한 이름 convention을 잘 지켜주셔야 포스팅이 올라갑니다.
* _layouts/ 포스트 글의 디자인이 적용된 템플릿이 있는 디렉토리 입니다.


### 7. 테마 수정 (HTML/CSS 변경)

About 페이지를 수정해볼까요?
혹시 이 기본 theme이 싫으신 분은 먼저 theme을 변경한 후에 수정하시면 됩니다.

default theme인 minima가 어디 위치해있는지 확인합니다.
bundle show minima


아래의 경로로 이동합니다.
/Users/AllieKim/.rvm/gems/ruby-2.4.2/gems/minima-2.5.0



수정하고 싶은 요소를 가져와서 변경하면, jeykyll에서 overwrite하여 보여주게 됩니다.
