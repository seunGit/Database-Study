### 출처
- [solvesql](https://solvesql.com/problems/restaurant-vip/)

### 문제

**난이도: 쉬움, 주제: GROUP BY, 제출 횟수: 549번, 정답 횟수: 296번, 정답률: 53.92%, 출제자: [데이터리안] 선미**

`tips` 테이블에는 식사 금액, 팁, 결제자 성별, 요일, 시간대 등 어느 레스토랑의 테이블 당 결제에 관련된 데이터가 들어있습니다. 요일별로 가장 높은 금액의 결제 내역을 출력하는 쿼리를 작성해주세요. 쿼리 결과에는 `tips` 테이블에 있는 모든 컬럼이 포함되어야 합니다.

### 풀이
<br>

**재석**

```sql

```   

**승기**
- `max()` : 최대값 출력
- 모든 컬럼(`*`), 요일별 출력(`group by`), 가장 높은 금액(`max()`)
- 위 세가지 항목을 충족시키면 된다.
```sql
select * from tips
group by day
order by max(total_bill) desc
```

**연수**

```sql
SELECT * FROM tips
GROUP BY day
ORDER BY max(total_bill) desc
```

**형준**
```sql

```
