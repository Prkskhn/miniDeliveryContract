

#    Mini Delivery Contract


## 프로젝트 소개
`🔎 REMIX IDE에서 진행할 수 있는 배달 프로젝트입니다.`
>📱 혼자서 가게, 배달원, 고객으로 배달 프로세스를 경험해볼 수 있습니다!
<br>

## 구현 목표
>컨트랙트로 입금하기
>함수를 실행하여 컨트랙트의 돈을 전송하기
> 필요한 구조체를 선언 및 활용
> require, modifier를 사용하여 함수 실행 조건 설정하기
> storage 활용하여 상태변수 변경하기

<br>


## 📚 실행 가이드 및 설치 방법(How to build)
### 설치/실행 방법
<summary>0.  준비 사항</summary>

`❗️❗️코드를 복사하여 REMIX IDE에서 간편하게 시험하실 수 있습니다.`
`❗️❗️REMIX IDE의 COMPLIER 탭에서 Enable optimization를 선택해주세요!`
`❗️❗️가상환경에서 1번,2번,3번 계정은 각 가게,고객,라이더로 진행합니다`
`❗️❗️주문 구조체의 마지막에 가게와 배달원의 상태가 있다는 점을 참고해주세요!`

<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/1edba613-270b-4f92-b461-6a4a3a61874f" width="" height="300"><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/427c6242-1920-4e6b-8996-86463ca9f624" width="" height="300">
`❗️❗️DEPLOY & RUN TRANSACTIONS 탭에서 배포후 시작합니다!`



<summary>1.  [가게] 계정 등록하기</summary>
<div markdown="1">

<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/60526f60-51a7-4d57-aa27-9e13c6be832c" width="" height="">

```
가게를 입점하며 가게명, 지역을 입력해줍니다.
```

</div>



<summary>2. [가게] 메뉴 등록하기</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/de23eecc-68db-4a7c-9c25-785177cbd94c" width="" height="">

```
가게에 등록할 음식명, 음식의 가격을 등록해줍니다.
```

</div>



<summary>3. [고객] 계정 등록하기</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/3b7dc1b4-d2e0-4303-9aac-807bc5758808" width="" height="">

```
고객 회원가입을 하며 닉네임과 지역을 입력해줍니다.
```

</div>



<summary>4.  [고객] 장바구니 담기.</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/62f6bd9f-676b-4455-aee4-ecc533e3af58" width="" height="">


```
주문을 원하는 가게명, 음식명,수량을 입력하여 장바구니에 담아줍니다.
```

</div>



<summary>5.  [고객] 주문하기.</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/e3a9958b-0cbb-486d-8c3d-c640d37f3060" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/ddb13d0a-9f35-44d6-a4eb-cab265037fa6" width="50%" height="">

```
배달팁(선택)여부에 맞게 가격을 넣어주시고(ether단위), 주문상태 변경을 확인할 수 있습니다.(마지막 두 숫자 4(notyetChoice),0(notSelected))
```
</div>
<summary>6.  [가게] 주문 수락/거절하기.</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/2814e3ba-babf-4097-a716-19c3279de743" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/7cf65ee8-ed0a-4494-abaf-8ab80d1bd23a" width="50%" height="">

```
가게에 들어온 첫 주문을 수락/거절합니다.주문상태 변경을 확인할 수 있습니다.(마지막 두 숫자 1(accept),0(notSelected))
```
</div>
<summary>7.  [라이더] 계정 등록하기.</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/f73b5d3b-015b-465d-a5c7-ed113e580693" width="50%" height="">

```
라이더 회원가입을 진행합니다. 배달방식,배달지역을 입력합니다.
```
</div>
<summary>8.  [라이더] 배달건 선택하기.</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/02e4ec52-ddcc-45f8-a5e0-0769051c8b08" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/86426eb4-5785-4813-990e-aef7c01a2b3e" width="50%" height="">

```
배달할 주문건을 선택합니다. 1번 주문을 입력합니다.주문상태 변경을 확인할 수 있습니다.(마지막 두 숫자 1(accept),2(isPicked))
```
</div>
<summary>9.  [고객] 주문 가격 지불하기.</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/8e0a0cff-bc2d-45b6-9b2d-4a3e230a8c72" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/db115577-7537-408b-b1bc-467964b18b76" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/8ec1b70e-bbac-4266-8c9c-8bf5f671687e" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/a475b495-aa8b-4dc8-aa55-4d79df50b88d" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/5379fc15-0a23-4d4a-9684-df62f1f223dc" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/fc01259f-6fcf-4bca-a10d-dce90a191ee0" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/e9816cb7-bd79-4bdc-8f61-be8624d61dc0" width="50%" height="">


```
치킨가격(1),배달비(0),배달팁(0)으로 총 지불비는 1입니다. msg.value에 1 ETHER를 입력하시고 payment를 진행합니다. 컨트랙트에 돈이 보내지고 잔액의 변화를 확인할 수 있습니다.주문상태 변경도 확인할 수 있습니다.(마지막 두 숫자 5(checkMoney),4(checkMoney))
```
</div>
<summary>10.  [가게] 조리 완료하기.</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/66651a50-5aa6-4cf1-9624-dc37faddae9f" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/f06cc89f-9d7b-43e1-bc3b-696310652dab" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/fc01259f-6fcf-4bca-a10d-dce90a191ee0" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/dd5e9020-fb90-469b-b86c-1fdac121c2ed" width="50%" height="">

```
조리를 완료합니다. 1번 주문을 입력하여 조리완료 함수를 실행합니다.가게는 고객이 지불한 배달비와 동일한 배달비를 msg.value에 입력해야합니다. 고객이 지불한 배달비는 현재 0이므로 msg.value 입력 없이 진행합니다.또한 컨트랙트에 고객이 보낸 음식값을 수령하여 잔액의 변화를 확인할 수 있습니다. 주문상태 변경도 확인할 수 있습니다.(마지막 두 숫자 2(cookFinish),4(checkMoney))
```
</div>
<summary>11.  [라이더] 배달 시작하기.</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/e20d15b3-3c28-46b5-ab93-f20365845742" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/7fe28b29-4f0e-4c42-99ad-6c9f3231fe16" width="50%" height="">

```
1번 주문에 대한 배달을 시작합니다.주문상태 변경도 확인할 수 있습니다.(마지막 두 숫자 2(cookFinish),1(inDelivery))
```
</div>
<summary>12.  [라이더] 배달 완료하기.</summary>
<div markdown="1">
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/39e15645-153a-490d-b585-b004b209df83" width="50%" height=""><img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/d78c1b53-3226-499e-b149-d641fda6d7be" width="50%" height="">

```
배달 완료할 주문번호1번을 입력합니다. 배달 주문건의 상태도 확인할 수 있습니다.(마지막 두 숫자 3(isPicked),3(deliveryComplete))
```
</div>


<br>




## 활용기술

#### Language 
<img src="https://github.com/Prkskhn/BaeBlock/assets/104644024/af410c99-2486-4a06-baa2-536f74fc40cd" width="30"/> 

#### IDE

<img src="https://github.com/Prkskhn/BaeBlock/assets/104644024/28f6e6eb-aa41-48bf-9194-e9945310e7ed" width="30"/>
<img src="https://github.com/Prkskhn/miniDeliveryContract/assets/104644024/72cb741e-7357-40cd-bb8b-d6b9eb5f5c77" width="30"/> <br/>



