# Sprint boot?

## db 접속정보

src/main/resources  
application.properties

- MySQL 설정  
  spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

- DB Source URL 설정
- 예시) spring.datasource.url=jdbc:mysql://localhost:3306/test_db?useSSL=false&useUnicode=true&serverTimezone=Asia/Seoul  
  spring.datasource.url=jdbc:mysql://localhost:3306/mydb241119?useSSL=false&useUnicode=true&serverTimezone=Asia/Seoul&allowPublicKeyRetrieval=true

- DB 사용자 이름 설정
- 예시) spring.datasource.username=root  
  spring.datasource.username=kjg24

- DB 사용자이름에 대한 암호 설정
- 예시) spring.datasource.password=root  
  spring.datasource.password=temp

- true 설정 시, JPA 쿼리문 확인 가능  
  spring.jpa.show-sql=true

- DDL(create, alter, drop) 정의 시, DB의 고유 기능을 사용할 수 있음.  
  spring.jpa.hibernate.ddl-auto=update

- JPA의 구현체인 Hibernate가 동작하면서, 발생한 SQL의 가독성을 높여줌.  
  spring.jpa.properties.hibernate.format_sql=true

## 자동증가값까지 반환으로 받기

Mapper에서
@Options(useGeneratedKeys=true, keyProperty="컬럼명")
