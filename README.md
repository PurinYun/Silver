


지난 1월, Facebook CEO 마크 저커버그(Mark Zuckerberg)가 <아이언맨>에 등장하는 ‘자비스’와 같은 AI 비서 개발에 도전하겠다는 개
인적인 새해 목표를 밝힌 것을 기억하시나요?

저커버그가 1년간의 도전의 결과물인 자비스를 모두에게 소개했습니다.

먼저, 저커버그가 자신의 Facebook 프로필(https://www.facebook.com/zuck)에 업로드한 동영상으로 자비스를 만나 볼까요?




저커버그는 자비스 구축 과정에서 배우고 느낀 점을 글로 전하기도 했는데요, 아래에서 간략한 내용을 만나 보실 수 있습니다.

자비스는 어떻게 개발됐는지, 무엇을 할 수 있는지, 그리고 AI에 대해 저커버그는 어떤 생각을 하고 있는지 살펴 보세요. 원문은 해>당 링크(https://www.facebook.com/notes/mark-zuckerberg/building-jarvis/10154361492931634)에서 확인하실 수 있습니다.

‘자비스(Jarvis)’ 구축하기

2016년 한 해 동안 저는 개인적인 프로젝트를 하나 진행했습니다. 바로 <아이언맨>에 등장하는 ‘자비스’처럼 집안일을 도와 주는 간>단한 인공지능(AI)을 구축하는 일인데요.

프로젝트 기간 동안, AI의 놀라운 발전을 직접 경험하는 동시에 아직 갈 길이 멀다는 것 역시 깨달을 수 있었습니다.

‘자비스’는 스마트폰과 컴퓨터를 매개체로 사람의 말을 이해하고 조명∙온도∙가전∙음악∙보안 등 각종 집안 시설을 제어할 수 있습니다
. 또한 자비스는 사람의 취향과 습관을 학습할 수 있으며 새로운 단어와 개념을 학습하고, 심지어 아이와 놀아줄 줄도 아는 똑똑한 AI입니다. 자비스 개발에는 자연어 처리, 음성 인식, 얼굴 인식, 강화 학습처럼 다양한 AI 기술과 파이썬, PHP, 오브젝티브-C 등 다양
한 프로그래밍 언어가 사용됐습니다.

지금부터 여러분께 자비스를 소개합니다. 그리고 이 프로젝트를 진행하면서 제가 배우고 느낀 점에 대해 말씀드리겠습니다.
시작은 집안을 연결하는 것부터 

집안에 있는 시스템을 서로 연결하는 것은 생각보다 복잡했습니다. 시스템들이 각기 다른 프로그래밍 언어와 프로토콜로 이뤄져 있었고, 대부분의 가전제품은 인터넷에 연결조차 돼 있지 않았기 때문입니다.

자비스와 같은 AI 도우미들이 미래에 보


지금부터 여러분께 자비스를 소개합니다. 그리고 이 프로젝트를 진행하면서 제가 배우고 느낀 점에 대해 말씀드리겠습니다.
시작은 집안을 연결하는 것부터

집안에 있는 시스템을 서로 연결하는 것은 생각보다 복잡했습니다. 시스템들이 각기 다른 프로그래밍 언어와 프로토콜로 이뤄져 있었고, 대부분의 가전제품은 인터넷에 연결조차 돼 있지 않았기 때문입니다.

자비스와 같은 AI 도우미들이 미래에 보다 널리 사용되기 위해서는 더 많은 기기를 서로 연결할 수 있는 공통 API와 같은 표준이 필요하다는 것을 알 수 있었습니다.

자연어

다음 단계는 집안 시스템들이 사람의 말을 알아들을 수 있도록 하는 일이었습니다. 우선, 자비스와 사람이 문자로 소통할 수 있는 체계를 만들기로 했습니다. 그 다음, 사람의 목소리를 문자로 변환하고, 자비스가 저에게 하고 싶은 말을 소리로 전달할 수 있는 능력을 추가했습니다.

처음에는 ‘침실’, ‘전등’, ‘스위치 켜줘’와 같은 기본적인 키워드로 시작했습니다. 이 과정에서 자비스에게 ‘화장실’이나 ‘욕실’과 같은 유의어를 학습시킬 필요가 있다는 것을 자연스럽게 터득할 수 있었습니다. AI에게 맥락을 이해시키는 일의 중요성도 깨달았습니다. AI가 사람이 전하고자 하는 맥락을 정확히 이해해야 보다 어려운 열린 질문에도 능숙하게 대처할 수 있기 때문입니다.

비전인식과 얼굴인식

AI가 이미지와 동영상에 담긴 정보를 이해하는 과정에는 추적, 사물 인식, 얼굴 인식 등이 매우 중요합니다. 시각 정보를 이해하는 AI 시스템의 활용 가능성은 무궁무진합니다. 일례로, 아기가 낮잠에서 깬 것을 알아채고 음악을 틀어줄 수도 있고, “불 좀 켜줘”라는 명령을 듣고 사람이 어느 방에 있는지 파악해 방의 전등을 켜는 일 등을 들 수 있습니다.


메신저 봇

자비스는 컴퓨터를 기반으로 구축된 AI이지만, 시간과 장소에 대한 제약 없이 자유롭게 대화를 주고받기 위해서는 스마트폰을 활용할 필요가 있었습니다. 이를 위해 Facebook 메신저 봇을 사용했고요. Facebook 메신저 플랫폼이 제공하는 봇 프레임워크를 활용하면 별도의 앱을 구축하는 것보다 훨씬 적은 시간과 노력으로도 목적에 부합하는 메신저 봇을 개발할 수 있기 때문입니다.

이를 통해, 언제 어디서든 자비스와 대화를 주고받을 수 있게 됐습니다. 스마트폰을 통해 자비스 봇에게 메시지를 보내면, 메시지는 즉각 자비스 서버로 전송됩니다. 자비스 봇에게 음성 메시지를 보
# Silver
# 저도 이에 대해 전적으로 동의 합니다. 
준연 작성
==========
