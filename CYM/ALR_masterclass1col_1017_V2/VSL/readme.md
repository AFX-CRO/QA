# VSL (#10) VWO Headline Test
Please use the *index.html* as a starting point for this project. The *original-pagesource.html* file is a copy of the view page source of this link: https://pro.chooseyourselffinancial.com/p/TreePreview/Preview/652703/False

### This folders preview link is: https://afx-cro.github.io/QA/CYM/ALR_masterclass1col_1017_V2/VSL/

## Doc Index
1. [Using this repo](#Using)  
2. [Where to put the css](#css)   
3. [Adding html](#html) 
4. [Secure Links](#Secure) 
5. [Framework](#framework)
6. [Browser Support](#support)
7. [Transfering to vwo](#vwo)
8. [Codes to transfer to vwo](#transferables)


##  <a id="using" name="Using">Using this repo</a>
	For now, feel free to overwrite the index.html doc with your changes. Once The preview link is circulating it maybe best to fork this, make changes locally, then merge once the changes are ready for QA(quality assurance). 


## <a id="css" name="css">Where to put CSS</a>
 Since this test won't use a lot of css please keep any additional css in the head content of *index.html*, in between the style tags and added /*vwo*/ /*vwo*/


##  <a id="html" name="html">Adding html</a>
	When adding html to this please surround your changes in <!-- vwo --> and <!-- / vwo --> This should help when transitioning this file to vwo. 


##  <a id="framework" name="framework">framework</a>
	Currently our pages use the foundation xy grid framework. It is in the styles1-1 sheet.


##  <a id="Secure" name="Secure">Secure</a>
	On the final product all links should be https and not http.


##  <a id="support" name="support">We support IE10 and up</a>
	If you code with that in mind the others should fall in line. :)


##  <a id="vwo" name="vwo">Taking the *index.html* file into VWO</a>
	We should only transfer to vwo the minimum amount of changes to the page necessary for the test. I am hoping that will be just copying the new css between the comments  /*vwo*/
  	   /*vwo*/ and updating the <!-- vwo →<!-- / vwo → html elements. 


## <a id="transferables" name="transferables">Codes to copy to VWO</a>

	Add this in the bottom section of <style> tag inside the <head> tag
	
	```
	/*vwo*/
		.headline-inner {
			font-family: 'Josefin Sans', sans-serif;
			background-image: url("https://d13p2xj50zkyqm.cloudfront.net/promos/LF/ALR/CryptoMasterClass_0817/ACT_CryptoMasterClass_DesignTest_Background.jpg");
			background-repeat: no-repeat;
			background-size: 100% 100%;
			margin-top: -3.1em;
		}
		
		.headline-inner p {
				font-family: 'Josefin Sans', sans-serif;
				color: #fff;
				text-align: left;
		}
		
		.headline-inner p.header-inner-top {
			font-weight: 700;
			font-style: italic;
			font-size: 33px;
			padding: 20px 0 0;
			margin-bottom: 0.6em;
			margin-left: 0.7em;
		}  

		.header-inner-middle {
			background: #42cbdb;
			opacity: .88;
		}

		.header-inner-middle  img {
			margin-top: 12px;
		}

		.headline-inner h1 {
			font-family: 'Josefin Sans', sans-serif;
			font-size: 40px;
			line-height: 50px;
			color: #001060;
			margin-top: 0.7em;
			text-transform: uppercase;
		}  
		
		.headline-inner h1 span {
			font-size: 50px;
			color: #fff;
			text-shadow: -4px 0px 0px rgba(0, 16, 96, 1);
		}

		.headline-inner p.header-inner-msg {
			font-size: 30px;
			line-height: 40px;
			text-align: center;
			font-weight: 700;
			margin-bottom: 0;
			padding-bottom: 15px;
		}

		.headline-inner p.header-inner-msg .author {
			font-size: 20px;
			text-transform: uppercase;
			font-weight: 500;
		}
		
		.headline .warning {
			display: block;
			width: 100%;
			font-size: 23px;
			color: #fff;
			background: #7d0000;
			margin-top: 0;
			margin-left: 0;
			padding: 10px 5px;
			text-transform: uppercase;
		}

		/*----------============= Queriers  =============--------*/
		@media screen and (max-width:750px){
			.header-inner-middle  img {
				display: none;
			}

			.headline-inner p.header-inner-msg {
				margin: 15px 5px 0;
			}
			
			.headline .warning {
				font-size: 22px;
			}
		}

		@media screen and (max-width:435px){
			.headline-inner { 
				background: #013667;
			}

			.headline-inner p.header-inner-top {
				font-size: 30px;
			}

			.headline-inner h1 {
				font-size: 34px;
				line-height: 40px;
				margin: 15px 0px 10px;
			}

			.headline-inner h1 span {
				font-size: 40px;
			}

			.headline-inner p.header-inner-msg {
				font-size: 28px;
				line-height: 32px;
			}
			
			.headline .warning {
				font-size: 20px;
			}
		}

		@media screen and (max-width:360px){

			.headline-inner p.header-inner-top {
				font-size: 26px;
			}

			.headline-inner h1 {
				font-size: 30px;
				line-height: 34px;
			}

			.headline-inner h1 span {
				font-size: 34px;
			}

			.headline-inner p.header-inner-msg {
				font-size: 24px;
				line-height: 28px;
			}

		}
	/*vwo*/
	```
	Replace whatever between  <!--====||  Start Headline  ||====--> to <!--====||  End Headline  ||====-->

	```
	<!--====||  Start Headline  ||====-->
  <!--== vwo ==-->
  <div class="headline">
    <div class="headline-inner">
      <p class="header-inner-top"><em>FOR THE FIRST TIME EVER&hellip;</em></p>

      <div class="row header-inner-middle">
          <div class="large-4 columns"><img src="https://d13p2xj50zkyqm.cloudfront.net/promos/LF/ALR/CryptoMasterClass_0817/millionaire-man.png"></div>
          <div class="large-8 columns">
            <h1>Eccentric Millionaire <br class="hidebr" />
              Reveals His Secret <br /><span>$1.8 Million</span><br class="hidebr" />
              Cryptocurrency Script</h1>
          </div>
      </div>

      <p class="header-inner-msg">“If you follow my script below, you could turn <br class="hidebr" />
          $100 into <i><u>a retirement fortune</u></i> in the next 12 months… <br class="hidebr" />
          while cutting your risk down to virtually zero!”<br />
          <span class="author">- James Altucher, crypto millionaire</span></p>
    </div>
    
    <p class="warning"><strong><u>WARNING:</u></strong> This opportunity disappears on February 2, 2018 at 4p.m.</p>
  </div>
    <!--== vwo ==-->
<!--====||  End Headline  ||====-->
	
	```
	Replace whatever beetween <!--=== /Video Script ==--> to <div class="unhide">

	```
	<!--=== /Video Script ==-->

  <!--== vwo / Remoeved some text from here / ==--> 

  <div class="unhide">

	```


