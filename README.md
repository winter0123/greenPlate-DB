<h1 align="center">GreenPlate</h1>

<div align="center">
   <img src="./img/greenplateimg.jpg"  style="width:60% ;" align="center"/>
</div>  
<br>

> [플레이 데이터] 한화시스템 BEYOND SW캠프  
> 6기 1차 프로젝트 팀 404x
## 🤚 404x 팀원
<table>
 <tr>
    <td align="center"><a href="https://github.com/ohgyulim"><img src="https://avatars.githubusercontent.com/ohgyulim" width="150px;" alt=""></td>
    <td align="center"><a href="https://github.com/wns2212"><img src="https://avatars.githubusercontent.com/wns2212" width="150px;" alt=""></td>
    <td align="center"><a href="https://github.com/dyun23"><img src="https://avatars.githubusercontent.com/dyun23" width="150px;" alt=""></td>
    <td align="center"><a href="https://github.com/lrkdms125"><img src="https://avatars.githubusercontent.com/lrkdms125" width="150px;" alt=""></td>
    <td align="center"><a href="https://github.com/winter0123"><img src="https://avatars.githubusercontent.com/winter0123" width="150px;" alt=""></td>
  </tr>
  <tr>
    <td align="center"><b>Team Leader</b> <br> <a href="https://github.com/ohgyulim"><b>오규림</b></td>
    <td align="center"><a href="https://github.com/wns2212"><b>권준형</b></td>
    <td align="center"><a href="https://github.com/dyun23"><b>김다윤</b></td>
    <td align="center"><a href="https://github.com/dlrkdms125"><b>이가은</b></td>
    <td align="center"><a href="https://github.com/winter0123"><b>장유정</b></td>
  </tr>
  </table>

## 📌 프로젝트 주제 
### 건강한 삶을 위한 나만의 식재료 추천 사이트 
레시피를 추천해주고, 레시피 속 필요한 재료를 한 번에 담을 수 있는 기능을 제공

레시피에 사용된 재료 각각의 칼로리를 보여주고, 장바구니에 상품을 담았을 때 장바구니에 담긴 전체 상품의 칼로리 합계를 보여주는 기능 

라이브 스트리밍과 커머스의 합성어인 라이브커머스 서비스 제공
[추가 자료](https://github.com/beyond-sw-camp/be06-1st-404x-GreenPlate/wiki/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EA%B0%9C%EC%9A%94)

## 🔧 기술 스택
운영 환경  
 ![](https://img.shields.io/badge/VMware-607078?logo=vmware&logoColor=white&style=for-the-badge) ![Cent OS](https://img.shields.io/badge/cent%20os-002260?style=for-the-badge&logo=centos&logoColor=F0F0F0)  
DB  
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white)  
모니터링  
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white)
협업 툴  
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) ![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=for-the-badge&logo=notion&logoColor=white)  
[세부 사항 위키](https://github.com/beyond-sw-camp/be06-1st-404x-GreenPlate/wiki/%EA%B8%B0%EC%88%A0-%EC%8A%A4%ED%83%9D)

## 📄 요구사항 명세서
[스프레드 시트 링크](https://docs.google.com/spreadsheets/d/18xtuXo7vrMqQ2GdFQdnLxmKsj9kOOjgsPDi9ZospRJM/edit#gid=0)


## ERD 다이어그램
   <img src="./img/ERDimg.png"  style="width:80% ;" align="center"/>  
  
[ERD 링크](https://www.erdcloud.com/d/f3onDN2odBNSReR5x)

## 🖥️ 시스템 아키텍처
   <img src="./img/architecture.png"  style="width:80% ;" align="center"/>

## ✨ DR(재난 복구)
- DB 서버 : Master - Slave 방식 사용  
DB의 요청의 절반 이상이 읽기 요청이기 때문에 Replication 구성 선택

## 📚 SQL 실행 결과
<!--
<details>
<summary>회원 가입</summary>
<div>
<figure align="center"> 
  
 </figure>
</div>

</details>

<details>
<summary>로그인</summary>
<div>
<figure align="center"> 

 </figure>
</div>

</details>
-->


