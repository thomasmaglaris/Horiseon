# 01 HTML CSS Git: Code Refactor

This task involves the practice of using the Scout Rule for existing code that has built the Horiseon web page in order to meet greater accessbility standards in terms of code readability plus enabling the web page to be more functional for those with any disability impairment or socioeconomic restrictions. Any changes/refactoring made to this code will be mentioned in this READ.ME file for further explanation. 

CHANGES:

title changed from 'website' to 'Horiseon'.
This allows for the company name to be seen on the tab as opposed to just seeing website. This change makes the company look more professional plus allows the user to see the companys website name if multiple tabs are open. 


Added id="search engine optimization" so that the search engine optimization link at the top of the web page will navigate to the right location on the webpage. Prior to this, clicking on the search engine optimisation link would result in no navigation at all. 


Added alternative text to all the image files in the html. Adding alternative text to all the images allows for people with visual impairments that may access the website through assistive technologies to understand what the image is showing without actually being able to see it. Therefore, the addition of alternative text for images has allowed for greater accessibility for disabled users. Furthermore, adding alternative text also makes it easier for a developer to know what image is what without having to rely solely on the image source. Finally, using clear, descriptive language in the alternative text also increases search engine recognition, further enhancing overall accessibility. 
Alternative text that was added for images are below
<!--<img src="./assets/images/search-engine-optimization.jpg" alt="notepad in office setting illustrating search engine optimization avenues"
<img src="./assets/images/online-reputation-management.jpg" alt="person on laptop with screen that illustrates reputation management through various graphs" 
<img src="./assets/images/social-media-marketing.jpg" alt="office professionals sitting around a desk that has various images relative to social media jargon such as 'like', 'share', 'tweet'."
<img src="./assets/images/lead-generation.png" alt="A wheel translating into a dollar sign to symbolise lead generation"
<img src="./assets/images/brand-awareness.png" alt="a light bulb over the face of a person to symbolise brand awareness"
<img src="./assets/images/cost-management.png" alt="a wheel translating into dollar signs to symbolise cost management"-->


Nested all the CSS selectors that share the same properties. This allows for easier readbility of the code when a developer is looking from the back end. Any css selector that shared the same property was nested and seperated via a comma. CSS selectors that were nested include:
<!-->.benefit-lead, .benefit-brand, .benefit-cost  {
    margin-bottom: 32px;
    color: #fffffff

.benefit-lead h3, .benefit-brand h3, .benefit-cost h3  {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-lead img, .benefit-brand img, .benefit-cost img   {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

.search-engine-optimization, .online-reputation-management, .social-media-marketing {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

.search-engine-optimization img, .online-reputation-management img, .social-media-marketing img {
    max-height: 200px;
}

.search-engine-optimization h2, .online-reputation-management h2, .social-media-marketing h2  {
    margin-bottom: 20px;
    font-size: 36px;
} 
-->


Changed semantic html elements to make the code easier to read and follow. One thing that really stood out on initial inspection of the code was that the < div > tag was used for just about everything. Changing some of these < div > tags to a better suited html tag will make it easier for the person to read the code and get a clearer idea of what he is inspecting. Changes to the semantic structure of the HTML are as follows:
 <!--Changed div to header, changed header > h1 > div to header > h1 > nav-->
 This is self explanatory as the there is a header section it is approprate to change the tag to header, whilst changing the other div to nav is also appropriate as the list items within that code contain navigation links to other areas on the page. 

<!--Changed all the divs within <div class="content" into a section tag-->
This makes up the main content of the page and it is clear that the main content is split into three sections. Hence, why section tags were used here. 

<!--Changed div tag to <aside class = "benefit" and all the divs within that aside tag are changed to section tags-->
Its clear from the visual lay out of this information and the content within it that this can be considered additional info. For that reason the div tag has been changed to an aside tag. However, there are still three sections evident within this aside tag, so those divs were changed into section tags also. 



To conclude, the changes made to this code have resulted in significant improvement in several key areas:
* the addition of a concise but descriptive title
* fixing the broken link so it navigates to the correct area of the page
* adding alternative text to all images present in the html
* nesting css selectors to condense and clean up the code
* Changing semantic elements for better readbility of the code. 

These changes have contributed to greater accessbility for those with a disability, greater overall usability of the webpage, optimised search engine crawls and enhanced accessbility for those who wish to access and read the code. 



