# Binder
## 역할
신희원
 - Splash
 - Login
 - First setting
 - Search Activity
 - Post Activity
 - Search FriendList
 
홍태희
 - MainActivity
 - AddPostActivity
 - Home Fragment
 - MyPage Fragment
 - MyfrinendList Fragment
 - SearchPostList Fragment
## 가이드
### git
1.  커밋 메시지
    -   모든 커밋 메시지 앞에는 [ ? ]을 작성해서 어떤 내용을 추가, 변경 등의 작업을 했는지 확실히 구분하도록 합니다.
        -   [Add] : 신규 파일 추가
        -   [Update] : 신규 기능 추가
        -   [Fix] : 오류 수정
        -   [Delete] : 파일 삭제
        -   [Modify] : 코드 변경 (로직 동일)
        -   [Refactor] : 코드 변경 (로직 변경)
      - PR
        -   자기가 올린 PR 직접 Merge하지 않기, PR 주소 페메에 올리고 해달라고 요청
        -   코드 리뷰 대충하지 말기
        -   Conflict 나는 부분 발생 시 수정하거나 페메에 올려서 도움 요청하기.
2.  Issue
    -   버그 발생 : issue에 올리고 못 볼 수 있으니 페메에 한번씩 이슈 주소랑 뭔 문제인지 올리기, Tag : Bug
        
    -   개발 중 문제 발생 : 만들 때 힘들거나 질문도 issue에 올리기, Tag : question, help wanted
        
        → Error Logcat 등을 함께 올립시다! 오류 발생하는 부분 등...
        
    -   충돌 발생 : issue 올리고, 같은 코드를 작성한 사람을 페메로 불러주세요. Tag : conflict.
### xml & Naming
1.  xml 변수 네이밍
    
    -   TextView, EditText : `tv_{기능}_{activity_name}`
        
        → activity name은 중복되는 기능이 다른 액티비티에 있는 경우 간단하게 추가해줍니다. (모두 동일)
        
    -   Button : `btn_{기능}_{activity_name}`
        
    -   ImageView / ImageButton : `img_{기능}_{activity_name}`
        
        → 기능 칸에서 button과 view를 간단히 구분할 수 있도록 합니다.
        
        ex) `img_user`, `img_readybutton` ... (예시기 때문에 개연성 없이 작성합니다)
        
2.  xml 네이밍
    
    -   View : `activity_???`, `fragment_???`
        
    -   icon : `ic_???`
        
    -   animation : `view_an_???`
        
        → ex) dicide_an_error : DicideActivity에서 사용한 `???` animation
        
    -   vector : 애니메이션을 구현할 수도, 그냥 그린 데이터 모두 자유롭게 네이밍, 하지만 이해하지 못하게는 짓지 않는다.
        
3.  values.xml
    
    -   color.xml : @android.color에 있는지 확인한 후에 없는 경우 color에 등록한다.
        
    -   strings.xml : 우선 하드코딩한 후 마무리 작업 때 모두 정리한다.
        
        → 단 밑줄 등 html 코드나 style이 들어갈 경우 strings.xml에 미리 작성한다.
        
    -   styles.xml
        
        1.  theme naming : `{기능}Theme` 등으로 작성해 한번에 알아볼 수 있도록 작성.
