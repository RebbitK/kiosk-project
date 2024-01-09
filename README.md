# KIOSK-PROJECT
## 과제 소개

````
📢 내가 좋아하는 카페 또는 패스트푸드점의 키오스크를 만들어보자!

    지금까지 배워온 Java 언어를 사용하여 키오스크 프로그램을 만들어봅시다.
    내가 좋아하는 카페나 패스트푸드점의 메뉴판 데이터를 사용하면 더 재밌겠죠?
````
<figure>
    <img src="https://file.notion.so/f/f/83c75a39-3aba-4ba4-a792-7aefe4b07895/8ca4da3d-2338-41ec-ba10-84feae77273b/Untitled.png?id=d9bf83cd-5db6-44a4-9bc8-cef8fbfdb603&table=block&spaceId=83c75a39-3aba-4ba4-a792-7aefe4b07895&expirationTimestamp=1704873600000&signature=5fpPZTrGA83NrffRNQ8gyAd2MXyRrk9RfXV_7iKdNxU&downloadName=Untitled.png">
</figure>

1. 메뉴판을 보고 주문할 수 있는 Java 프로그램
2. 화면은 `System.out.println()` 메소드를 사용해서 심플하게 출력한다.
3. `메뉴 클래스`와 `주문 클래스`를 사용하여 Java 의 핵심 기능인 **상속**을 최대한 사용
4. 내가 좋아하는 메뉴들로 다양하게 구성해보세요!

## ☕ 과제 요구사항 및 출력 예시

---

- 필수 요구사항
    
    > **Java 클래스 설계 시 필수 요구사항!**
    > 
    > - 메뉴 클래스는 이름, 설명 필드를 가지는 클래스로 만들어주세요.
    > - 상품 클래스는 이름, 가격, 설명 필드를 가지는 클래스로 만들어주세요.
    > - 상품 클래스의 이름, 설명 필드는 메뉴 클래스를 상속받아 사용하는 구조로 개발해주세요.
    > - 주문 클래스도 만들어서 상품 객체를 담을 수 있도록 해주세요.

**1. 메인 메뉴판 화면**
   - 메인 메뉴판이 출력되며 메뉴판에는 상품 메뉴가 출력 됩니다.
   -  상품 메뉴는 간단한 설명과 함께 출력 되며 최소 3개 이상 출력 됩니다.
   - 상품 메뉴 아래에는 Order(주문)와 Cancel(주문 취소) 옵션을 출력해줍니다.
 ````
맥도날드에 오신것을 환영합니다.
아래 메뉴판을 보시고 메뉴를 골라 입력해주세요.
[ McDonald's MENU ]
1. Burgers                   | 주문 즉시 바로 조리해 더욱 맛있는, 맥도날드의 다양한 버거 
2. Dessert                   | 가볍게 즐길 수 있는 디저트 메뉴! 
3. Side                      | 버거와 함께 푸짐하게 즐기는 사이드 메뉴 
4. Drink                     | 언제나 즐겁게, 다양한 음료를 부담없이 즐기세요! 

[ ORDER MENU ]
5. Order                     | 장바구니를 확인 후 주문합니다. 
6. Cancel                    | 진행중인 주문을 취소합니다.
````
**2. 상품 메뉴판 화면**
    - 상품 메뉴 선택 시 해당 카테고리의 메뉴판이 출력됩니다.
    - 메뉴판에는 각 메뉴의 이름과 가격과 간단한 설명이 표시됩니다.
````
맥도날드에 오신것을 환영합니다.
아래에 상품메뉴판을 보시고 상품을 골라 입력해주세요.
1. Big Mac                        | W5.5 | 맥도날드 하면 가장 먼저 떠올리게 되는 대표적인 제품 
2. McCrispy Shanghai Burger       | W5.5 | 겉은 바삭, 속은 부드러운 치킨 패티의 매콤함으로 입맛도 기분도 화끈하게! 
3. 1955 Burger                    | W5.5 | 1955년 당시의 맛을 다시한번 재탄생! 
4. Quarter Pounder Cheese         | W5.5 | 세계적으로 사랑받고 있는 맥도날드의 대표적인 프리미엄 버거 
5. Bulgogi Burger                 | W3.1 | 한국인의 입맛에 딱 맞는 불고기 소스에 잘 재운 패티의 조합!
````
**3. 구매 화면**
    - 상품 선택 시 해당 상품을 장바구니에 추가할지 확인하는 문구가 출력 됩니다.
    - `1.확인` 입력 시 장바구니에 추가되었다는 안내 문구와 함께 메인 메뉴로 다시 출력 됩니다.
````
Big Mac                        | W5.5 | 맥도날드 하면 가장 먼저 떠올리게 되는 대표적인 제품 
위 메뉴를 장바구니에 추가하시겠습니까?
1. 확인          2. 취소
1
Big Mac가 장바구니에 추가되었습니다.
````
**4. 주문 화면**
    - `5.Order` 입력 시 장바구니 목록을 출력해줍니다.
    - 장바구니에서는 추가된 메뉴들과 총 가격의 합을 출력해줍니다.
    - `1.주문` 입력 시 주문완료 화면으로 넘어가고, `2.메뉴판` 입력 시 다시 메인 메뉴로 돌아옵니다.
````
[ Orders ]
 Big Mac                        | W5.5 | 1개 | 맥도날드 하면 가장 먼저 떠올리게 되는 대표적인 제품 

[ Total ] 
 W5.5

1. 주문            2. 메뉴판
````
**5. 주문완료 화면**
    - `1.주문` 입력 시 대기번호를 발급해줍니다.
    - 장바구니는 초기화되고 3초 후에 메인 메뉴판으로 돌아갑니다.
````
주문이 완료되었습니다! 

대기번호는 [ 1 ] 번 입니다.
(3초후 메뉴판으로 돌아갑니다.)
````
**6. 주문 취소 화면**
    - 메뉴판에서 `6.Cancel` 입력시 주문을 취소할지 확인을 요청하는 문구가 출력 됩니다.
    - `1.확인` 을 입력하면 장바구니는 초기화되고 취소 완료 문구와 함께 메뉴판이 출력 됩니다.
````
진행하던 주문을 취소하시겠습니까?
1.확인          2.취소
1
주문이 취소되었습니다.
````
💡 선택 요구사항  
**1. 주문 개수 기능 추가**
   - 장바구니에 똑같은 상품이 담기면 주문 화면에서 상품 개수가 출력 되도록 합니다.
````
아래와 같이 주문 하시겠습니까? 

[ Orders ]
 Taro Pie                       | W1.8 | 2개 | 달콤한 보랏빛 디저트! 
 Tomato Chicken Snack Wrap      | W3.0 | 2개 | 상큼한 토마토와 바삭한 치킨의 조합! 

[ Total ] 
 W9.6

1. 주문            2. 메뉴판
````
**2. 상품 옵션 기능 추가**
    - 상품에 옵션을 선택 후 장바구니에 추가 할 수 있게 세분화 합니다.
````
 Big Mac                        | W5.5 | 맥도날드 하면 가장 먼저 떠올리게 되는 대표적인 제품 
위 메뉴의 어떤 옵션으로 추가하시겠습니까?
1. single( W 5.5 )        2. Set( W 6.9 )
````
````
 Big Mac set                    | W6.9 | 맥도날드 하면 가장 먼저 떠올리게 되는 대표적인 제품 
위 메뉴를 장바구니에 추가하시겠습니까?
1. 확인          2. 취소
````
**3. 총 판매금액 조회 기능 추가**
    - 구매가 완료될 때마다 총 판매 금액을 누적해줍니다.
    - 숨겨진 기능으로 0번 입력 시 총 판매금액을 출력합니다.
````
[ 총 판매금액 현황 ] 
 현재까지 총 판매된 금액은 [ W 15.1 ] 입니다.
1. 돌아가기
````
**4. 총 판매상품 목록 조회 기능 추가**
    - 구매가 완료될 때마다 판매 상품 목록을 저장해줍니다.
    - 숨겨진 기능으로 0번 입력 시 총 판매 상품 목록을 출력합니다.
````
[ 총 판매상품 목록 현황 ] 
현재까지 총 판매된 상품 목록은 아래와 같습니다.

- Big Mac                  | W 5.5
- Taro Pie                 | W 1.8
- Taro Pie                 | W 1.8
- Tomato Chicken Snack Wrap| W 3.0
- Tomato Chicken Snack Wrap| W 3.0
````
## 회고
이번 개인프로젝트인 키오스크만들기에서 가장 고민을 많이 했었던 부분은 주문 개수 기능 추가와 상품 옵션 기능 추가였습니다.  
처음에는 단순하게 하나의 상품 객체에서세트 주문이 들어오면 가격 필드만 변경하는 식으로 진행하였는데 이 부분에서 결국 상품 객체의 
주소는 변하지 않았기 때문에 같은 객체로 인식하여 주문 개수를 카운트 할 때 오류가 발생하였습니다.  
나는 이 부분을 새로운 리스트를 만들어 그 리스트에 세트가 포함된 메뉴의 리스트를 가져와 그 리스트에서 가격 필드만 수정하는 식으로 해결하였습니다.  
팀원들간의 코드리뷰를 거치면서 위의 방법 외에도 상품 생성자를 나누어 단품 상품 생성자와 세트 상품 생성자로 단품일 경우와 세트일 경우의 객체가 다르게 생성되게하여 해결하는 방법또한 배울 수 있었고,  
또한 팀원분들의 피드백을 바탕으로 메인스크린 메서드에서 발생하는 이벤트들을 전부 메서드로 묶어 가독성을 올리고 외부에서 접근하는 것을 막기위해 접근제어자를 지정하는 식으로 코드를 더욱 발전시킬 수 있었습니다.
