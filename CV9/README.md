# AIFFEL Campus Online 5th Code Peer Review Templete
- 코더 : 서희원
- 리뷰어 : 조대호	


# PRT(PeerReviewTemplate) 
각 항목을 스스로 확인하고 토의하여 작성한 코드에 적용합니다.

- [O] 코드가 정상적으로 동작하고 주어진 문제를 해결했나요?
  >네 코드가 정상적으로 작동하고 문제에 대해 해결했습니다.
- [O] 주석을 보고 작성자의 코드가 이해되었나요?
  > 네 주석을 보고 코드를 이해하는데 도움이 되었습니다.
- [O] 코드가 에러를 유발할 가능성이 없나요?
  > 네 에러가 발생하지 않았습니다.
- [O] 코드 작성자가 코드를 제대로 이해하고 작성했나요?
  > 네 작성한 코드를 보면서 궁금했던 부분에 대한 질문에 대해 답변을 잘 해주셨습니다.
- [O] 코드가 간결한가요?
  > 네 함수를 만들어 반복되는 부분을 처리했습니다.

# 예시
1. 코드의 작동 방식을 주석으로 기록합니다.
2. 코드의 작동 방식에 대한 개선 방법을 주석으로 기록합니다.
3. 참고한 링크 및 ChatGPT 프롬프트 명령어가 있다면 주석으로 남겨주세요.
```python
# 사칙 연산 계산기
class calculator:
    # 예) init의 역할과 각 매서드의 의미를 서술
    def __init__(self, first, second):
        self.first = first
        self.second = second
    
    # 예) 덧셈과 연산 작동 방식에 대한 서술
    def add(self):
        result = self.first + self.second
        return result

a = float(input('첫번째 값을 입력하세요.')) 
b = float(input('두번째 값을 입력하세요.')) 
c = calculator(a, b)
print('덧셈', c.add()) 
```

# 참고 링크 및 코드 개선
```python
image = cv2.drawContours(image, [rect_cam], 0, (0,255,0), 2)
image = cv2.drawContours(image, [rect_grad_cam], 0, (255,0,0), 2)

plt.imshow(image)
plt.show()

res1= cam(cam_model, item)
res2 = grad_cam(cam_model, item)
print("labelnumber: ",item['label'])
print("model1: {:.3f}    model2: {:.3f}".format(res1, res2))
```
gradcam과 cam으로 만든 바운딩박스의 이미지 비교와 iou 값 비교를 해주셨으면 좀 더 두 방식의 차이를 알기 쉬웠을것 같습니다.
