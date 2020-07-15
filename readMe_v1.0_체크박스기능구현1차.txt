[형상관리요약]
1. 버전 1.1
2. 날짜 2020.07.15 13:17
3. 내용
  1) HMTL 체크박스 요소 적용완료
  2) CSS 기능구현 완료
   - 체크박스를 대신하는 이미지를 크기와 위치를 변경하여
     체크박스 효과와 동일한 기능을 구현함
  3) 체크박스 display:none; 적용, 
	     left: -10px; 제거,
	     transition: all 2s; 제거

[엔티티즈]

&nbsp;
&gt;
&lt;

[이미지 바꾸기]

        input[type=checkbox].css-checkbox+label {
            display: inline-block;
            padding: 0 0 0 30px;
            height: 20px;
            line-height: 20px;
            background: url(images/bg_checkbox.png);
            background-repeat: no-repeat;
            background-size: 20px 40px;
            vertical-align: middle;
        } -> 체크 안했을때 보일 이미지 요소,위치 설정
        
        input[type=checkbox].css-checkbox:checked+label {
            background-position: 0 -20px;
        } -> 체크 했을때 보일 이미지 위치 설정