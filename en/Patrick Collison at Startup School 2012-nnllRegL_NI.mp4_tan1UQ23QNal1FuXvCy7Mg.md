**Patrick Collison at Startup School 2012-nnllRegL\_NI.mp4**  

\[00:00:00\] Morning them.

Hopefully this clicker works.

When I sat down to write this talk I really racked my brains to try to figure out what the most interesting and relevant and useful content would be for a lot of people who were sort of interested in web startups.

When I thought about it in those terms.

The topic of my talk became fairly obvious but then.

I thought about it more and the Algren doesn\'t even seem to be deterministic.

I\'m not sure anyone even knows how it works.

So I guess I\'ll actually have to talk about stripe instead.

Two years ago Brian from Airbnb Inbee spoke at Sahib\'s school.

In 2010 he opened his talk by showing a picture of Startup School in 2008.

Two years previously and that picture showed a snapshot of the audience and he picked out one particular head.

He was just sitting there and anonymous had in the audience and I know this because I was at his talk in 2010.

And so two years later he was on stage outside of school and somehow two years later here I am and I\'m sure there\'s at least one person here who who\'ll be on stage in two years time and stripe definitely isn\'t as far along as air being.

But it drove home the point to you when I realized this that startups are very unpredictable.

You know software is really hard to get your head around somebody telling me not all that long ago that that evidence was just becoming a huge success.

They were making something like ten thousand dollars a week and we\'re thinking man that\'s really impressive.

And now I\'ve no idea what urban Ebony\'s actual revenue figures are today but it wouldn\'t at all shock me if they\'re making ten thousand dollars an hour.

Like what Dad even liked to try to build a company for that kind of growth is possible.

Startups are strange for a whole bunch more reasons.

They\'re usually kind of counterintuitive because they were counterintuitive.

Somebody else would probably solved the problem is already on top of that.

Startups often don\'t actually want don\'t actually want to be all that well understood it can actually be quite helpful to be sort of under estimated and under comprehended.

But I think the biggest reason that startups are hard to understand is that so few people still get to see them up close during those first couple orders of magnitude.

And when people do tell the stories or from the stories are told they often tend to be kind of wrong.

They\'re about sort of rocketships and frantically holding on and trying to add more server capacity as quickly as you can to handle the next million users.

They\'re not about the late night arguments and wondering if your product could ever possibly work more.

Trying to figure out when you launch your product why it\'s not growing.

The thing is even the really successful startups have this phase that that famous summer when Facebook moved out to Palo Alto in 2004.

Most people don\'t realize this but there were other people in the same house working in other startups like this is the most successful technology company started in the 21st century and in the same house there were people working at a startup ideas six months after launch.

It\'s it really takes a while.

And so stripe is obviously very very different to Facebook and urban bee and nowhere near as far along as they are.

But we\'ve now gone through a small bit of growth.

And so I want to try to describe how it actually works.

In October of 2009 John and I were walking home from dinner in Potrero up in the city.

I\'ve been kicking around this idea of starting an online payments company.

We\'re really kind of fascinated by the concept of Internet payments and all the other companies in the space seemed like total dinosaurs.

And as the web sort of spread around the world and more deeply into our lives through mobile devices it seemed kind of obvious there should be some kind of universal payment infrastructure for the Internet to be just really easy to transact online.

And John just turned to me he said you know while the debate about you know what I would just go build it won\'t be all that hard.

 \[00:04:00\] He actually said that if I won\'t be all that hard and so I said okay sure why not backtracked a little bit here.

 \[00:04:09\] John is my co-founder at stripes.

He\'s ulting my brother.

And people often ask me about how this works in practice.

And so for the record started a company with your brother.

Turns out to be a really good idea.

John is not only the most brilliant people I know.

I think he got the highest results in Irelands university entrance examinations but he\'s also someone with whom I\'ve literally decades of experience building things.

 \[00:04:33\] Here\'s an earlier venture that we worked on together.

 \[00:04:38\] And so it\'s October 2009 we decide to work in this online payments company.

We decided to call it slash dev slash payments.

The API should be just as straightforward as any other node endeavor Fasth were kind of OK had programming and definitely not at naming things.

But everyone else seriously have been targeting their product.

They told us a finance sector product they were targeting chief foes and business people.

And we thought the international just moving in a completely different direction.

We decided to target makers the people actually building things.

We thought that Internet payments was a technology problem and we wanted to build a completely new stack for anybody transacting online.

So we worked nights and weekends.

We were both in college at the time I was at MIT.

And John was off the road at Harvard and so we\'d code together in the evenings between problem sets and writing papers.

January rolls around switch for both of those schools.

You sort of have that month off but of course anybody who knows Boston knows a January in Boston is unbelievably freezing.

And so we decide to go somewhere else to work for the month.

We read a few blogs that claim the one Azarias was surprisingly a really good place to get things done.

It\'s it\'s pretty cheap it\'s really warm it\'s friendly.

For some reason I don\'t know why those Wi-Fi everywhere everything happens on a really late schedule like the bars up until 5:00 AM nobody has dinner until midnight and nothing starts before noon.

It\'s Veazey a city on a programers schedule.

So we read all of this really great.

We\'ve got to run as our eyes.

And so we did and we just worked nonstop in cafes for three weeks.

I still never seen a single one of the tourist attractions and one Azarias or I presume they exist and then read like we could all day and we go to dinner at 11:00 o\'clock or something and then go to bed.

I can\'t emphasize this enough if you want to get something done consider going to an Atari\'s.

On January 9.

We got our first production user for sloughed slushed such payments.

Like I say it.

This is only a few weeks after we started working on it but we really wanted to get production users shaping the product as quickly as we could.

The user was a friend of ours.

I called Ross Bouchet who was working in a company called Tweetie north at the time.

Results also actually wisely funded.

Funnily enough he actually became the seventh person to work at stright but that\'s a separate story.

Here\'s a screenshot of what DIAF payment looked like at the time and this screenshot you can see that John and I are definitely programmers and not designers but OK.

So January 9th we now have one user.

This great story from the early days of Amazon how a celebrated when they got their first buyer who wasn\'t any of their moms.

And you know Ross wasn\'t exactly our mom but he was a good friend.

So we definitely weren\'t out of the woods just yet.

So we went back to school and we can do to work on debt payments in our spare time.

There was this one cafe that I worked out of so much they took pity on me and I\'m still Facebook friends with a bunch of the Bristow\'s.

Yeah like strivings that kind of unusual company.

We\'re about technology but roles about payments and the technology side requires good reliability and you know clean baby eyes and a really nice product and have lots of technology things Wheatley\'s hoped to know something about.

But the Peyman side requires working with banks and dealing with credit card companies and just generally handling a slew of finance industry issue issues.

We really had no new experience with no idea how to handle.

We love meetings where I sort of sat somebody down and said Right.

So payments how do they work.

Programmers often and this is unfortunate looked down at the folks who are trying to learn to code of.

I want to learn real for my web startup crowd but actually a lot of sympathy for them because we were that bad.

But in finance summer came around to of six months and we moved out to Palo Alto though we hadn\'t actually yet decided to take leave from school.

We found a tiny bungalow just off university and the living room and the kitchen became our office.

It was pretty hot didn\'t have any air conditioning and so John just slept in the garden most nights wouldn\'t allow me to post a picture of this.

And by and large we just kept on writing code because I mean that\'s mostly what sauteing a software company looks like in the early days or through the writing code or you\'re talking to people who use the code or you\'re wasting time.

And here\'s a chart of our transaction volume over the first six months.

And that\'s not a technical error.

If you look really closely you can see a tiny little wiggly line at the bottom.

It\'s admittedly not wiggling all that much around this time though we did have our first person join and we\'re based in Silicon Valley home to the best international talent from Berlin to Beijing to Bangalore and so of course we took full advantage of it.

We heard a guy called Dara Butley who was one of my smartest friends from college and he grew up in a small town called Limerick in Ireland.

About 2 miles from here John and I grew up.

Raised our first investment for our first real investment I guess.

Why see it obviously already invested.

This was from from Peter Till then we hadn\'t told very many people about DIAF payments and those we had told had reacted mostly by telling us we were crazy.

But of course luckily Peter Teal is crazy.

So he invested and it\'s been really helpful to have him on board.

Soon after that moved into our first office which looked something like this.

It\'s actually sort of said Ramona and university and Parlato just sort of Cubitt cafe.

It\'s actually a converted house and because it was a house it had this wonderful fireplace the world light in the winter.

The fireplace looked something like this which I think may have contravened some fire in the workplace codes and baozi were just working nonstop.

We acted to we we became four people around this time.

The first person fourth person was a guy named Greg.

I remember when Greg was sort of considering joining and dropping out of school he asked me about our work schedule and whether or not we worked weekends.

Obviously we did work weekends but he really didn\'t want to make this sort of scare him off and make it seem like he\'d have to answer.

So I sort of said well you know we usually work some of the weekend we really care about work life balance and we just cut me off means I\'m great.

I\'m not on the same page and working all day everyday.

And so we knew he\'d fit in.

We decide to change our name.

I can\'t even begin to list the problems that flashed such payments had somehow it turned out that not everyone immediately got the devil S analogy.

Nobody was really able to get their head around the whole slash thing and we started to get Mayeux with things like this.

And then there was the admittedly pretty inconvenient fact that Amazon had launch a product an online payments product called Amazon dev pay and so it precursory just wasn\'t going to work out and so we spent hours brainstorming names and we eventually came up with the name stripe and we didn\'t actually think that stripe was all that great an aim for come up with it but we decided to just put a date in the calendar and if we didn\'t come up with a better name by that date then we\'d stick with stripe.

And sure enough it became striped and actually a few months later I learned that this is how Apple ended up with a name Apple with the exact same thing.

Jeremy reached the end of our first year mostly intact.

A bunch of Y Combinator companies started to use Stripe and those was pretty good where we\'re getting some real feedback.

And here\'s another chart.

This are transaction volume through the first year.

And so it\'s still kind of a ways to go.

We spent January of 2011 our one year anniversary in Rio de Janeiro because January in South America was becoming a tradition as anyone who\'s been to Rio de Janeiro knows it\'s when most beautiful places on earth.

 \[00:12:11\] And of course we took full advantage of it.

 \[00:12:18\] At this point we\'re an invite only private beta and so there probably is something obvious we could have done to grow at least a little bit faster are you to launch a friend refers to invite only private beta as the baby blankets of startups.

And I think that\'s about right.

But the beta period was actually really helpful to stripe and were Paul Buchheit saying that should start out by making hundred people really happy rather than many more people.

Only a little bit happy you really took this to heart and took advantage of the small number of users to really focus on them as much as we could and really try to figure out what they wanted.

Forgiveable not long after we launch the first version of strife we had a Peter duty so we\'d all get called from the site with down pretty standard and pretty reasonable.

But then we realized that any time a user gets any kind of error or like even if the site is down that\'s actually a really bad experience for them and we could probably make them much happier if we went and investigated the error and sort of proactively reach out to them and help them fix it.

 \[00:13:14\] And so we changed the code a little bit so that any time anyone hit any error it would send an e-mail that would go sort of straight the top of everybody\'s inbox and I would also phone everybody and we\'d go and fix it no matter what.

And I really mean that I would get out of bed if necessary.

We\'re basically never without a laptop and the means to tether.

Here\'s a photo of one such incident.

This is Greg and I have gone to the cinema in Redwood City a user encountered an error.

And so of course out came our laptops and we had to go fix it.

I think Greg I think Greg is here so much.

 \[00:13:46\] I mean I think he still feels a little bit bitter about missing the start of the movie over this movie may or may not have been Twilight Breaking Dawn start after high stress you need to unwind.

 \[00:14:00\] We also realize that ending with an engineer is basically the best support experience possible.

Like it\'s really frustrating to have to go into to file a ticket and find the support email address and then wonder does this come to reply to those who bought e-mails or if they do reply.

How long does it take them or all of these issues.

Like it\'s much nicer you can just start sort of directly chatting with somebody.

And it\'s also way more productive for us because we can then go and sort of try to figure out what the underlying issue is rather than having to sort of guess based on the user\'s initial description.

So we just opened up this chat system on our Web site where anyone can jump in and just start asking questions and we actually still have this today and that was it was really good but then we thought why stop there.

Isn\'t it really a really bad experience when somebody asks a question and there\'s nobody there to answer them.

And so we a hot pager duty.

And so we hooked it up so that if you asked a question in the Streib chat room and there was nobody there to answer you it would go and phone one of us after 30 seconds.

And so I don\'t think many of you will know this but like for many months that stripe if you asked a question in our chat room there\'s no one there to answer someone would be woken up if necessary to help you.

 \[00:15:02\] We don\'t do that today.

 \[00:15:07\] So those strike wasn\'t yet publicly available to everyone.

We really tried to sort of turn up the dial on our users feedback and to force ourselves to be extremely sensitive to what they wanted and what their experience was like.

We our users talking to us during every waking hour.

And if anything went wrong for them they were like literally interrupting our sleep.

The other thing that comes in bated was the fact we weren\'t just building a fin software layer.

We thought that stripes would encompass everything from the API requests to have the money ended up in your bank account and we wanted to able to define the experience.

And we wanted to be able to do it at scale.

We were really influenced by things like Amazon Web Services and easy to watch.

It\'s really interesting innovation because you see two is fantastic you\'re a smaller company or a startup startup or a side project or something like this but it scales right through to be a Netflix or a Zynga or indeed an Amazon.

 \[00:15:58\] It\'ll work for a company of any size and we decided we wanted to do that.

But for internet payment infrastructure we wanted to make something that was really easy to start with but something would also work for the largest companies in the world.

Until that meant working with really good banks.

The problem is that banks and startups are basically the business equivalent of oil and water and figuring out how to combine them is pretty hard.

The best bank in the business is like Wells Fargo which powers some of the largest payments companies in the world and almost it was pretty tough to get them to talk to us or even to return our e-mails.

Their price hardware some strange kind of Nigerian scam like Make Money Online Fast from the comfort of your own home.

So we asked a friend an investor and now a partner at Y Combinator.

Jeff Ralston to help out.

Jeff had previously been CEO of a company called Lalah an online music startup and they had negotiated successfully with the record labels and we thought that if you could as a technology startup negotiate successfully with the record labels you could basically convince anyone in the world to do anything ever.

And here\'s a picture of Jeff on a conference call with Wells Fargo.

That\'s Dhara.

They\'re on the other side and you might wonder why is Jeff on the floor.

Well Jeffrey on the floor.

Because our office was also flooded at the time.

We also had a security audit that day sometimes trucks are just like a reality TV show.

It\'s like negotiate with one of the biggest banks in the world.

While Undergoing a security audit while wading through water and the water is full of Trina\'s or something.

But thanks to Jeff and a bunch of others we eventually convinced Wells Fargo to become one of our backhands in moving all of our systems to work out of their platform.

It was a couple of weeks of honestly really intense work we had to hit a particular deadline.

This is the night of our first successful transaction.

This is John after another particularly long all nighter in general I mean this seriously.

This is the unglamorous side of startups that people do not get to see all that much.

You really want to make something work and lots of other people think that it\'s a bad idea and it\'s really hard.

And everything happens much much slower than you\'d like and you\'ve sort of many late night discussions like this and sort of soul searching debates and wondering like Is this actually a good idea or maybe it is a good idea but it\'s just too hard for us to pull off and Tharp\'s are hard.

And the thing is this doesn\'t actually go away.

This is the thing I didn\'t realize before doing a startup.

I thought the two of you have all these doubts in the early days and then it was hard to take off and things would get easy.

But no matter how successful you will have lots of doubts.

The first American to win the Tour de France was a guy called Greg Lamond and he has a quote I\'ve always really liked.

It doesn\'t get easier you just get to go faster and it\'s kind of like this with startups like the startup might start going faster.

It doesn\'t really get easier.

In our case we\'ve got the pieces in place and we got to the point were ready to launch we launch on the twenty ninth of September 2011.

So just over a year ago at the time striated in predict had been in production use for 19 months and we\'ve been working on it fulltime for four year and three months.

We\'re 10 people whom we launched Eisele to fit all the names in a tweet.

And by the end of the year here\'s our daily transaction volume looks like promising but launching is definitely not a panacea.

But the signs were positive and we kept going.

And over the last few months two and a half years in stripe has finally started to become an overnight success.

Jessica talked about how startups are roller coasters and there\'s a lot of downs but there\'s also ups the next slide is our daily transaction volume through today and it looks like this.

From being for people not all that long ago stripe is now 34 people.

Which is actually twice as many people as are in this picture because everything is all behind them a start up and we haven\'t got around to taking our newgroup shot yet and many thousands of companies are using Stripe and a lot of new things go live everyday.

I mean it\'s a bunch of well-known brands like Foursquare and boxy and Hipmunk and the Afaf and New York MoMA but loved less well-known ones too.

And they actually tend to be sort of just as interesting as things like good eggs which enables you to buy directly from local farmers or Samasource which brings computer based work to people living in poverty or even stuff like the Bedford cheese shop which is now just selling its cheese online.

I guess I\'m just hungry and I\'m making these slides she seemed like a good idea.

If anyone here ever looked into the history of container shipping sir I know there\'s a bit of context for trom cheese container shipping and the shipping container like with those 40 foot shipping containers.

On some level they\'re the most mundane thing in the world and we see them around all the time but there were actually an absolutely enormous innovation 60 years ago before shipping containers transportation was a massive issue with physical goods transportation costs often accounted for up to 25 percent of the final cost of a physical item.

Overall transportation costs and shipping costs were like 10 percent of the value of all the imports in theU.S.

Think about that read 10 percent.

That means your margins 20 percent just by bringing your goods to another market.

You cut your profit in half.

So unsurprisingly most manufacturing happens at a very close to our physical price was consumed.

And so the shipping container and then in the mid 1950s essentially eliminated the cost of shipping physical goods.

It cut the costs of loading and unloading ships by 95 percent.

And it\'s now at the point for and actually cutting this from aU.S.

government report.

It\'s better to assume that moving goods is essentially costless.

Really the history here is Vaselines a few kind of good books about it.

But the point is this technological breakthrough is sort of this elimination of friction.

And in particular this abstraction over geography.

It played an enormous role in facilitating the rise of Singapore and South Korea and Taiwan and Japan and China as manufacturing hubs and my point is really that a technology that doesn\'t just monetize itself but actually enables new commerce can really enormous impact the shipping container literally reshape the world economy.

We sometimes describe we\'re doing with stripe as building economic infrastructure for the Internet.

It\'s not very flashy but for most of human history we\'ve had to buy from the people beside us.

But thanks to the Internet that\'s no longer true.

We have a new way to abstract over place.

Anyone can now build a global business.

But yet while the Internet has revolutionized how we communicate and how we collaborate and how we share we\'ve only sort of started to explore how it can change what we create and how we transact and what kind of business is possible.

And a lot of the other companies whose founders are speaking today are are pretty good examples of that thrived.

We simply want to turn payment\'s into a ubiquitous utility.

We won more commerce on the internet but it\'s still really early days and honestly most the time we\'re not thinking at these kinds of problems we\'re trying to figure out how to decrease the load on DBI 3 or trying to get some particular design just right and working through the 20th iteration or wondering if some particular product is a is a good idea or having some debate in Gmail that\'s so long We\'ve overflowed the Gemalto thread limit.

And it\'s now become a completely new thread.

It\'s all the day to day stuff.

You know it turns out that all the high level stuff the the larger motivations and and the bigger ideas and the day to day implementation like the debates and the tweaking and the iterations both of them are really addictive and that\'s why we keep doing this.

Thank you.
