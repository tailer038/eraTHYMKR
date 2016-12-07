- 첫경험 표시 패치 설명서

CFLAG:500 = 캐릭터 번호 +1 (초기치가 0이기 때문에 '주인'을 판별하기 위해서 굳이 +1로 함)
CSTR:5 = 처녀를 빼앗은 캐릭터의 이름

기본은 처녀 상실 때 VIRGIN_ROAD.ERB에 들어있는 함수를 참조해서, 각 캐릭터의 CFLAG:500 및 CSTR:5를 변경하여 처녀를 빼앗은 대상을 판별합니다. 판별 대상은 각 캐릭터와 도구(바이브, 로터, 손가락, 딜도 등), 촉수, 동물 등등입니다. 3P나 윤간은 [불명]으로 처리됩니다.

조수를 범한다, 역강간, 조수를 범하게 한다 등의 커맨드는 조교자→노예 관계가 아니라 주인→조수, 노예→조수 관계로 처녀 상실 처리가 이루어지므로 부득이하게 COMF_ALL.ERB을 수정했습니다.

또 약방의 노란 사탕 먹고 처녀 상실이 이루어지거나, 밤 이벤트에서 처녀 상실이 이루어지거나, 멋진 식후의 운동으로 처녀 상실이 이루어질 때는 각각 해당 파일에서 독자적으로 처리하고 있으니 착오 없기를.

무명 캐릭터의 경우는 구매시에 첫경험 여부를 판별합니다.


□수정한 파일 목록

EVENT_NIGHT1.ERB
EVENT_SELF.ERB
INFO0.ERB
RANDOM_STATE.ERB
SHOP_DRUGUSE1.ERB
SHOP_LUNCH0.ERB
SOURCE0.ERB
SYSTEM_DEBUG.ERB
SYSTEM_TENTACLE.ERB
VIRGIN_ROAD.ERB

COMF_ALL.ERB