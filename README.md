- # 익명 의견 교환 커뮤니티 <😺Cat-In-Box>

  고양이를 사랑하는 사람들이 모여 관련 이야기를 익명으로 나누는 커뮤니티 공간

  

  

  ## Stack

  - Language : Java
  - Framwork : SpringBoot
  - DB : MariaDB
  - etc... bootstrap, Thymleaf, JPA

  

  

  ## 어플리케이션 로직

  ![image-20240111155225357](https://raw.githubusercontent.com/wholeheartedness/image_repo/main/img/image-20240111155225357-1704956881526-1.png)

  ![image-20240111155236532](https://raw.githubusercontent.com/wholeheartedness/image_repo/main/img/image-20240111155236532-1704956881527-3.png)

  

  

  ## 데이터베이스 로직

  ![image-20240111155323112](https://raw.githubusercontent.com/wholeheartedness/image_repo/main/img/image-20240111155323112-1704956881527-5.png)

  ![image-20240111155336515](https://raw.githubusercontent.com/wholeheartedness/image_repo/main/img/image-20240111155336515-1704956881527-7.png)

  

  

  ## 주요 구현 기능

  | 번호 | 구현 기능        |
  | ---- | ---------------- |
  | 1    | 게시판 기능      |
  | 2    | 게시글 기능      |
  | 3    | 댓글 기능        |
  | 4    | 검색 기능        |
  | 5    | 게시글 추가 기능 |

  

  ### 1️⃣ 게시판 기능

  - Categoryid와 Board Entity를 1:n 관계로 매핑

  - Category Entity의 테이블 수에 따라 View에 출력하여 url에 따라 Board List가 출력됨

  - 해당 로직은 BoardRepository 및 BoardCategoryRepository 인터페이스와 BoardService 및 BoardCategoryService 클래스에서 구현

  - 전체 게시글 보기, 게시판별 게시글 보기 가능

    ![image-20240111155750824](https://raw.githubusercontent.com/wholeheartedness/image_repo/main/img/image-20240111155750824-1704956881527-9.png)

    ![image-20240111155808022](https://raw.githubusercontent.com/wholeheartedness/image_repo/main/img/image-20240111155808022-1704956881527-11.png)

  

  ### :️2️⃣ 게시글 기능

  - 제목과 내용으로 구성된 게시글 CRUD 기능 구현
  - 게시글 작성 시 게시판, 제목설정, 내용설정, 패스워드 설정이 가능

  