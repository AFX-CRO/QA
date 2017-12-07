# Iris Html (#10) VWO Headline Test
Please use the *index.html* as a starting point for this project. The *original-pagesource.html* file is a copy of the view page source of this link: https://pro.chooseyourselffinancial.com/p/TreePreview/Preview/652703/False

## Doc Index
1. [Using this repo](#Using)  
2. [Where to put the css](#css)   
3. [Adding html](#html)  
5. [Secure](#Secure)
6. [Browser Support](#support)
7. [Transfering to vwo](#vwo)


##  <a id="using" name="Using">Using this repo</a>
	For now, feel free to overwrite the index.html doc with your changes. Once The preview link is circulating it maybe best to fork this, make changes locally, then merge once the changes are ready for QA(quality assurance). 


## <a id="css" name="css">Where to put CSS</a>
 Since this test won't use a lot of css please keep any additional css in the head content of *index.html*, in between the style tags and added /*vwo*/ /*vwo*/


##  <a id="html" name="html">Adding html</a>
	When adding html to this please surround your changes in <!-- vwo --> and <!-- / vwo --> This should help when transitioning this file to vwo. 


##  <a id="framework" name="framework">framework</a>
	Currently our pages use the foundation xy grid framework. It is in the styles1-1 sheet.


##  <a id="secure" name="secure">Secure</a>
	On the final product all links should be https and not http.


##  <a id="support" name="support">We support IE10 and up</a>
	If you code with that in mind the others should fall in line. :)


##  <a id="vwo" name="vwo">Taking the *index.html* file into VWO</a>
	We should only transfer to vwo the minimum amount of changes to the page necessary for the test. I am hoping that will be just copying the new css between the comments  /*vwo*/
  	   /*vwo*/ and updating the <!-- vwo →<!-- / vwo → html elements. 


