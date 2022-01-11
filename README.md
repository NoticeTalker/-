<html>
<head>
<title>알림토커</title>
<script id="javascript-sdk" src="https://developers.kakao.com/sdk/js/kakao.min.js"></script>
</head>
<body>
<p><strong>아래 카카오톡 아이콘을 눌러 전송하세요</strong> By. 알림토커</p>
<a id="kakao-link-btn" href="javascript:sendLink()">
  <img
    src="https://developers.kakao.com/assets/img/about/logos/kakaolink/kakaolink_btn_medium.png"
  />
</a>
<script type="text/javascript">
 Kakao.init('c036519ab68884be2d54ec47d14736ab');
  function sendLink() {
    Kakao.Link.sendDefault({
      objectType: 'feed',
      content: {
        title: 'LVC 블로그에 놀러오세요!',
        description: 'LVC 블로그에는 다양한 주제의 글들이 있습니다. ',
        imageUrl:
          'https://i.ytimg.com/an/SPkqNswafRyRV9JrrmZDLw/featured_channel.jpg?v=600aa51b',
        link: {https://blog.naver.com/hanlyn1110
          mobileWebUrl: '사진클릭시 모바일 주소',
          webUrl: '사진클릭시 PC 주소',
        },
      },
      social: {
        likeCount: 좋아요 수, //99999가 최대입니다
        commentCount: 댓글 수, //99999가 최대입니다
        sharedCount: 공유 수, //99999가 최대입니다
      },
      buttons: [
        {
          title: '버튼1 글자',
          link: {
            mobileWebUrl: '클릭시 모바일 주소',
            webUrl: '클릭시 PC 주소',
          },
        },
      ],
    })
  }
</script>
<!-- www.blackcats4567.com -->
<!-- 이미지/버튼 클릭 시 주소는 Kakao Developers의 애플리케이션 > 플랫폼 > Web에 넣어야 클릭했을때 성공적으로 표시됩니다 -->
  </body>
</html>
