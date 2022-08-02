# Board README


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


### 엔티티 관계도
![image](https://user-images.githubusercontent.com/109207727/182314999-77026384-033c-414b-9b98-0bc463f0cdb0.png)
