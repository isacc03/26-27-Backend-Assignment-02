# ERD 작성 참고

직접 작성한 ERD 이미지를 이 폴더에 추가합니다. 테이블 정의는 다음과 같습니다.

| 테이블 | 컬럼 |
|---|---|
| genres | id BIGINT PK, name VARCHAR(100) NOT NULL |
| books | id BIGINT PK, title VARCHAR(200) NOT NULL, author VARCHAR(120) NOT NULL, genre_id BIGINT NOT NULL FK |

`books.genre_id`는 `genres.id`를 참조합니다. 하나의 장르에는 여러 도서가 속할 수 있고, 도서는 반드시 하나의 장르에 속합니다. 텍스트 관계 정의는 [schema.mmd](schema.mmd)를 참고할 수 있습니다.
