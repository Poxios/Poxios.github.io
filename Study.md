## 웹 폰트 font-face 사용법

```css
const globalStyles = createGlobalStyle`
    ${reset};
    @font-face {
        font-family: 'paybooc-Medium';
        src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_20-07@1.0/paybooc-Medium.woff') format('woff');
        font-weight: normal;
        font-style: normal;
    }
    @font-face {
        font-family: 'notosans-Regular';
        font-style: normal;
        font-weight: 400;
        src: url('http://fonts.gstatic.com/ea/notosanskr/v2/NotoSansKR-Regular.woff2') format('woff2'),
        url('http://fonts.gstatic.com/ea/notosanskr/v2/NotoSansKR-Regular.woff') format('woff'),
        url('http://fonts.gstatic.com/ea/notosanskr/v2/NotoSansKR-Regular.otf') format('opentype');
    }
    body {
        font-family: 'paybooc-Medium', 'notosans-Regular', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    }
    * {
        margin: 0;
        padding: 0;
    }
`;
```

import 해서 사용하는 법도 있지만, 웹 폰트 (woff, woff2) 들은 그냥 제공되는 웹서버에서 가져오는게 좋다.
