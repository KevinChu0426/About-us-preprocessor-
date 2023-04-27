# About-us-preprocessor-

## Pug

```
doctype html
head
  meta(charset='utf-8')
  meta(name='viewport' content='width=device-width')
  title GAN大的Studio
  link(href='style.css' rel='stylesheet' type='text/css')
nav
  .nav_logo(onclick="location.href='index.html'")
  .nav_space
  .nav_about ABOUT
  .nav_work WORK
  .nav_contact CONTACT
  img.nav_search(src='res/nav_search.png' width='24' height='24')
main
  #hi_there_and_welcome
  .brand_banner
    #we_are_a_company
    #that_believes_in
    #brand_banner_glasses
  .slideshow-container
    // section 1
    .slideshow-element
      .slideshow-pic
        #chiang_pic_1
        #chiang_clickme.clickme(onclick='flip()')
      #chiang-introduction.slideshow-introduction
        #chiang_pic_2
        .introduction_background
        .introduction_content
          h1 江沛晴`
          h2 設計總監 專案經理
          p
            | 國立成功大學工業設計所碩一，熱愛音樂、舞蹈，探索世界的未知領域，嘗試新鮮且具 有創意的事物。目前就職於洪郁修教授領導的精益產品研發中心，是認真學習精實管理、精實服務、精實醫療的小老鼠。
            br
            | 專長：Uxi design、Service design
            br
            | 工具：Ai、Ps、Pr、Figma
        .slideshow-closebutton(onclick='flip()')
    // section 2
    .slideshow-element
      .slideshow-pic
        #camilo_pic_1
        #camilo_clickme.clickme(onclick='flip()')
      #camilo-introduction.slideshow-introduction
        #camilo_pic_2
        .introduction_background
        .introduction_content
          h1 Camilo
          h2 設計師
          p
            | 國立成功大學資訊工程學系大四，喜歡踢足球、閱讀、游泳和隨心所欲地探索。
            br
            | 專長：前端開發、Ui design
            br
            | 工具：Figma
        .slideshow-closebutton(onclick='flip()')
    // section 3
    .slideshow-element
      .slideshow-pic
        #chu_pic_1
        #chu_clickme.clickme(onclick='flip()')
      #chu-introduction.slideshow-introduction
        #chu_pic_2
        .introduction_background
        .introduction_content
          h1 朱佑中
          h2 工程師
          p
            | 國立成功大學工業與資訊管理學系大二，熱愛電影、電視劇
            br
            | 專長：C++、Python、HTML、CSS、JavaScript
            br
            | 工具：Office
        .slideshow-closebutton(onclick='flip()')
    // section 4
    .slideshow-element
      .slideshow-pic
        #lin_pic_1
        #lin_clickme.clickme(onclick='flip()')
      #lin-introduction.slideshow-introduction
        #lin_pic_2
        .introduction_background
        .introduction_content
          h1 林冠銘
          h2 工程師
          p
            | 國立成功大學電機系大三，熱愛音樂、攝影
            br
            | 專長：C++、HTML、CSS、JavaScript
            br
            | 工具：Lr、Ai
        .slideshow-closebutton(onclick='flip()')
    // Next and previous buttons
    a.slideshow-prev(onclick='plusSlides(-1)')
    a.slideshow-next(onclick='plusSlides(1)')
  #group_pic
  #thanks_for_watching
footer
  p GAN大的 Studio
script(src='script.js')
script(src='https://replit.com/public/js/replit-badge-v2.js' theme='dark' position='bottom-right')
```

## Sass

```
*
  box-sizing: border-box
  margin: 0

html
  width: 100vw
  overflow-x: hidden

body
  width: 100%
  height: 100%
  background-image: url("res/background_small.jpg")
  background-size: 198px 398px
  background-repeat: repeat
  display: flex
  align-items: center
  justify-content: space-around
  flex-wrap: wrap

/* ---------------------------------
/* nav
/* ---------------------------------

nav
  height: 10vh
  display: flex
  align-items: center
  justify-content: space-around
  flex-wrap: wrap

.nav_logo
  background-image: url("res/nav_logo.png")
  background-size: cover
  margin-left: 10vw
  width: 75px
  height: 75px
  left: 5vw

.nav_space
  width: 25vw

.nav_about
  /* ABOUT

  font-family: 'Inter Tight', sans-serif
  font-style: normal
  font-weight: 300
  font-size: 18px
  line-height: 50px

  /* or 278%
  margin-right: 85px
  color: #111111
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25)

.nav_work
  /* WORK

  font-family: 'Inter Tight', sans-serif
  font-style: normal
  font-weight: 300
  font-size: 18px
  line-height: 50px

  /* or 278%
  margin-right: 85px
  color: #111111
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25)

.nav_contact
  /* CONTACT

  font-family: 'Inter Tight', sans-serif
  font-style: normal
  font-weight: 300
  font-size: 18px
  line-height: 50px

  /* or 278%
  margin-right: 123px
  color: #111111
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25)

.nav_search
  margin-right: 10vw
  filter: drop-shadow(4px 4px 4px rgba(0, 0, 0, 0.25))

.nav_logo:hover, .nav_about:hover, .nav_work:hover, .nav_contact:hover, .nav_search:hover
  cursor: pointer

/* ---------------------------------
/*
/* ---------------------------------

#hi_there_and_welcome
  width: 100%
  height: 40vh
  margin-top: 10vh
  background-image: url("res/hi_there_and_welcome.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat
  align-items: center

.brand_banner
  height: 50vh
  width: 100vw
  margin-top: 5vh
  position: relative

#we_are_a_company
  position: absolute
  width: 50%
  height: 100%
  left: 5%
  background-image: url("res/we_are_gan_gan_studio.png")
  background-size: contain
  background-position: center
  background-repeat: no-repeat

#that_believes_in
  position: absolute
  width: 50%
  height: 60%
  right: 5%
  background-image: url("res/that_believe_great_work_begin_with.png")
  background-size: contain
  background-position: center
  background-repeat: no-repeat

#brand_banner_glasses
  position: absolute
  width: 50%
  height: 50%
  right: 0
  bottom: 0
  background-image: url("res/glasses.png")
  background-size: contain
  background-position: center
  background-repeat: no-repeat

/* ---------------------------------
/* Slideshow container
/* ---------------------------------

/* Slideshow container

.slideshow-container
  height: 85vh
  width: 80vw
  left: 10vw

  /* for center allignment
  margin-top: 10vh
  position: relative

.slideshow-element
  display: none
  height: 100%
  background-image: url("res/slideshow_element_background.png")
  background-position: center
  background-size: cover
  background-repeat: no-repeat

.slideshow-pic
  height: 100%
  width: 100%
  position: absolute
  backface-visibility: hidden
  transform-style: preserve-3d

#chiang_pic_1
  position: absolute
  height: 90%
  width: 100%
  top: 5%
  background-image: url("res/chiang1.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

#chiang_clickme
  position: absolute
  height: 40%
  width: 40%
  top: 60%
  left: 50%
  background-image: url("res/clickme_chiang.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

#camilo_pic_1
  position: absolute
  height: 90%
  width: 100%
  top: 5%
  background-image: url("res/camilo1.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

#camilo_clickme
  position: absolute
  height: 40%
  width: 40%
  top: 60%
  left: 10%
  background-image: url("res/clickme_camilo.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

#chu_pic_1
  position: absolute
  height: 90%
  width: 100%
  top: 5%
  background-image: url("res/chu1.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

#chu_clickme
  position: absolute
  height: 40%
  width: 40%
  top: 60%
  left: 50%
  background-image: url("res/clickme_chu.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

#lin_pic_1
  position: absolute
  height: 90%
  width: 100%
  top: 5%
  background-image: url("res/lin1.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

#lin_clickme
  position: absolute
  height: 40%
  width: 40%
  top: 60%
  left: 10%
  background-image: url("res/clickme_lin.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

.clickme:hover
  cursor: pointer

.slideshow-introduction
  height: 100%
  width: 100%
  position: absolute
  backface-visibility: hidden
  transform-style: preserve-3d
  transform: rotateY(180deg)

#chiang_pic_2
  position: absolute
  height: 90%
  width: 100%
  top: 5%
  margin-left: -20%
  background-image: url("res/chiang2.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

#camilo_pic_2
  position: absolute
  height: 90%
  width: 100%
  top: 5%
  margin-left: -20%
  background-image: url("res/camilo2.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

#chu_pic_2
  position: absolute
  height: 90%
  width: 100%
  top: 5%
  margin-left: -20%
  background-image: url("res/chu2.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

#lin_pic_2
  position: absolute
  height: 90%
  width: 100%
  top: 5%
  margin-left: -20%
  background-image: url("res/lin2.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

.introduction_background
  position: absolute
  height: 100%
  width: 50%
  right: 0
  background: #8EA8A7
  box-shadow: -5px 0px 4px rgba(0, 0, 0, 0.25)

.introduction_content
  position: absolute
  width: 44%
  right: 3%
  display: flex
  flex-direction: column

  >
    h1
      margin-top: 20%
      font-family: 'Inter Tight', sans-serif
      font-style: normal
      font-weight: 700
      font-size: 32px
      color: white

    h2
      font-family: 'Inter Tight', sans-serif
      font-style: normal
      font-weight: 300
      font-size: 32px
      color: white

    p
      margin-top: 16%
      font-family: 'Inter Tight', sans-serif
      font-style: normal
      font-weight: 300
      font-size: 24px
      color: white
      line-height: 170%

.slideshow-closebutton
  position: absolute
  height: 10%
  width: 10%
  top: 3%
  right: 0
  background-image: url("res/close_button.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

  &:hover
    cursor: pointer

/* next & previous buttons

.slideshow-prev
  cursor: pointer
  position: absolute
  top: 50%
  height: 5vh
  width: 5vw
  color: white
  user-select: none

.slideshow-next
  cursor: pointer
  position: absolute
  top: 50%
  height: 5vh
  width: 5vw
  color: white
  user-select: none
  right: 0
  background-image: url("res/slideshow_next.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

.slideshow-prev
  left: 0
  background-image: url("res/slideshow_prev.png")
  background-position: center
  background-size: contain
  background-repeat: no-repeat

/* ---------------------------------
/*
/* ---------------------------------

#group_pic
  height: 90vh
  width: 80vw
  margin-left: 12vw
  margin-top: 5vh
  background-image: url("res/group_pic_decorated.png")
  background-size: contain
  background-repeat: no-repeat
  background-position: center

#thanks_for_watching
  height: 25vh
  width: 70vw
  margin-left: 15vw
  margin-top: 8vh
  margin-bottom: 20vh
  background-image: url("res/thanks_for_looking.png")
  background-size: contain
  background-repeat: no-repeat
  background-position: center

/* ---------------------------------
/* footer
/* ---------------------------------

footer
  width: 100vw
  height: 10vh
  background-color: #111111
  display: flex
  align-items: center

  > p
    margin-left: 15vw
    padding-left: 2vw
    padding-right: 6vw
    border-color: white
    border-width: 1px
    border-style: solid
    color: #ffffff
    font-family: 'Inter Tight', sans-serif
    font-size: 20px

/* ---------------------------------
/*
/* ---------------------------------
```
