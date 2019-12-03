# :sparkling_heart: 비쥬얼 프로그래밍 **6팀** :sparkling_heart: 


## :star2: 팀장 : **조재호(20151251)**   
## :two_men_holding_hands: 조원 : **황지환(20151257)**   , **박준호(20150503)** 

**역할분담**
==============
| 이름 | 역할 |
|---|:---:|
| `조재호` | `발표, 코딩` | 
| `황지환` | `주제 선정 및 자료조사` | 
| `박준호` | `자료조사 및 GITHUB 작성` | 

**계획서**
===========

| 날짜 | 내용 | 변경사항 |
|---|:---:|---:|
| `11/25` | `프로젝트에 주제에 대한 자료조사 및 토의` | `없음` |
| `11/26` | `주제변경으로 인한 자료 재조사` | `주제변경` |
| `11/27` | `MP3 주제에 이미지 출력 및 현 시간 추가` | `없음` |
| `12/03` | `프로젝트 점검 및 발표준비 ` | `없음` |
| `12/4~17` | `발표준비 ` | `예정` |


## :exclamation: Project - MP3 Player :exclamation:

![image](https://user-images.githubusercontent.com/54825917/69726315-9fe15280-1163-11ea-8b76-94b373b9143e.png)

## 수정사항
- **타이머 추가** 

- **그림 추가**


#define TIMER_TIME 20<br/>
#define TIMER_PAINT 10<br/>
두개의 정적 변수 추가로 인해 OnTimer 변수 추가<br/>


	switch (nIDEvent)
	{
	case TIMER_TIME:
		cTime = CTime::GetCurrentTime();
		mDay.Format(L"%04d.%02d.%02d", cTime.GetYear(), cTime.GetMonth(), cTime.GetDay());
		mTime.Format(L"%02d:%02d:%02d", cTime.GetHour(), cTime.GetMinute(), cTime.GetSecond());

		SetDlgItemText(IDC_STATIC1, mDay);
		SetDlgItemText(IDC_STATIC2, mTime);
		break;

	case TIMER_PAINT:
		if (i == 0) {
		pWnd = (CWnd*)GetDlgItem(IDC_PIC);
		dc = pWnd->GetDC();
		staticSize = (CStatic*)GetDlgItem(IDC_PIC);
		staticSize->GetClientRect(rect);
		i++;
		}
		switch(i)
			case 1:
				m_Img.Load(_T("1.jpg"));
				m_Img.Draw(dc->m_hDC, 0, 0, m_Img.GetWidth(), m_Img.GetHeight());
				i++;
				break;

			
	
		}
		break;
	}



:mega:**소감** :mega:
 - **조재호(20151251)** :  이번에 팀과제를 진행하면서 MFC 프로그램을 찾는 도중에 MFC로 정말로 많은 프로그램을 만들 수 있다는 것을 알았습니다.
                     또한 프로그램을 수정하면서 코딩실력이 매우 향상되었음을 느꼈습니다.
                     정말 좋은 팀과제를 내 주신 교수님께 감사드립니다 교수님 사랑합니다.:heart_eyes_cat:
 - **황지환(20151257)** : 가볍게 생각하고 준비했었던 mfc팀과제였었는데, mfc에 조금은 알고 있다고 생각하였으나,
                     구글링을 통한 예제들을 살펴보고 따라 해본결과 mfc에 대해 더욱 열심히 해야 된다는 생각이 들었습니다.
                     하지만 많은 mfc 예제들을 살펴보았고,
                     그것을 저희가 수업시간에 배웠던 mfc 기술들을 추가하기 위해 노력하면서 많이 배웠고 의미있는 시간이었습니다.
                     MFC 사랑합니다.:two_hearts:
 - **박준호(20150503)** : MFC 과제를 하는데 팀원들과 토의 결과 미리미리 일찍해놓는게 좋을 것 같아 이렇게 빨리 하였습니다. 
                     최종과제를 하며 오픈소스코드에 저희가 배운내용 및 등을 추가하는데 쉽게 생각하였으나 많은 어려움에 부딪혔습니다.
                     하지만 조재호 팀장이 열심히 저희 조원들을 이끌어 주며 협업을 하였는데 그 덕에 중간에 다음에 다시하자 라는 생각보다는
                     지금 다시 하는 생각을 가지며 열심히 하여서 만들었습니다.
                     그래서 협동심이 부쩍 성장하는 느낌이였습니다.
                     MFC 사랑합니다.:gift_heart:
