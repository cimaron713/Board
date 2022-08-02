# Board README



# API 규격서
### **HTTP Method**

- POST : 생성 (POST를 통해 해당 URI를 요청하면 리소스를 생성한다)
- GET : 조회 (GET를 통해 해당 리소스를 조회한다. 리소스를 조회하고 해당 도큐먼트에 대한 자세한 정보를 가져온다)
- PUT : 수정 (PUT를 통해 해당 리소스를 수정한다)
- DELETE : 삭제 (DELETE를 통해 리소스를 삭제한다)

| Method | URI | Description |
| --- | --- | --- |
| Get | /board/list | 리스트 조회 |
| Post | /board/register | 방명록 남기기 |
| Get | /board | redirect : /board/list |
| Post | /board/remove | 방명록 삭제 |
| Get | /board/read | 방명록 읽기 |
| Post | /board/modify | 방명록 수정 |
| get | /board/list | 검색기능 |
| Get | /board/list(page= ${result.end + 1} | 다음 페이지 |
| Get | /board/list(page= ${result.start -1} | 이전 페이지 |

| 방식 | URI | 작업 |
| --- | --- | --- |
| GET | /replies/board/{bon} | 해당 게시물의 댓글 조회 |
| POST | /replies/ | 댓글 추가 |
| DELETE | /replies/{rno} | 댓글 삭제 |
| PUT | /replies/{rno} | 댓글 수정 |


# 엔티티 관계도
![image](https://user-images.githubusercontent.com/109207727/182314999-77026384-033c-414b-9b98-0bc463f0cdb0.png)


# GIT TREE
![image](https://user-images.githubusercontent.com/109207727/182327041-d571d69e-d7bd-4acb-b823-53307e5b0d79.png)



# 소개
## 1. 메인화면
![image](https://user-images.githubusercontent.com/109207727/182326284-0c2924a6-1bc7-414c-853c-fc61bfa3c0cb.png)

## 2. 게시글 조회 및 댓글 조회
![image](https://user-images.githubusercontent.com/109207727/182326437-aa094454-ac2b-4652-8149-95a1ada60dfb.png)

### 2.1. 게시글 수정 및 댓글 수정
![image](https://user-images.githubusercontent.com/109207727/182326626-218156c4-ea12-4ca5-9ad6-9454c062d4eb.png)
![image](https://user-images.githubusercontent.com/109207727/182326664-fccbccec-f2e6-4def-8513-a6b9f7beb919.png)

## 3. 검색기능
![image](https://user-images.githubusercontent.com/109207727/182326841-55b38267-32bf-4d53-9b68-d412349b9d73.png)

