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
    <td align="center"><a href="https://github.com/lrkdms125"><img src="https://avatars.githubusercontent.com/dlrkdms125" width="150px;" alt=""></td>
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
**DB 서버 : Active - Active**

각각의 서버가 Master, Slave 역할을 동시에 수행한다.

**Active - Active 선택 이유**
- 양방향 복제를 통해 **두 서버는 항상 동일한 데이터를 유지**할 수 있다.
- 두 서버의 데이터가 일관되게 유지되기 때문에 **로드 밸런서로 부하를 분산**시킬 수 있다.
- 한 서버에 문제가 생기더라도 다른 서버로 요청을 지속적으로 처리할 수 있어서 **에러 대처 능력**이 뛰어나다.
- 이커머스 특성 상, **상품을 사용자에게 보여주는 부분이 많기 때문에** 빠른 속도로 상품을 보여주기 위해 클러스터 방식보단 Active - Active 구성이 더 적합하다고 판단했다.

**재난 복구 계획**
- 프로메테우스, 그라파나와 같은 모니터링 시스템을 통해 DB 서버의 상태를 확인한다.
- DB 서버에 문제가 발생했을 경우, 문제가 발생하지 않은 DB 서버의 로그 파일을 기반으로 문제 DB 서버를 복구한다.


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


