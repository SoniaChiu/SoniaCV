<!DOCTYPE html>
<html>
  <head>
     <!-- bootstrap 載入css, js-->
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>
     <!-- 載入 jquery -->
     <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.8.0/jquery.min.js"></script>
     <!-- 引入外部檔案的方式 -->
     <script type="text/javascript" src="commonFunc.js"></script>
     <link rel="stylesheet" type="text/css" href="style.css">
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.8.1/font/bootstrap-icons.css">
    <title>Sonia's Website</title>
    
    <!-- update the version number as needed -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <style>
      html, body {
        height: 100%;
      }
      /* 點擊偏離 解決方案 */
      :target {
        padding-top: 56px;
        margin-top: -56px;
      }
    </style>
  </head>
  <body>
    <header>
      <ul class="header__nav">
        <li class="nav__item"><a href="#section--1" title="1">PROFILE</a></li>
        <li class="nav__item"><a href="#section--2" title="2">EXPERIENCE</a></li>
        <li class="nav__item"><a href="#section--3" title="3">EDUCATION</a></li>
        <li class="nav__item"><a href="#section--4" title="4">STRENGTHS</a></li>
      </ul>
      <a class="hamBar" href="#">
        <i class="bi bi-list"></i>
      </a>
    </header>
    <main class="main">
      <div class="self_card">
        <img
          class="avatar"
          src="./img/Sonia.jpg"
          alt="Loading error" />
        <div class="self_intro">
          <h1>Jing Ya Chiu</h1>
          <br/>
          <h3>Marketing / PR</h3> 
          <br/>
          <br/>
          <br/>
            <div style="display: flex; flex-direction: row; align-items: center; margin-left: 15px;">
              <i class="bi bi-telephone-inbound"></i>
              <div style="padding-left: 5px;">0919-167-362</div>
            </div>
            <div style="display: flex; flex-direction: row; align-items: center; margin-left: 15px; margin-top: 5px;">
              <i class="bi bi-envelope"></i>
              <div style="padding-left: 5px;">soniiachiu@gmail.com</div>
            </div>
        </div>
      </div>
      <div class="content" style="background-color: white;">
        <section id="section--1">
          <h2 class="section__title">Profile</h2>
          <p>Results-oriented and flexible coordinator with extensive working experience in marketing. 
            <br/>Collaborative in working closely with strategic and creative teams to develop marketing plans for the brand.</p>
        </section>
        <section id="section--2">
          <h2 class="section__title">Experience</h2>
          <p>
            <p><h5>Sino Cell Technologies, Taipei, Taiwan</h5>
              <h6>Senior Specialist (Jan 2021 - Present)</h6>
                  ．Content marketing. Copywriting, includes website articles, social media posts, journal, advertorial, news release
              <br/>．Manage multiple social media channels, including Facebook fanpage, website, Youtube, Line@ 
              <br/>．Revised digital marketing strategy by re-positioned tone and manner of social media
              <br/>．Improve UI & UX by converting website into RWD
              <br/>．Brand management. In charge of annual marketing plan, budget management
              <br/>．Work closely with the manager of Scientific R&D dept. to generate biotechnology-related content 
              
              <br/><br/><h6>Achievement</h6>
                   ．Plan and optimize advertising strategy, which improved click through rate by 3% 
              <br/>．Improve search engine ranking and achieved No.1 ranking naturally
              <br/>．Cell therapy obtained the legislation permission. News release acquired more than 30 media exposures
              <br/>．Planned the promotion campaign for the exhibition and increased sales for 3 cases, which was the maximum profits of the past three years
              <br/>
    
              <br/><p><h5>Strategic Public Relations Group, Taipei, Taiwan</h5>
              <h6>Account Executive (Mar 2019 - May 2020)</h6>
                   ．Enhanced brand’s SOV and increase sales performance by developed KOL / KOC strategies on social media or social forums
              <br/>．Social listening, prepared response documents beforehand in case any negative messages appeared
              <br/>．Built and maintained relationships with KOL and KOC to elevate brand awareness 
              <br/>．Monitored news coverages in asset management industry, analyze industrial trends and creating media exposure for clients
              <br/>．Arranged and executed campaigns for B2C market including press conference, consumer events, TV/online news cooperation shooting
              <br/>．Organized content for website maintenance, by proposing appropriate industrial candidates for interview, editing and distributing articles
            
              <br/><br/><h6>Achievement</h6>
                   ．KOC’s posts on Facebook groups acquired 5 media exposures and increased sales for the brand
              <br/>．Acquired the maximum of KOL’s exposures and attendance in asset management press conference over the years
              <br/>
    
              <br/><p><h5>Ogilvy & Mather Public Relation, Taipei, Taiwan</h5> 
              <h6>Administrative Assistant (Nov 2017 - Jul 2018)</h6>
                   ．Monitored news coverages in luxuries industry, generated reports on a daily/weekly/monthly basis
              <br/>．Assisted in press conferences, media gathering events, opening of pop-up stores
              </p>
          </p>
        </section>
        <section id="section--3">
          <h2 class="section__title">Education</h2>
         <p> Shih Hsin University                                                                                                                        Taipei, Taiwan
         <br/>Bachelor of Art, June 2018	
         <br/>Major: Public Relations and Advertising
         </p>
         
          
        </section>
        <section id="section--4">
          <h2 class="section__title">Strengths</h2>
          <p>Flexibility, organization, curiosity, creativity
            <br/>Meta business suite and business manager, Wordpress, Google Analytics
          </p>
        </section>
        
      <div>
    </main>

       
    <script>
      $(document).ready(() => {
        $('.hamBar').click(function(){
          //避免 a 標籤會觸發
          event.preventDefault();
          //觸發展開收起來
          $('.header__nav').toggleClass('show');  
        })
        $('.header__nav li a').click(function(){
          event.preventDefault();
          //移除class，才會讓 menu 消失
          $('.header__nav').removeClass('show');
          var sectionTitle = this.title;
          console.log(sectionTitle);
          var sectionId = "#section--" + sectionTitle;
          console.log(sectionId);
          var scrollPoint = $(sectionId).offset().top;
          var lastScrollPoint = scrollPoint - 100;
          $("html,body").animate({ scrollTop: lastScrollPoint }, 800);
        })
      });
    </script>
  </body>
</html>
