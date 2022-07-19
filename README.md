# 예담 최종프로젝트, 'YFactory'
### 예담직업전문학교(교육기관)에서 팀 단위로 실시한 최종프로젝트 결과물입니다.
### 저희팀은 'MES(생상공정 관리 시스템)' 이라는 주제로 프로젝트를 만들게 되었습니다.

## <a href="https://github.com/Hyeonjinkk/yFactory" target="_blank">전체 프로젝트 바로 보기 ▶️</a>

## 개요
### MES란?
* MES는 제품주문에 의한 착수에서 완성품의 품질검사까지 전 생산활동을 관리하는 시스템으로 생산실적, 제품 품질정보 등을 실시간으로 수집하여 고품질의 수익 지향적 생산체제를 갖추게 하는 **통합 생산관리시스템**

## 설계의 주안점
1. <b>Lombok</b>을 이용하여 어노테이션 설정으로 간단하게 VO 객체를 생성하여 코드를 간결화 시켜줌.
2. <b>Controller</b>을 이용하여 어노테이션 설정으로 페이지 Redirection 처리.
3. <b>RestController</b> 어노테이션 설정으로 <b>Script</b>내에서 비동기 처리를 @Controller와 구분하여 개발 효율성 증대.
4. <b>Toast UI Chart</b> 라이브러리를 이용해 설비 온도 상태와 생산 시작 시 실시간으로 생산량 증가를 체크하도록 구현.
5. <b>AJAX</b>를 통해 페이지 로딩속도 및 클라이언트에게 편리성 제공.
6. <b>BootStrap</b>을 활용한 반응형 페이지 제작 및 Modal 활용.
7. <b>Jasper Studio</b> 라이브러리를 이용해 페이지 내 PDF출력물 형식 구현.
## Contens
```sh
* 영업관리
* 자재관리
* 생산관리
* 품질관리
* 설비관리
```

## <span style="color:red">차별점</span>
### 저희는 학원에서 배우기만 한 기술스택이 아닌, 저희 스스로가 학습하여 새로운 기술스택을 활용해보았습니다. 
### 이 프로젝트는 Spring Boot, thymeLeaf를 활용하여 서비스를 구축하였습니다. 
### 또한 저 개인적으로, 마크다운 이라는 언어를 스스로 공부하여 깃허브 데스크탑과 연동해 포트폴리오를 깃허브에 업로드 했습니다. 



## 사용기술 및 개발환경

<img src="/개발환경.jpg" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<hr>

|Category|Detail|
|:---:|:---:|
|OS|Windows 10 pro|
|개발언어|Java(11), Servlet, SpringMVC2, Mybatis, HTML5, Javascript, CSS|
|데이터베이스|Oracle Database Express Edition 11g Release 2|
|서버|TOMCAT 9.0|
|IDE|Eclipse IDE|
|빌드 배포|Maven, jenkins|
|테스트 툴|Junit|
|프로세스|Intel(R) Core  i7-10700 CPU @ 2.90GHz|
|메모리|16GB RAM|
|보조 기억장치|SSD 512GB|
|형상관리|GitHub|

## 프로젝트 기능 구현

<ul>
  <li>영업관리</li>
    <ul><li>주문서 조회</li></ul>
    <ul><li>BOM 관리</li></ul>
    <ul><li>LOT 재고 조회</li></ul>
    <ul><li>안전 재고 관리</li></ul>
    <ul><li>출고 관리</li></ul>
  <li>자재관리</li>
    <ul><li>발주 및 입고 관리</li></ul>
    <ul><li>안전 재고 관리</li></ul>
  <li>생산관리</li>
    <ul><li>생산 계획 및 지시 관리</li></ul>
    <ul><li>생산 및 공정 실적 관리</li></ul>
    <ul><li>공정 및 공정 흐름도 관리</li></ul>
  <li>품질관리</li>
    <ul><li>품질 검사 등록 및 관리</li></ul>
    <ul><li>품질 검사 결과 및 불량 내역 조회</li></ul>
  <li>설비관리</li>
    <ul><li>설비 점검 관리</li></ul>
    <ul><li>설비 실시간 온도 및 생산량 상태 조회</li></ul>
</ul>


# 페이지 소개
## 1.1 영업관리 - 주문서 조회
<img src="/images/영업-주문서조회.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 영업관리의 주문서 조회입니다. 
##### 해당 페이지에서는 주문의 정보를 확인할 수 있습니다.
##### 목록의 주문 코드를 더블클릭하게 되면 해당 주문의 상세 주문 내역을 열람할 수 있는 모달이 출력됩니다. 
##### 금일의 매출 부분입니다. 구글차트를 통해 차트를 표현했으며, 현재 차트가 표시되지 않는 이유는 당일날의 매출이 없기 때문입니다. 

## 2.1 생산관리 - 계획 등록
<img src="/images/생산-계획등록.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 생산 계획 관리입니다.
##### 생산 계획관리는 제품을 생산 하기전에 생산 계획을 등록하는 페이지로 관리와 등록으로 나뉘어집니다.
##### 주문이 등록되거나 재고를 늘릴때 생산계획을 생성할 수 있습니다.
##### 주문서 목록이 출력되며, 주문코드를 선택하면 주문목록을 조회해옵니다.
##### 필수 내용에 맞게 입력한 후, 계획등록 버튼을 클릭하면 확인창이 출력됩니다.

## 2.2 생산관리 - 지시 등록
<img src="/images/생산-지시등록.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 생산 지시 등록입니다.
##### 생산지시관리는 미지시 계획을 조회하고, 미지시 계획에 대하여 생산을 지시할 수 있는 페이지입니다.
##### 미지시 계획 조회를 클릭하면 미지시 계획 목록이 출력됩니다.
##### 생산계획코드를 클릭하면 생산지시를 생성할 수 있으며, 생산계획에 따른 라인코드가 입력됩니다.
##### 필수 내용을 입력한 후 조회를 클릭하면 해당 라인 공정에 사용되는 필요자재를 조회합니다.
##### 자재코드 클릭시, 공정에 투입할 자재를 선택할 수 있는 자재 LOT 목록을 출력합니다.
##### 등록된 자재를 선택 및 수량 입력 후 생산지시 등록을 하게 되면 확인창이 출력되고 승인을 하면 생산지시 등록이 완료됩니다.

## 2.3 생산관리 - 생산
<img src="/images/생산-생산.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 생산관리의 생산입니다.
##### 라인에 맞는 공정을 통해 제품을 생산하는 페이지입니다.
##### 생산지시 목록을 클릭시, 생산 지시 목록을 조회할 수 있습니다.
##### 생산 시작할 생산지시코드를 클릭하면 진행생산지시 목록이 추가되고, 공정 목록에서 공정별 진행상황을 확인할 수 있습니다.
##### 생산시작 클릭 시 첫 순번 공정 상태가 진행 상태로 바뀌며 작업시작시간이 입력되고 실시간으로 생산이 진행됩니다.
##### 순번의 합격량이 일정 수량을 넘으면 다음 순번의 공정이 진행됩니다.
##### (생산시작시 프로시저를 통해 생산이 시작되어지고 , 이전 공정의 합격량이 일정량을 넘기면 다음 공정이 진행됩니다.)


## 3.1 원자재 - 발주등록
<img src="/images/자재-발주등록.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 발주등록 페이지 입니다.
##### 생산 지시하지 않은 생산계획서를 통해 생산계획코드를 조회합니다.
##### 체크박스 항목을 클릭후 선택버튼을 클릭시 bom을기반으로 생산계획별 부족한 원자재를 조회할수있습니다.
##### 선택버튼클릭시 부족한원자재를 기반으로 현재고를 파악하여 계획대비 필수량과 발주량을 확인할수있으며 발주신청이 가능합니다.
##### 저장버튼을 누르면 등록 알림창이뜨고, 저장이 완료되는순간 프로시저를 이용하여 원자재 발주코드와 발주상세코드를 자동 생성하도록 구현하였습니다.

## 3.2 원자재 - 입고등록
<img src="/images/자재-입고등록.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 입고등록 페이지 입니다.
##### 검수가 끝난 입고예정인 원자재를 입고시키는 페이지입니다.
##### 추가버튼을 클릭시 입고예정인 원자재를 조회하는 모달창을 출력하고 체크 후 선택 시 입고등록페이지에 넘겨줍니다.
##### 입고등록페이지에 추가된원자재는 입고예정목록 모달창에선 조회할수없으며 체크박스를 선택후 삭제버튼을 클릭하면 다시 조회가 가능합니다.
##### 저장버튼을 클릭하면 승인알림창이뜨며, 승인시 프로시저를 통해 입고예정인 원자재를 입고처리할수있으며, 입고예정에서는 삭제됩니다.

## 4.1 품질관리 - 검사등록
<img src="/images/자재-입고등록.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 품질검사 관리 페이지 입니다.
##### 발주된 자재들을 입고하기 위해 품질검사를 요청하는 페이지입니다.
##### 돋보기 아이콘을 클릭하면 발주코드를 조회하는 모달창을 출력합니다.
##### 출력된 모달창에서 요청할 발주코드를 더블클릭하면 품질검사요청 페이지에 각 입력창에 자동으로 입력됩니다.
##### 신청버튼을 클릭하면, 프로시저를 이용해 해당 발주코드가 갖고 있는 모든 발주정보들이 검사관리에 등록되며 요청이 완료됩니다.
##### 요청된 발주코드들의 발주정보들을 조회할 수 있으며, 품질을 검사하는 페이지입니다.
##### 합격량을 더블클릭하면 입력창이 활성화되어 입력할 수 있으며, 불량량은 발주량에서 합격량을 뺀 값이 자동으로 입력됩니다.
##### 불량량까지 입력된 발주정보는 불량코드를 등록할 수 있습니다.
##### 완료버튼을 클릭 시 프로시저를 이용해 검사한 자재들의 품질정보가 입력됨과 함께 합격량은 자재LOT번호를 부여받고 입고예정량으로 들어가게 됩니다.

## 5.1 설비관리 - 설비 실시간 상태
<img src="/images/설비-실시간.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 설비 실시간 상태 페이지 입니다.
##### 각 라인의 공정들의  온도와 생산량을 실시간으로 볼 수 있도록 구현하였습니다.
##### 설비 실시간 온도에 경우 확인하고 싶은 라인을 클릭하면 선택한 라인의 각 공정 별 온도를 실시간으로 보여줍니다.
##### 설비 실시간 생산량에 경우에도 확인하고 싶은 라인을 클릭할 경우 생산이 시작된  해당 라인의 각 공정들의 생산량을 보여줍니다.

# 소스코드 소개
## 2.1 출퇴근시간을 계산해서 percent로 보여주는 쿼리

```xml:workerAttendance_mapper.xml

<select id="getPercent" resultType="com.yedam.tfprj.admin.workerAttendance.service.WorkerAttendanceVO">
        SELECT W.WORKER_ID,
               S.ATT_DT,
               W.GOING_TIME,
               QUITTING_TIME,
               TO_DATE(S.IN_TIME, 'YY-MM-DD HH24:MI') AS inMTime,
               S.OUT_TIME,
               ROUND(((current_date - TO_DATE(S.IN_TIME, 'YY-MM-DD HH24:MI')) *24)/((QUITTING_TIME - GOING_TIME) *24),2) * 100  AS percent,
               ROUND((W.QUITTING_TIME - current_date) * 24 * 60 * 60, 2) AS getMTime
        FROM WORKSHEET W, STAFF_ATTENDANCE S
        WHERE W.WORKER_ID = S.WORKER_ID
               AND S.ATT_DT = TO_CHAR(current_date, 'YY-MM-DD')
               AND TO_CHAR(W.GOING_TIME, 'YY-MM-DD') = S.ATT_DT
               AND W.WORKER_ID = #{workerId}
    </select>
```

## 2.2 회원, 비회원의 매출을 구분하여 보여주는 쿼리

```xml:workerAttendance_mapper.xml

<select id="findMemNonMem" resultType="map">
        SELECT CASE WHEN MEMBER_ID = '0' THEN '비회원' ELSE '회원' END AS "member", SUM(PAYMENT_AMOUNT) AS "paymentAmount"
        FROM PAYMENT
        where TO_CHAR(PAYMENT_DATE, 'YYYY-MM-DD') BETWEEN #{firstDate} AND #{lastDate}
        <if test='day != 0'>
            AND TO_CHAR(PAYMENT_DATE, 'D') = #{day}
        </if>
        GROUP BY CASE WHEN MEMBER_ID = '0' THEN '비회원' ELSE '회원' END
    </select>

```

## 2.3 현재 출근한 근무자의 정보를 조회할 수 있는 쿼리

```xml:workerAttendance_mapper.xml
<select id="getNowWorker" resultType="com.yedam.tfprj.admin.workerAttendance.service.WorkerAttendanceVO">
        SELECT A.WORKER_ID,
               A.IN_TIME,
               A.OUT_TIME,
               A.IS_LATE,
               A.IS_ABSENCE,
               I.WORKER_NAME, W.GOING_TIME, W.QUITTING_TIME, A.ATT_DT ,I.POSITION_CD, I.USERTYPE, I.STARTDAY, I.ALLPAY
        FROM STAFF_ATTENDANCE A
                 INNER JOIN STAFF_INFORMATION I
                            ON A.WORKER_ID = I.WORKER_ID
                 INNER JOIN WORKSHEET W
                            ON I.WORKER_ID = W.WORKER_ID
        WHERE TO_CHAR(current_date, 'yy-MM-dd hh24:mi') BETWEEN A.IN_TIME AND TO_CHAR(W.QUITTING_TIME, 'yy-MM-dd hh24:mi')
          AND TO_DATE(A.ATT_DT, 'yy-MM-dd') = TO_DATE(current_date, 'yy-MM-dd')
          AND A.OUT_TIME IS NULL
          and to_char(w.going_time, 'yy-MM-dd') = a.att_dt
    </select>
```




#### 해당 내용은 프로젝트의 일부분을 소개한 것입니다. 포트폴리오를 더 상세하게 조회하고 싶으시면
#### 메인 브랜치의 pdf를 참고 해 주시면 감사하겠습니다.

#### 감사합니다.

