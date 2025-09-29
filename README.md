<!--We were told to make this layout using basic html and css, not custom fonts, so it will not match the original NYT layout
Cutting of marks just for the fonts seems petty.
AI was used in the process, but yeah, it did not help much. 
But hey, it's the future of coding, and you can't learn html, css in one day and do a raw assignment.-->

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>NYT Layout</title>
    <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: Georgia, "Times New Roman", serif;
    }

    .top {
      display: flex;
      justify-content: space-between; 
      align-items: center;
      padding: 10px;                                       /*Adjust as needed*/
      font-size: 14px;                                     /*Adjust as needed*/
      position: relative; 
    }

    .top-left {
      margin-top: 2px;                                     /*Adjust as needed*/          
      margin-left: 10px;                                   /*Adjust as needed*/          
      font-family: "Roboto", Arial, sans-serif;
    }

    .logo {
      position: absolute;                                  /* detach from flex flow */
      left: 50%;                                           /* move to middle horizontally */
      transform: translateX(-50%);                         /* correct offset */
      font-size: 40px;                                     /*Adjust as needed*/  
      font-weight: bold;
      font-family: "Times New Roman", serif;
    }

    .nav {
      display: flex;
      justify-content: center;
      gap: 20px;                                           /*Adjust as needed*/            
      font-size: 16px;                                     /*Adjust as needed*/
      margin-top: 6px;                                     /*Adjust as needed*/
      font-family: "Roboto", Arial, sans-serif;
    }

    .divider1 {
      /*border-top: 1px solid rgb(121, 121, 121);*/        /*Uncomment only to thicken the line*/
      border-bottom: 1px solid rgb(121, 121, 121);
      margin-top: 5px;                                     /*Adjust as needed*/
      margin-bottom: 3px;                                  /*Adjust as needed*/
      margin-left: 20px;                                   /*Adjust as needed*/
      margin-right: 20px;                                  /*Adjust as needed*/
    }
    
    /*A 2nd divider to lessen the gap betwween the 2 dividers*/
    .divider2 {
      /*border-top: 1px solid rgb(121, 121, 121);*/        /*Uncomment only to thicken the line*/
      border-bottom: 1px solid rgb(121, 121, 121);
      margin-bottom: 20px;                                 /*Adjust as needed*/
      margin-left: 20px;                                   /*Adjust as needed*/
      margin-right: 20px;                                  /*Adjust as needed*/
    }

    .article-section {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;                                           /*Adjust as needed*/
      padding: 0 20px 40px 20px;                           /*Adjust as needed*/ 
    }

    .article-left {
      display: flex;
      flex-direction: column;
      gap: 20px;                                           /*Adjust as needed*/
    }

    .article {
      border-bottom: 1px solid #ccc;
      padding-bottom: 15px;                                /*Adjust as needed*/                
    }

    .article h4 {
      font-size: 12px;                                     /*Adjust as needed*/                   
      text-transform: uppercase;
      color: gray;
      margin: 0 0 6px 0;                                   /*Adjust as needed*/
      font-family: "Roboto", Arial, sans-serif;
    }

    .article h2 {
      font-size: 22px;                                     /*Adjust as needed*/             
      margin: 0 0 10px 0;                                  /*Adjust as needed*/   
      font-family: "Merriweather", Georgia, serif;
      font-weight: 700;                                    /*Adjust as needed*/           
    }

    .article p {
      font-size: 16px;                                     /*Adjust as needed*/         
      margin: 0 0 6px 0;                                   /*Adjust as needed*/         
      line-height: 1.4;
      font-family: Georgia, "Times New Roman", serif;
      text-align: justify;
    }

    .article span {
      font-size: 12px;                                     /*Adjust as needed*/           
      color: gray;
      font-family: "Roboto", Arial, sans-serif;
    }

    .article:last-child {
      border-bottom: none;
    }

    .article-right img {
      width: auto;
      height: 80vh;                                        /*Adjust as needed, to fit the screen as was shown in the lab. The image size may look different on your screen*/
      object-fit: cover;
      display: block;
    }

    .article-right span {
      display: block;
      text-align: right;
      font-size: 13px;
      color: gray;
      font-family: "Roboto", Arial, sans-serif;
      margin-top: 10px;                                    /*Adjust as needed*/           
    }
  </style>
</head>
<body>

  <div class="top">
    <div class="top-left">
      <div>Sample day, Month, Day, Year here</div>         <!--Day, date, month and year here-->
      <div>Today’s Paper</div>                             <!--Or you can put a date here-->
    </div>
    <div class="logo">
      <div>The New York Times</div>
    </div>
  </div>

  

  <div class="nav">
    <div>U.S.</div>
    <div>World</div>
    <div>Business</div>
    <div>Arts</div>
    <div>Lifestyle</div>
    <div>Opinion</div>
    <div>Audio</div>
    <div>Games</div>
    <div>Cooking</div>
    <div>Wirecutter</div>
    <div>The Athletic</div>
  </div>

  <div class="divider1"></div>
  <div class="divider2"></div>

  <div class="article-section">
    <div class="article-left">
      <div class="article">
        <h4>Analysis</h4>
        <h2>Article Title Here</h2>
        <p>Description Here, sample text, lorem ipsum dolor sit amet consectetur adipiscing elit sed do eiusmod tempor incididunt ut labore et dolore magna aliqua ut enim ad minim veniam quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat</p>
        <span>Timer Here</span>                           <!--like '3 min read', '5 min read' etc-->
      </div>

      <div class="article">
        <h2>Article Title Here</h2>
        <p>Description Here, sample text, lorem ipsum dolor sit amet consectetur adipiscing elit sed do eiusmod tempor incididunt ut labore et dolore magna aliqua ut enim ad minim veniam quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat</p>
        <span>Timer Here</span>
      </div>

      <div class="article">
        <h2>Article Title Here</h2>
        <p>Description Here, sample text, lorem ipsum dolor sit amet consectetur adipiscing elit sed do eiusmod tempor incididunt ut labore et dolore magna aliqua ut enim ad minim veniam quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat</p>
        <span>Timer Here</span>
      </div>
    </div>

    <div class="article-right">
      <img src="1920x1080.jpg" alt="Sample Image Title">  <!--Put your image in the same folder and put your image name on src-->
      <span>Sample Text Here</span>                       <!--Put Whatever text here-->
    </div>
  </div>

</body>
</html>

