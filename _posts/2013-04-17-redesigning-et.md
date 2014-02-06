---
layout: post
title: Redesigning an online newspaper
word_count: 2653
read_time: 13
---

# Background
## Life as a kid
I used to be an odd kid. Growing up in New Delhi, I always enjoyed reading the newspapers. Not just the page 3 stuff, but everything - the main stories, special columns, international news, you name it. On weekdays, I wouldn't be able to read in the morning since school started at 7:30am but I would come home around 2pm and it was the first thing I always did - read The Times of India (TOI) and The Economic Times (ET). Once every week, they'd come with special magazines like ET's Brand Equity and TOI's Sunday Times and those were awesome days. Apart from playing cricket, watching Star Sports and playing simulation video games, reading the newspapers would be one of my favourite things to do every day. I can't remember when or how I picked it up but it was definitely an odd thing to do at my age. When I think about it now, I credit a lot of my interest today in world affairs and news to this habit. Also, what's interesting is that it wasn't just the content I was interested in, but the disciplined layouts, variations in font sizes and weights, the colours and all the other aspects of the presentation. I think ET generally did a better job than TOI in presentation. As I approached my early teens, I got hooked to TOI's Delhi Times - the page 3 stuff, mostly for the Bollywood gossip and Heidi Klum pictures. But I wasn't inspired by its design - it was cluttered, lacked discipline and never made me feel nearly as good as reading ET would.
<div class="img-with-caption">
  <img src="/img/et.jpg" alt="The Economic Times, paper version">
  <h5>The Economic Times, paper version</h5>
</div>


## Today

Fast forward 15 years. I don't read newspapers anymore. Last time I read a newspaper in print was most definitely at an airport. Web and Twitter have made this a pretty widespread phenomenon. I'm still very interested in reading ET and TOI, but  I don't ever end up spending more than a couple of minutes on their digital counterparts. Being on the <a href="http://timesofindia.com">timesofindia.com</a> feels akin to being at a railway station during a riot. Stuff just comes flying at you from all corners of the screen. No I don't want a new ICICI credit card or travel insurance or a profile on shaadi.com. Neither do I want to read about Sunny Leone's new energy drink.

## The DailyMail.co.uk effect
The digital experiences of some of India's foremost news publications (especially timesofindia.com) have turned into tabloids. Compromising content quality and brand value in favour of 'spicy content' to get high click-through rates is a terrible idea. On top of that, placing obtrusive ads left, right and centre keeps readers like me far away on publications that do a much better job of presenting high-quality content with a decent design sense (<a href="http://qz.com">Quartz</a>, <a href="http://ft.com">FT</a>, as well as <a href="http://nytimes.com">NYT</a> to some extent). 
	<div class="img-with-caption">
  <img src="/img/dailymail.png" alt="The Daily Mail">
  <h5>The <a href="http://dailymail.co.uk">dailymail.co.uk</a> is a tabloid. Tabloids purposely seem to exhibit poor design sense.</h5>
</div>

However, apart from venting a tad bit about the state of online journalism in India, the purpose of this post is to share a <a href="http://etredesign.herokuapp.com">design I've created for The Economic Times</a>. I re-imagined what I'd want a digital ET to look like and created a couple of HTML/CSS mockups. Now I'm going to briefly share my design process that went into creating it. 

# The Design Process
## Content first, then design

The precursor to any good design is having a good sense of the content structure. Content comes first. For ET, I came up with a list of major sections a typical reader in 2013 would be interested in: Markets, Technology, Finance, Economy, Columns, World, Media, Specials (like Brand Equity), editor blogs, popular articles, breaking news, and detailed stories. 

Then I realized Economy and World are redundant in today's context because stories are better off being topic-localized than segregated by location. So, Media and Specials became Features,  while Columns became Opinion to be more consistent with ET's existing nomenclature. 

For an economic publication, markets is probably the most important topic. I needed to make this prominent somehow. After visiting some popular business-type journals, it seemed that indices and stock quotes were the most prominent sections under markets. So I decided to have a global indices and stocks section that would be accessible from any section of the site. 



This content structure was good enough to kick off the design.

## Vibes

Before designing mockups and prototypes for any project, I always come up with a list of vibes I'd want the design to give off. So this is what came to mind:

- <b>Disciplined</b>: Major newspapers traditionally belong to disciplined media. They shouldn't be comical or ostentatious. They adhere to strict standards and that's what makes them credible.
- <b>Bold/Prominent</b>: The content should be structured in such a way that whenever someone visits the site, they're instantly updated with what's making the news. Just as when a passerby glances at a newsstand and knows what's the main thing going on in the country/world.
- <b>Clean</b>: The existing ET site is pretty cluttered and there's barely any whitespace. While having excessive whitespace doesn't make business sense for a newspaper, there should be room to breathe. I wanted a little more whitespace than average just to take an opposite and more refreshing stance from the existing site. 
- <b>Paperish feel</b>: I wanted to recreate the experience of reading the paper version as a kid. Usually, this isn't the best strategy when designing for digital because the possible set of affordances in digital is radically different than that of print, but I still wanted that paperish feeling.
- <b>Slick</b>: I wanted modern elements to balance out the paperish feel to make it feel all 21st-century.

## Converting vibes into a design direction

I was pretty happy with what I had so far - I knew what I wanted. Usually, this is the hardest part in UX and life - knowing what you want. Even clients usually don't know what they want, they just say "we want it to look like that other thing" which is cool too but I always have the urge to steer them towards what they actually want. But once you know exactly what you desire, it's 100x easier to work towards getting there. Otherwise, it's like you getting in your car with no destination in mind. Being in a lost state can sometimes be good but not in this case when I wanted to start and finish this design on the same Saturday. The next step was to convert the list of vibes into a list of actual design elements to put in place to get closer to each of those vibes:

- Grids and dividers: A grid system seemed obvious in order to achieve discipline. Applying some design aesthetics of <a href="http://en.wikipedia.org/wiki/Massimo_Vignelli">Massimo Vignelli</a> seemed appropriate to perpetuate the discipline factor - so, things like bold bottom and top borders, square edges, lots of straight lines, strong alignment and use of varying font weights to create contrast was in order.
	
<div class="img-with-caption">
  <img src="/img/vignelli.png" alt="Massimo Vignelli's design aesthetic">
  <h5>The Vignelli design aesthetic (src: <a href="http://vignellidesign.tumblr.com/">vignellidesign.tumblr.com</a>)</h5>
</div>


- Big, bold titles and text: A significantly large font size for headlines and section titles seemed appropriate to achieve a more prominent look than typical news sites.
- Lots of padding and margins: To achieve more whitespace than average to exhibit a clean look.
- Background and font stack to mimic print: The Economic Times in print is defined by its peach-ish background and black serif font so I wanted to recreate that feel.
- Flat design, HTML5 embedded videos, big HD images, a responsive layout with a hamburger menu, and some Helvetification (actually, Helvetica for me has been dead for a while. Proxima Nova is in) here and there would add the modern into the design and make it look all 2013.

# The mockups
## Straight to HTML/CSS

By this point, I was getting pretty impatient and I just wanted to go ahead and convert all these specs into markup. Since I was short on time - I only allocated one day for this entire redesign - I decided to hit up my favourite text editor Sublime Text 2. Yes, I skipped Photoshop. The truth of the matter is that I'm way faster at HTML and CSS than Photoshop. It all comes down to what you're most comfortable with and if you're pretty fast at Photoshop or Fireworks or your favourite mockup tool, then by all means work in that first. But personally, I find that the control that HTML, CSS and JS give you is unmatched by any mockup tool out there. In addition, strategies such as bottom-up writing of media queries (as opposed to making the site responsive <i>after</i> finishing the desktop version), and hacking in Chrome Dev Tools let you test out a variety of design concepts very quickly.

From then on, it was simply iterating with frequent glances at the design direction notes.
<div class="img-with-caption">
  <img src="http://etredesign.herokuapp.com/static/img/et-redesign.png" alt="The redesign">
  <h5>My redesign of The Economic Times. You can access it at <a href="http://etredesign.herokuapp.com">etredesign.herokuapp.com</a></h5>
</div>




## The design, explained
I picked out 6 of the topics in the section list and made it the major sections of the site. For this redesign, I've created one of those sections: Technology, as well as what an article in that section would look like. 

## Navigation
I linked the major sections up at the top. Under each section in the top nav bar, there is a link to the main news article from that section. This is an effort to reduce the number of clicks the reader has to perform in order to get to the content - the backbone of the site. I like to think of the homepage and section page of any news site as layers hiding the content of news articles. The lesser the number of steps to the content, the better. This way of thinking stems from Bret Victor's <a href="http://worrydream.com/MagicInk/">landmark paper</a> on user interfaces (that I read in its 73-page entirety - it's like the mother of UI essays and I recommend it to anyone interested in user experiences). 

My friend <a href="http://twitter.com/aareet">@aareet</a> pointed out that the top nav bar could be fixed as you scroll even in the non-mobile view. Realized that made a lot of sense to maintain consistent behaviour with the mobile layout. It literally took 2 mins and 5 lines of jQuery to test this in Chrome Dev Tools. 
<div class="img-with-caption">
  <img src="/img/etredesign-1.png" alt="Scrolling navbar">
  <h5>A scrolling navbar was a 2-min hack in Chrome Dev Tools</h5>
</div>
 

## News ticker
The idea behind the ticker right below the top nav is that it would get updated in real-time with articles being published on the site, perhaps with a high-priority filter.

## Section header
I aligned the section header to the right in the section-view to create some whitespace in the middle of the page, and to the center in article-view to draw focus into the article content. After playing with a bunch of font stacks on <a href="http://typekit.com">Typekit</a> I went with the beautiful <a href="http://www.myfonts.com/fonts/dstype/acta-display/">Acta Display</a> for the giant serif header. I found this font to be a perfect fit as it was originally designed for a Chilean newspaper La Tercera and is conservative enough for a news site.

## Left sidebar
I went with a sidebar for the indices and stock quotes I wanted present site-wide (except on the article pages). This also creates a fair amount of real estate for ad spots - necessary for a newspaper publication. The idea is that these numbers would update in real-time. (It would be pretty cool to implement some rolling animation to update only single digits like the "Arrived" and "Boarding" in flight status boards at airports).

The sidebar goes away at screen-widths below 768px, adhering to the norms of good responsive design. 
<div class="img-with-caption">
  <img src="/img/etredesign-3.png" alt="The sidebar goes away in the mobile layout">
  <h5>The sidebar goes away in the mobile layout</h5>
</div>

## Right sidebar
I combined a popular articles section and video stories into a sidebar on the right. The video stories gives you the option of viewing 5 different embedded videos without navigating away from the page. I went with the awesome HTML5-based <a href="http://flowplayer.org">flowplayer</a> for this. It's by far the sexiest video player I've seen to date on the web.

## Featured section
The purpose of this section is to mimic the "Spotlight" section on ET's website. This would be to link to special, in-depth stories - the ones that usually occupy the entire page in the print version.

## Categories 
If you notice, every article link on the page contains category information right above the article headline, but they follow more of a "here's an article from Telecom, and here's an article from Software that's making the news" than a catch-all for stories from a particular category. The latter is the More Stories section (stole this idea from The Financial Times website).

## Article
In the article-view, I wanted to draw focus to the article headline, image and content. So I made the section-header significantly smaller and got rid of the left sidebar. I tried breadcrumbs but that seemed redundant (Home > Technology > Article headline) - both the homepage and section page can be reached by just clicking the appropriate headers. I placed the right sidebar next to the article. The idea is to have related content in that (like related news articles, videos and other stuff) as well as a banner ad.
<div class="img-with-caption">
  <img src="/img/etredesign-2.png" alt="Article-view">
  <h5>Article-view of the ET redesign, <a href="http://etredesign.herokuapp.com/article">etredesign.herokuapp.com/article</a></h5>
</div>

## Note to self: Take screenshots continuously

That's it! One thing I forgot to do was take screenshots of every version of the evolving design - I'll make sure to do that for my next project so that I have a visual reference for different design ideas I try and it would definitely make for a better blog post.


# Where to go from here
So far, these are just static mockups. I'd like to do the homepage next and play around with ways to make the design more context-sensitive. I was almost tempted to scrape off the content from economictimes.com and make this site dynamic so I can use a better ET everyday, but I don't think <a href="http://en.wikipedia.org/wiki/The_Times_Group">Bennett Coleman</a> (the company that owns ET and TOI) is going to like that. If you liked reading this article, drop me a line on twitter (<a href="http://twitter.com/sidjha">@sidjha</a>) or shoot me an <a href="mailto:sid@sidjha.com">email</a>. I love feedback. 