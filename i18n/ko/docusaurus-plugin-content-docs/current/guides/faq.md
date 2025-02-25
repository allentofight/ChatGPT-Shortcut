# 자주 묻는 질문

## 왜 힌트가 영어로 되어 있나요?

AiShort 는 ChatGPT 를 사용하는 비영어권 사용자를 위해 만들어진 것입니다. 그러나, 힌트는 모두 영어입니다. 이는 ChatGPT 가 다른 언어보다 영어 이해력이 탁월하기 때문입니다. 중국의 첫 대화형 대형 언어 모델인 MOSS 도 MOSS 의 영어 응답 능력이 중국어보다 뛰어나다고 인정합니다. 따라서 영어 힌트를 사용하는 것이 권장됩니다. (MOSS 는 더 이상 개발되지 않음)

비영어 힌트를 사용하면 괜찮은 결과를 얻을 수 있지만, 같은 비영어 힌트를 다시 입력하면 결과가 크게 달라질 수 있습니다. 왜냐하면 ChatGPT 가 비영어를 이해하는 방식이 항상 다르기 때문입니다. 그래서 생산성 힌트를 입력할 때는 영어 힌트를 사용하여 출력 효과를 보장하는 것이 좋습니다. 또한, 영어 힌트는 대답도 영어로 받을 가능성이 높습니다. 힌트 끝에 `respond in Chinese`를 추가하여 대답을 중국어로 지정할 수 있습니다. 만약 당신의 모국어가 다른 언어라면, "Chinese"를 당신의 모국어로 바꿔주세요.

## 항상 프롬프트를 입력해야 하나요?

API 에서 힌트를 '시스템 프롬프트'로 설정할 수 있습니다. 그러면 이후에는 힌트를 입력할 필요가 없고, ChatGPT 는 시스템 프롬프트에 따라 동작합니다.

웹 버전 ChatGPT 에서는 주 힌트를 바꾸지 않는다면, 따옴표로 후속 응답 내용을 선택하면 됩니다. 이렇게 하면 매번 힌트를 입력할 필요가 없습니다. 만약 응답 내용이 힌트 요구사항에 부합하지 않는다면, 그것은 ChatGPT 가 힌트를 잊어버렸다는 것을 의미합니다. 이 경우, 힌트를 다시 입력하여 그것을 깨워야 합니다. 또한, 각 대화의 링크는 고유하므로, 자주 사용하는 대화를 북마크에 저장하여 나중에 사용할 수 있습니다.

## 입력 방식에 따른 검색 지연

검색 기능은 Docusaurus 의 쇼케이스를 기반으로 하며, PC 단에서의

 입력 방식 포커스 손실 문제가 있습니다. Docusaurus 에 피드백을 제공한 후, 해당 회사는 이 문제를 해결하고 '어차피 중국어를 사용해서는 안 된다. 왜냐하면 쇼케이스는 현지화되지 않았기 때문이다.'라고 말했습니다. 그러나 문제는 계속되었습니다. 그래서 저는 검색 컴포넌트를 모바일 버전과 PC 버전 두 가지로 분류하였습니다. 모바일 검색 로직은 그대로 유지되며, 화면 폭 임계값이 768px 이상인 PC 에서는 `debounce` 함수를 도입하여 입력 방식 문제를 해결하였습니다. 그러나 이로 인해 PC 에서는 두 가지 문제가 발생하였습니다: 첫째, 비영어 입력은 800 밀리초 이내에 완료해야 합니다. 둘째, PC 검색 새로 고침이 즉시에서 800 밀리초 지연으로 변경되었습니다. 더 나은 해결책이 있다면 피드백을 주시기 바랍니다.

## 거짓 정보 출력

ChatGPT 는 매우 강력하긴 하지만, 만능은 아닙니다. 때로는 그것이 거짓 정보를 출력할 수 있습니다. 예를 들어, 수백 개의 정보를 AiShort 에 입력해야 할 때, 저는 ChatGPT 에게 지정된 형식으로 데이터를 변환하도록 했습니다. 그러나 변환 과정에서 몇몇 정보가 ChatGPT 에 의해 잘못 적힌 것을 발견했습니다. 예를 들어, 텍스트에서의 한 태그는 'movie critic'인데, ChatGPT 는 그것을 'film critic'으로 바꿔 버렸습니다. 이것은 텍스트에서는 별 문제가 되지 않지만, 코드에 넣으면 오류가 발생합니다. 따라서, ChatGPT 를 사용할 때는 그것이 출력하는 내용을 반드시 확인해야 합니다.

## 힌트가 도움이 되지 않는다

모든 힌트는 인터넷에서 가져왔으며, 주기적으로 업데이트됩니다. 모든 힌트를 테스트했지만, 실제 효과는 요구사항에 따라 달라질 수 있습니다. 만약 오류를 발견하거나 창의적인 아이디어가 있거나 좋은 힌트가 있다면, [피드백 및 제출](https://github.com/allentofight/ChatGPT-Shortcut/discussions/11)을 환영합니다.

요약을 진행하는 경우, GPT 를 사용

하여 기존의 답변을 다시 수정할 수 있어 답변의 정확도를 향상시킬 수 있습니다. 더불어, 힌트는 일만을 위한 것이 아니라 당신의 사고를 확장하고, 다양한 각도에서 문제를 고려하고, 사람들이 생각할 때 쉽게 놓칠 수 있는 문제를 해결하는데 도움이 될 수 있습니다.
