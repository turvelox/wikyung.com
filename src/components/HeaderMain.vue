<template>
    <header class="header" id="header">

        <div class="header-contents">

            <!-- Main-header -->
            <div class="main-header wd-1140">
                <div class="header-dw" id="header-dw">
                    <span class="header-date" id="header-date">2022. 03. 29</span><span class="header-weather" id="header-weather">비</span>
                </div>
                <h1 class="main-logo"><a href="#">위즈경제</a></h1>
                <div class="member-box" id="member-box">
                    <div class="no-login">
                        <a href="#" class="no-login-text">로그인을 해주세요.</a>
                    </div>
                    <div class="member-icon" id="member-icon"></div>
                </div>
            </div>

            <!-- GNB -->
            <nav class="gnb wd-1140" id="gnb">
                
                <ul class="depth-01" id="depth-01">
                    <li class="depth-01-item">
                        <a>
                            <img class="depth-01-item-icon" src="static/common/gnb_icon_01.png" alt="-" />
                            <span class="depth-01-item-text">경제</span>
                        </a>
                        <!-- <ul class="depth-02">
                            <li class="depth-02-item">
                                <a href="#">
                                    <span class="depth-02-item-text">금융</span>
                                </a>
                            </li>
                            <li class="depth-02-item">
                                <a href="#">
                                    <span class="depth-02-item-text">증권</span>
                                </a>
                            </li>
                        </ul> -->
                    </li>
                    <li class="depth-01-item">
                        <a href="#">
                            <img class="depth-01-item-icon" src="static/common/gnb_icon_03.png" alt="-" />
                            <span class="depth-01-item-text">부동산</span>
                        </a>
                    </li>
                    <li class="depth-01-item">
                        <a href="#">
                            <img class="depth-01-item-icon" src="static/common/gnb_icon_04.png" alt="-" />
                            <span class="depth-01-item-text">가상자산</span>
                        </a>
                    </li>
                    <li class="depth-01-item">
                        <a href="#">
                            <img class="depth-01-item-icon" src="static/common/gnb_icon_05.png" alt="-" />
                            <span class="depth-01-item-text">정치/정책</span>
                        </a>
                    </li>
                    <li class="depth-01-item">
                        <a href="#">
                            <img class="depth-01-item-icon" src="static/common/gnb_icon_06.png" alt="-" />
                            <span class="depth-01-item-text">사회</span>
                        </a>
                    </li>
                    <li class="depth-01-item">
                        <a href="#">
                            <img class="depth-01-item-icon" src="static/common/gnb_icon_07.png" alt="-" />
                            <span class="depth-01-item-text">기획/탐사</span>
                        </a>
                    </li>
                    <li class="depth-01-item">
                        <a>
                            <img class="depth-01-item-icon" src="static/common/gnb_icon_08.png" alt="-" />
                            <span class="depth-01-item-text">글로벌르포</span>
                        </a>
                        <!-- <ul class="depth-02">
                            <li class="depth-02-item">
                                <a href="#">
                                    <span class="depth-02-item-text">유럽(EU)</span>
                                </a>
                            </li>
                            <li class="depth-02-item">
                                <a href="#">
                                    <span class="depth-02-item-text">우크라이나</span>
                                </a>
                            </li>
                        </ul> -->
                    </li>
                    <li class="depth-01-item">
                        <a>
                            <img class="depth-01-item-icon" src="static/common/gnb_icon_09.png" alt="-" />
                            <span class="depth-01-item-text">Poll</span>
                        </a>
                        <!-- <ul class="depth-02">
                            <li class="depth-02-item">
                                <a href="#">
                                    <span class="depth-02-item-text">진행중인 Poll</span>
                                </a>
                            </li>
                            <li class="depth-02-item">
                                <a href="#">
                                    <span class="depth-02-item-text">종료된 Poll</span>
                                </a>
                            </li>
                            <li class="depth-02-item">
                                <a href="#">
                                    <span class="depth-02-item-text">Poll Bank</span>
                                </a>
                            </li>
                        </ul> -->
                    </li>
                </ul>

                <form action="" class="search-bar" id="search-bar">
                    <input type="search" id="search-bar-input" />
                    <button type="submit">검색</button>
                </form>

            </nav>

        </div>

    </header>
</template>

<script>

export default {
  name: 'HeaderMain',
  data(){
      
  },
  methods: {
      
  },
  components: {
    
  }
}
</script>

<style>



</style>
