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
## 1.1.1 영업관리 - 주문서 조회
<img src="/images/영업-주문서조회.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 영업관리의 주문서 조회입니다. 
##### 해당 페이지에서는 주문의 정보를 확인할 수 있습니다.
##### 목록의 주문 코드를 더블클릭하게 되면 해당 주문의 상세 주문 내역을 열람할 수 있는 모달이 출력됩니다. 
##### 금일의 매출 부분입니다. 구글차트를 통해 차트를 표현했으며, 현재 차트가 표시되지 않는 이유는 당일날의 매출이 없기 때문입니다. 

## 1.2.1 생산관리 - 계획 등록
<img src="/images/생산-계획등록.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 생산 계획 관리입니다.
##### 생산 계획관리는 제품을 생산 하기전에 생산 계획을 등록하는 페이지로 관리와 등록으로 나뉘어집니다.
##### 주문이 등록되거나 재고를 늘릴때 생산계획을 생성할 수 있습니다.
##### 주문서 목록이 출력되며, 주문코드를 선택하면 주문목록을 조회해옵니다.
##### 필수 내용에 맞게 입력한 후, 계획등록 버튼을 클릭하면 확인창이 출력됩니다.

## 1.2.2 생산관리 - 지시 등록
<img src="/images/생산-지시등록.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 생산 지시 등록입니다.
##### 생산지시관리는 미지시 계획을 조회하고, 미지시 계획에 대하여 생산을 지시할 수 있는 페이지입니다.
##### 미지시 계획 조회를 클릭하면 미지시 계획 목록이 출력됩니다.
##### 생산계획코드를 클릭하면 생산지시를 생성할 수 있으며, 생산계획에 따른 라인코드가 입력됩니다.
##### 필수 내용을 입력한 후 조회를 클릭하면 해당 라인 공정에 사용되는 필요자재를 조회합니다.
##### 자재코드 클릭시, 공정에 투입할 자재를 선택할 수 있는 자재 LOT 목록을 출력합니다.
##### 등록된 자재를 선택 및 수량 입력 후 생산지시 등록을 하게 되면 확인창이 출력되고 승인을 하면 생산지시 등록이 완료됩니다.

## 1.2.3 생산관리 - 생산
<img src="/images/생산-생산.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 생산관리의 생산입니다.
##### 라인에 맞는 공정을 통해 제품을 생산하는 페이지입니다.
##### 생산지시 목록을 클릭시, 생산 지시 목록을 조회할 수 있습니다.
##### 생산 시작할 생산지시코드를 클릭하면 진행생산지시 목록이 추가되고, 공정 목록에서 공정별 진행상황을 확인할 수 있습니다.
##### 생산시작 클릭 시 첫 순번 공정 상태가 진행 상태로 바뀌며 작업시작시간이 입력되고 실시간으로 생산이 진행됩니다.
##### 순번의 합격량이 일정 수량을 넘으면 다음 순번의 공정이 진행됩니다.
##### (생산시작시 프로시저를 통해 생산이 시작되어지고 , 이전 공정의 합격량이 일정량을 넘기면 다음 공정이 진행됩니다.)


## 1.3.1 원자재 - 발주등록
<img src="/images/자재-발주등록.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 발주등록 페이지 입니다.
##### 생산 지시하지 않은 생산계획서를 통해 생산계획코드를 조회합니다.
##### 체크박스 항목을 클릭후 선택버튼을 클릭시 bom을기반으로 생산계획별 부족한 원자재를 조회할수있습니다.
##### 선택버튼클릭시 부족한원자재를 기반으로 현재고를 파악하여 계획대비 필수량과 발주량을 확인할수있으며 발주신청이 가능합니다.
##### 저장버튼을 누르면 등록 알림창이뜨고, 저장이 완료되는순간 프로시저를 이용하여 원자재 발주코드와 발주상세코드를 자동 생성하도록 구현하였습니다.

## 1.3.2 원자재 - 입고등록
<img src="/images/자재-입고등록.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 입고등록 페이지 입니다.
##### 검수가 끝난 입고예정인 원자재를 입고시키는 페이지입니다.
##### 추가버튼을 클릭시 입고예정인 원자재를 조회하는 모달창을 출력하고 체크 후 선택 시 입고등록페이지에 넘겨줍니다.
##### 입고등록페이지에 추가된원자재는 입고예정목록 모달창에선 조회할수없으며 체크박스를 선택후 삭제버튼을 클릭하면 다시 조회가 가능합니다.
##### 저장버튼을 클릭하면 승인알림창이뜨며, 승인시 프로시저를 통해 입고예정인 원자재를 입고처리할수있으며, 입고예정에서는 삭제됩니다.

## 1.4.1 품질관리 - 검사등록
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

## 1.5.1 설비관리 - 설비 실시간 상태
<img src="/images/설비-실시간.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 설비 실시간 상태 페이지 입니다.
##### 각 라인의 공정들의  온도와 생산량을 실시간으로 볼 수 있도록 구현하였습니다.
##### 설비 실시간 온도에 경우 확인하고 싶은 라인을 클릭하면 선택한 라인의 각 공정 별 온도를 실시간으로 보여줍니다.
##### 설비 실시간 생산량에 경우에도 확인하고 싶은 라인을 클릭할 경우 생산이 시작된  해당 라인의 각 공정들의 생산량을 보여줍니다.

# 소스코드 소개
## 2.1 생산관리 - 생산 진행 

```xml:workerAttendance_mapper.xml

create or replace PROCEDURE "PROC_PROCESS" IS

    v_nextLine  proc_prc.line_turn%TYPE;
    v_nextProc  proc_prc.proc_cd%TYPE;
    v_random    number;

    v_stop number;

    CURSOR cur_proc IS
        SELECT DISTINCT
        prc.proc_prcd,
        prc.proc_cd,
        prc.line_turn,
        prc.proc_qty prc_qty,
        st.proc_qty st_qty,
        err.err_qty ,
        pc.eq_cd,
        st.proc_passqty pass_qty,
        cm.comm_cd 
    --INTO p_PROC_PRCD,p_LINE_TURN,p_TPROC_QTY,p_PROC_QTY,p_CD_NM
    FROM
        proc_prc   prc,
        proc_st    st,
        proc_err   err,
        process    pc,
        comm_code  cm
    WHERE
            st.line_turn = prc.line_turn
        AND st.proc_prcd = prc.proc_prcd
        AND err.line_turn = prc.line_turn
        AND err.proc_prcd = prc.proc_prcd
        AND cm.comm_cd = st.proc_st
        AND pc.proc_cd = prc.proc_cd
    ORDER BY 3;

BEGIN


    --IF THEN
    FOR proc_list IN cur_proc LOOP

            SELECT 
            COUNT(*)
            INTO v_stop
            FROM
                 eq_ina  
            WHERE eq_cd= proc_list.eq_cd AND EQ_INAED IS NULL;

        IF proc_list.comm_cd = 'PLAN01' AND v_stop = 0 THEN 

         -- 일정 갯수 이상이되면 다음 공정 start
            IF proc_list.pass_qty + proc_list.err_qty >= 3 THEN
                SELECT nextLine, nextPrcd
                INTO v_nextLine,v_nextProc
                 FROM(
                         SELECT A.LINE_TURN,
                                A.PROC_PRCD,
                                LEAD(A.line_turn) OVER (ORDER BY A.LINE_TURN) nextLine,
                                LEAD(A.proc_prcd) OVER (ORDER BY A.LINE_TURN) nextPrcd
                         FROM(                    
                                            SELECT st.line_turn,
                                                   ST.PROC_PRCD
                                            FROM PROC_PRC PRC, PROC_ST ST, LINE LI
                                             where   ST.line_turn = PRC.line_turn
                                             and   ST.proc_prcd = PRC.proc_prcd
                                             and   LI.LINE_TURN = PRC.LINE_TURN
                                             and   li.line_cd= ( SELECT LI.LINE_CD
                                                                    FROM PROC_PRC PRC, PROC_ST ST, LINE LI
                                                                         where   ST.line_turn = PRC.line_turn
                                                                         and   ST.proc_prcd = PRC.proc_prcd
                                                                         and   LI.LINE_TURN = PRC.LINE_TURN
                                                                         and   ST.LINE_TURN = proc_list.line_turn
                                                                         and   ST.proc_prcd = proc_list.proc_prcd
                                                                         and   li.proc_cd= proc_list.proc_cd
                                                                    ) 
                                )A
                      )
               WHERE   LINE_TURN = proc_list.line_turn AND proc_prcd = proc_list.proc_prcd;
            END IF;
            --IF proc_list.st_qty = 0 THEN
            IF proc_list.pass_qty + proc_list.err_qty = 0 THEN
            -- 생산량 + 불량량 = 0일경우 작업시간 기입
                UPDATE proc_prc
                SET
                    proc_sttm = systimestamp
                WHERE 
                        line_turn = proc_list.line_turn
                    AND proc_prcd = proc_list.proc_prcd;
            END IF;
            -- IF proc_list.st_qty >= proc_list.prc_qty  THEN
            IF proc_list.pass_qty + proc_list.err_qty >= proc_list.prc_qty  THEN
            --  현재공정 생산 종료(생산량 + 불량량 = 투입량)
                UPDATE proc_st
                SET
                    PROC_QTY = PROC_PASSQTY
                WHERE
                        line_turn = proc_list.line_turn
                    AND proc_prcd = proc_list.proc_prcd;

                UPDATE proc_st
                SET
                    proc_st = 'PLAN02'
                WHERE
                        line_turn = proc_list.line_turn
                    AND proc_prcd = proc_list.proc_prcd;
                -- 현재 공정에 합격량을 다음공정 투입량 변경  
                UPDATE proc_PRC
                SET
                        PROC_QTY = (SELECT PROC_PASSQTY FROM PROC_ST
                                    WHERE line_turn = proc_list.line_turn
                                      AND proc_prcd = proc_list.proc_prcd)
                WHERE
                        line_turn = v_nextLine
                    AND proc_prcd = v_nextProc;                


                -- 종료시간 기입
                UPDATE proc_prc
                SET
                    proc_edtm = systimestamp
                WHERE 
                        line_turn = proc_list.line_turn
                    AND proc_prcd = proc_list.proc_prcd;    

                UPDATE proc_err
                SET
                    err_cd = 'ERRDEBEXP'
                WHERE 
                        line_turn = proc_list.line_turn
                    AND proc_prcd = proc_list.proc_prcd;  


            -- 생산량 증가     
            ELSE

                SELECT TRUNC(DBMS_RANDOM.VALUE(1, 100))
                INTO v_random
                FROM DUAL;

                IF v_random <= 5 THEN 
                    -- 불량량 증가
                    UPDATE proc_err
                    SET
                        err_qty = err_qty + 1
                    WHERE
                            line_turn = proc_list.line_turn
                        AND proc_prcd = proc_list.proc_prcd;

                ELSE
                    -- 합격량 증가
                    UPDATE proc_st
                    SET
                        PROC_PASSQTY = PROC_PASSQTY + 1
                    WHERE
                            line_turn = proc_list.line_turn
                        AND proc_prcd = proc_list.proc_prcd;
                END IF;

                -- 다음 공정 START    
                UPDATE proc_st 
                   SET proc_st = 'PLAN01'
                 WHERE line_turn = v_nextLine AND proc_prcd = v_nextProc AND proc_st = 'PLAN00';


                END IF;


            END IF;

      --  END IF;

    END LOOP;

    COMMIT;
END;
```

## 2.2 원자재 관리 - 발주등록 프로시져

```xml:workerAttendance_mapper.xml

create or replace PROCEDURE "INSERT_PO" (
                                       p_param VARCHAR2,
                                       p_mt_cd VARCHAR2,
                                       p_mt_nm VARCHAR2,
                                       p_vdr_nm VARCHAR2,
                                       p_req_dt VARCHAR2,
                                       P_res_qty NUMBER)
IS
            /* 업체코드 담을 변수 */
            v_vdr_cd VARCHAR2(100);
            /* 담당자 코드 담을 변수 */
            v_mgr_cd NUMBER := 1031;


            /* 발주 코드 담을 변수 */
            v_get_po mt_po.po_cd%type;

            v_result NUMBER;
BEGIN
        /* 1. SELECT = 업체코드*/
        SELECT VDR_CD
        INTO   V_VDR_CD
        FROM   VENDOR
        WHERE  VDR_NM  = p_vdr_nm;

        /* 2. SELECT = 변수 */
        SELECT COUNT(*)
        INTO v_result
        FROM MT_PO
        WHERE po_par = p_param;

         if  v_result = 1 then

                    /* 3. SELECT = 발주코드 */
                    SELECT distinct PO_CD
                    INTO v_get_po
                    FROM MT_PO
                    WHERE po_par = p_param;

            INSERT INTO MT_PODTL VALUES (SEQ_PODTL_CREATER.nextval, v_get_po, p_mt_cd, P_RES_QTY, TO_DATE(P_REQ_DT,'YYYY-MM-DD'));
        ELSE 

            v_get_po := GET_PO;


            INSERT INTO MT_PO VALUES (v_get_po, SYSDATE, V_MGR_CD, p_param);
            INSERT INTO MT_PODTL VALUES (SEQ_PODTL_CREATER.nextval, v_get_po, p_mt_cd, P_RES_QTY, TO_DATE(P_REQ_DT,'YYYY-MM-DD'));
        END IF;



END INSERT_PO;

```

## 2.3 품질 관리 - 검사 결과 등록 

```xml:workerAttendance_mapper.xml
create or replace PROCEDURE "QUAL_MT_INSERT" (
                                                    p_po_cd VARCHAR2                                                    
                                                )
IS
        V_CHK_CD mt_chk_dtl.chk_cd%type;
BEGIN

        --자재품질검사 INSERT
        INSERT INTO MT_CHK (po_cd, chk_mngr, chk_insp)VALUES (p_po_cd, '1051', 'MTRL01');

        FOR i IN (SELECT MT_CD FROM MT_PODTL WHERE PO_CD = p_po_cd)
        LOOP
            V_CHK_CD := GET_CK;
                --자재품질검사상세 INSERT
             INSERT INTO MT_CHK_DTL (CHK_CD, PO_CD, MT_CD ,CHK_DTL_INSP)VALUES (V_CHK_CD, p_po_cd, i.mt_cd, 'MTRL01');

                --자재불량내역 INSERT
             INSERT INTO MT_ERRLIST (CHK_CD, MT_CD)VALUES (V_CHK_CD, i.mt_cd);
        END LOOP;

        COMMIT;



END QUAL_MT_INSERT;
```





#### 감사합니다.

