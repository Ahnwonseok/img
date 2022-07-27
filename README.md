### 설명<br/>
사람이름(*숫자) : {'키값' : 거리계산값} *통과율 <br/>
*숫자 : 몇번째 사진이 now_face인지<br/>
*통과율 : 예를 들어 2/3이면 3개의 사진 중에 2개의 사진만 거리값이 0.4 미만<br/>
※표시는 인물의 사진 설명<br/>

### 인물들<br/>
권xx(1) : {'Axx43tg2d': 0.384, 'pxx43uA3o': 0.2} 1/2<br/><br/>

기xx(1) : {'wxx41J4S': 0.428, 'pxx41X6x': 0.384, 'uxx41z5S': 0.388} 2/3<br/>
※찡그린 사진->얼굴인식 잘 못함, 흑백사진->얼굴 디텍션 잘 못함<br/>

김미승(1):  {'icd52Qk6g': 0.563, 'PeC52SQ3vGHD': 0.499, 'Rbw52HZ5l': 0.415, 'dnE52mi2U': 0.284, 'dqL52PJ4C': 0.366} 2/5<br/>
※얼굴 45도 측면 사진이 다를 확률이 높다, 위로 45도 다르다고 인식할 확률이 높다.<br/>

김상욱(4) : {'BtL55f2E': 0.461, 'mPD55h3F': 0.384, 'XFf55I1D': 0.408} 1/3<br/>
※여러 명이 나온 사진에 다른 사람 얼굴을 탐지, 화질이 안 좋으면 얼굴인식이 어렵다<br/>

박xx(6) :  {'Bxx50EM5d': 0.446, 'Jxx50aL4A': 0.385, 'jxx50KI2A': 0.368, 'Oxx50uT1J': 0.503, 'Xxx50SA3s': 0.395} 3/5<br/>
※흐린사진, 측면 45도 사진 인식 못함<br/>

박가수(1) : {'aIR50Fr4Y': 0.29, 'lnE50WQ2w': 0.378, 'ZCY50wD3A': 0.306} 3/3<br/>

박배우(3) : {'Awl40q4q': 0.346, 'dHu40V5t': 0.28, 'SOl40j2K': 0.382} 3/4<br/>
※흐린사진 한 장은 얼굴인식을 아예 못함 / now_face의 임베딩 값을 얻지 못할 경우 예외처리<br/>

브레드(4) : {'eEE40u3VFVA': 0.558, 'nRp40I5uLDZLzQ': 0.456, 'PUz40o1PWfu': 0.571} 0/3 <br/>
※흐린사진 얼굴 탐지 못함, 측면/흑백사진 얼굴인식률 떨어짐<br/>

옥xx(1) : {'exx42hY3E': 0.373, 'hxx42Fg4C': 0.406, 'qxx42bM2e': 0.403, 'uxx42SZ5s': 0.383} 2/4 <br/>
※눈,코,입이 정확히 나와야 얼굴인식률 높아짐 / 비슷한 각도 사진들의 얼굴인식률이 높다<br/>

이경오(1) : {'Iys57q6L': 0.307, 'nMg57X5M': 0.356, 'peK57L4A': 0.413, 'PRM57i2i': 0.306, 'zeG57e3r': 0.366} 4/5<br/>
※눈을 아래로 뜬 사진은 얼굴이 다르다고 나왔다.<br/>

전은경(1) : {'Lfh44qV5n': 0.329, 'nrq44Dt2S': 0.229} 2/4<br/>
※눈 감은 사진 얼굴 탐지 못함, 옆 모습 얼굴 탐지는 하지만 얼굴인식은 못함<br/>

정민교(2) : {'kMH40Q6N': 0.445, 'oac40o4T': 0.517, 'PDX40O3O': 0.524, 'sHQ40R1w': 0.459} 0/5<br/>
※ 작은 얼굴은 탐지 못함<br/>

차영미(1) : {'Lpa50ks4N': 0.331, 'PlO50HP2V': 0.429, 'Xzd50yA5G': 0.349} 2/4<br/>
※ 옆모습은 얼굴탐지는 하나 얼굴인식은 불가, 보정 많이하면 얼굴인식률 떨어짐<br/>

### 총평<br/>
옆이나 위아래로 각도를 튼 사진, 보정을 많이 한 사진, 어두운 사진은 얼굴인식을 잘 하지 못하고 하더라도 다르다고 나온다.<br/>
