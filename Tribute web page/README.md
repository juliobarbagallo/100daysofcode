Tribute web page.

Tuesday, July 28, 2020
4:17 PM

User Story #1: My tribute page should have an element with a corresponding id="main", which contains all other elements.
	
	So, we are going to have a <main> element with an id attribute with the value of "main"
	
	<main id="main">
	…
	</main>
	And basically inside this main tag we will have our web content and child elements.
	
User Story #2: I should see an element with a corresponding id="title", which contains a string (i.e. text) that describes the subject of the tribute page (e.g. "Dr. Norman Borlaug").

	Here we need an HTML element with and id attribute with the value = "title"
	A good idea for a title, would be to use an <h#> element and because of that, an <h1> could work for this, so it would be like <h1 id="title">Red Hot Chili Peppers."</h1>

User Story #3: I should see a div element with a corresponding id="img-div".

	Here it says that needs a div element, for what we can know about this request, we need to load an image about our tribute.
	To load an image, we are going to use figure and img elements. To check how it works fo to> https://www.w3schools.com/tags/tag_figure.asp
	<div id="figure-div">
		<figure id="img-div">
			<img id="image" alt="Red Hot Chili peppers." src="https://wallpapercave.com/wp/wp1823246.jpg"/>
			<figcaption id="img-caption">
			      Red Hot Chili peppers.
			    </figcaption>
			
		</figure>
	</div>

	Some notes here, we are using alt (alternate text) attribute to help in case the image doesn’t load. And, we are also using a figurecaption to add a caption to the <figure>
	
User Story #4: Within the img-div element, I should see an img element with a corresponding id="image".

	This is done on the US#3.
	
User Story #5: Within the img-div element, I should see an element with a corresponding id="img-caption" that contains textual content describing the image shown in img-div.

	Also done on US#3.
	
User Story #6: I should see an element with a corresponding id="tribute-info", which contains textual content describing the subject of the tribute page.

	For this webpage section we can easily use a <section> element with and id attribute equal to "tribute-info". From the page we are using as reference (https://codepen.io/freeCodeCamp/full/zNqgVx), its using this part to enumerate on a list a timeline of the Dr. Borlaug's life.
	
	So, for this we are going with <section id="tribute-info"> … list for the timeline </section>. But, as I am doing it for the RHCP, we are using the list with released albums and years.
	<section id="tribute-info">
	    <h3 id="headline">RHCP albums list.</h3>
	    <ul>
	      <li><strong>1984</strong> - The Red Hot Chili Peppers.</li>
	   </ul>
	…
	</section>
	</main>
	
User Story #7: I should see an a element with a corresponding id="tribute-link", which links to an outside site that contains additional information about the subject of the tribute page. HINT: You must give your element an attribute of target and set it to _blank in order for your link to open in a new tab (i.e. target="_blank").

	This request needs to have a link <a>, an anchor tag with and id attribute = "tribute-link"
	Like, <a id="tribute-link">
	<h3>
	      If you like to know more about one of the biggest and famous band which always knew how to evolve and adapt, check the following
	      <a id="tribute-link" href="https://en.wikipedia.org/wiki/Red_Hot_Chili_Peppers" target="_blank">Wikipedia entry</a>.
	 </h3>
	
So far, we are almost done, at least we finished the HTML part. The next 2 request resides on the CSS side.

User Story #8: The img element should responsively resize, relative to the width of its parent element, without exceeding its original size.

	img {
	  max-width: 100%;
	  display: block;
	  height: auto;
	  margin: 0 auto;
	}
	
Making images responsive with CSS is actually very simple. You just need to add these properties to an image:
img {
  max-width: 100%;
  height: auto;
}
The max-width of 100% will make sure the image is never wider than the container it is in, and the height of auto will make the image keep its original aspect ratio.

From <https://www.freecodecamp.org/learn/responsive-web-design/responsive-web-design-principles/make-an-image-responsive> 

User Story #9: The img element should be centered within its parent element.

	Its done on the US#9
	
And that’s it from the requests we got. Now, the improvements to the CSS.
