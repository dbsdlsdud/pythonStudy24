# pythonStudy24
파이썬 ai 기초학습용

MBC아카데미 컴퓨터 교육센터 수원점에서 AI기초 학습으로 파이썬 학습 진행용

https://wikidocs.net/17684

파이썬 버전 3.11.2 설치, 파이참 설치

```
cof = 3
ca = 3
macha = 3
my = 0
coffee = ""
while True:
        print("==========================================")
        print("1.아메리카노 ", cof,"개, ", "2.말차라떼 ",macha,"개, ","3.카라멜마끼아또 ",ca,"개, ","4.취소")
        print("      2500원              2800원                3200원")
        cofnum = int(input("먹을 커피를 골라주세요 : "))
        print("==========================================")
        if cofnum == 1:
            money = int(input("돈을 넣어주세요: "))
            if money == 2500:
                print("아메리카노를 줍니다")
                cof = cof -1
                my = my + money
                if cof == 0:
                    print("아메리카노가 다 떨어졌습니다.")
                    break
            elif money > 2500:
                print("거스름돈 %d를 주고 아메리카노를 줍니다" %(money - 2500))
                cof = cof -1
                nam = money - 2500
                my = my + (money - nam)
                if cof == 0:
                    print("아메리카노가 다 떨어졌습니다.")
                    break
            else:
                print("돈을 다시 돌려주고 커피를 주지 않습니다.")
        elif cofnum == 2:
            money = int(input("돈을 넣어주세요: "))
            if money == 2800:
                print("말차라떼를 줍니다")
                macha = macha -1
                my = my + money
                if macha == 0:
                    print("말차라떼가 다 떨어졌습니다.")
                    break
            elif money > 2800:
                print("거스름돈 %d를 주고 말차라떼를 줍니다" %(money - 2800))
                macha = macha -1
                nam = money - 2800
                my = my + (money - nam)
                if macha == 0:
                    print("말차라떼가 다 떨어졌습니다.")
                    break
            else:
                print("돈을 다시 돌려주고 커피를 주지 않습니다.")
        elif cofnum == 3:
            money = int(input("돈을 넣어주세요: "))
            if money == 3200:
                print("카라멜마끼아또를 줍니다")
                ca = ca -1
                my = my + money
                if ca == 0:
                    print("카라멜마끼아또가 다 떨어졌습니다.")
                    break
            elif money > 3200:
                print("거스름돈 %d를 주고 카라멜마끼아또를 줍니다" %(money - 3200))
                ca = ca -1
                nam = money - 3200
                my = my + (money - nam)
                if ca == 0:
                    print("카라멜마끼아또가 다 떨어졌습니다.")
                    break
            else:
                print("돈을 다시 돌려주고 커피를 주지 않습니다.")
        elif cofnum > 4:
            print("다시 골라주세요.")
        elif cofnum == 4:
            print("커피를 주지 않습니다.")
            break

print("판매총액 : ", my)
```
