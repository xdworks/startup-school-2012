**Patrick Collison at Startup School 2012-nnllRegL\_NI.mp4**

*Patrick Collison，2012年创业学校-nnllRegL\_NI.mp4*

\[00:00:00\] Morning them. Hopefully this clicker works. When I sat down
to write this talk I really racked my brains to try to figure out what
the most interesting and relevant and useful content would be for a lot
of people who were sort of interested in web startups. When I thought
about it in those terms. The topic of my talk became fairly obvious but
then. I thought about it more and the Algren doesn\'t even seem to be
deterministic. I\'m not sure anyone even knows how it works. So I guess
I\'ll actually have to talk about stripe instead. Two years ago Brian
from Airbnb Inbee spoke at Sahib\'s school. In 2010 he opened his talk
by showing a picture of Startup School in 2008. Two years previously and
that picture showed a snapshot of the audience and he picked out one
particular head. He was just sitting there and anonymous had in the
audience and I know this because I was at his talk in 2010. And so two
years later he was on stage outside of school and somehow two years
later here I am and I\'m sure there\'s at least one person here who
who\'ll be on stage in two years time and stripe definitely isn\'t as
far along as air being. But it drove home the point to you when I
realized this that startups are very unpredictable. You know software is
really hard to get your head around somebody telling me not all that
long ago that that evidence was just becoming a huge success. They were
making something like ten thousand dollars a week and we\'re thinking
man that\'s really impressive. And now I\'ve no idea what urban Ebony\'s
actual revenue figures are today but it wouldn\'t at all shock me if
they\'re making ten thousand dollars an hour. Like what Dad even liked
to try to build a company for that kind of growth is possible. Startups
are strange for a whole bunch more reasons. They\'re usually kind of
counterintuitive because they were counterintuitive. Somebody else would
probably solved the problem is already on top of that. Startups often
don\'t actually want don\'t actually want to be all that well understood
it can actually be quite helpful to be sort of under estimated and under
comprehended. But I think the biggest reason that startups are hard to
understand is that so few people still get to see them up close during
those first couple orders of magnitude. And when people do tell the
stories or from the stories are told they often tend to be kind of
wrong. They\'re about sort of rocketships and frantically holding on and
trying to add more server capacity as quickly as you can to handle the
next million users. They\'re not about the late night arguments and
wondering if your product could ever possibly work more. Trying to
figure out when you launch your product why it\'s not growing. The thing
is even the really successful startups have this phase that that famous
summer when Facebook moved out to Palo Alto in 2004. Most people don\'t
realize this but there were other people in the same house working in
other startups like this is the most successful technology company
started in the 21st century and in the same house there were people
working at a startup ideas six months after launch. It\'s it really
takes a while. And so stripe is obviously very very different to
Facebook and urban bee and nowhere near as far along as they are. But
we\'ve now gone through a small bit of growth. And so I want to try to
describe how it actually works. In October of 2009 John and I were
walking home from dinner in Potrero up in the city. I\'ve been kicking
around this idea of starting an online payments company. We\'re really
kind of fascinated by the concept of Internet payments and all the other
companies in the space seemed like total dinosaurs. And as the web sort
of spread around the world and more deeply into our lives through mobile
devices it seemed kind of obvious there should be some kind of universal
payment infrastructure for the Internet to be just really easy to
transact online. And John just turned to me he said you know while the
debate about you know what I would just go build it won\'t be all that
hard.

[00：00]早上好。希望这个按键能起作用。当我坐下来写这篇演讲的时候，我真的绞尽脑汁想弄清楚，对于很多对网络初创公司感兴趣的人来说，最有趣、最相关、最有用的内容是什么。当我用这些术语来思考这件事的时候。我演讲的主题变得相当明显，但后来。我想得更多了，阿尔金人似乎并不是决定性的。我不确定是否有人知道它是如何工作的。所以我想我得去讨论条纹了。两年前，Airbnb的布莱恩在萨希布的学校演讲。2010年，他在演讲开始时展示了一张2008年创业学校的照片。两年前，这张照片展示了观众的快照，他挑出了一个特定的头部。他只是坐在那里，匿名者在观众席上，我知道这一点，因为我在2010年参加了他的演讲。两年后，他在校外的舞台上，不知何故，两年后，我来到这里，我确信至少有一个人将在两年后登上舞台，身上的条纹绝对不像空气那么远。但当我意识到创业公司是非常不可预测的时候，我就明白了这一点。你知道，就在不久之前，软件真的很难让你了解到有人告诉我，证据只是一种巨大的成功。他们每周挣一万美元左右，我们认为这是令人印象深刻的。现在我不知道城市埃伯尼现在的实际收入数字是多少，但如果他们每小时挣一万美元，我一点也不吃惊。就像爸爸所喜欢的那样，为了这样的增长而努力建立一家公司是有可能的。创业公司很奇怪，因为还有很多原因。他们通常是违反直觉的，因为他们是违反直觉的。其他人可能会解决问题，问题已经解决了。初创企业通常不想被完全理解-实际上，被低估和被理解是很有帮助的一件事。但我认为，创业公司之所以难以理解，最大的原因是，在最初的几个数量级中，几乎没有人能近距离地看到它们。当人们讲故事或从故事中讲述时，他们往往是错误的。它们是某种程度上的火箭，疯狂地坚持和试图尽快增加更多的服务器容量，以处理下一个百万用户。他们不是关于深夜的争论，而是想知道你的产品是否还能发挥更大的作用。试图弄清楚你什么时候推出你的产品，为什么它没有增长。事实是，即使是真正成功的初创企业，也有着著名的夏季阶段，当时Facebook在2004年搬到了帕洛阿尔托(PaloAlto)。大多数人没有意识到这一点，但在同一家公司里的其他人在其他初创公司工作，这是21世纪创立的最成功的科技公司，而在同一家公司，在成立6个月后，也有人在创业点子上工作。这真的需要一段时间。因此，条纹显然与Facebook和城市蜜蜂非常不同，而且与它们相去甚远。但我们现在经历了一小部分增长。所以我想试着描述一下它是如何工作的。2009年10月，我和约翰在波特雷罗市吃完晚饭步行回家。我一直在考虑创建一家在线支付公司的想法。我们对互联网支付的概念非常着迷，而在这个领域的所有其他公司似乎都像恐龙一样。随着网络在世界各地传播，并通过移动设备深入到我们的生活中，似乎很明显，互联网应该有某种通用的支付基础设施，才能真正容易地在网上进行交易。约翰转过身来对我说，你知道，虽然关于你的辩论知道我会去建造什么，但它不会那么难。

\[00:04:00\] He actually said that if I won\'t be all that hard and so I
said okay sure why not backtracked a little bit here.

[00：04：00]他实际上说，如果我不那么难的话，所以我说，好吧，为什么不在这里退一步呢。

\[00:04:09\] John is my co-founder at stripes. He\'s ulting my brother.
And people often ask me about how this works in practice. And so for the
record started a company with your brother. Turns out to be a really
good idea. John is not only the most brilliant people I know. I think he
got the highest results in Irelands university entrance examinations but
he\'s also someone with whom I\'ve literally decades of experience
building things.

约翰是我的创立者之一。他在批评我哥哥。人们经常问我这在实践中是如何运作的。因此，为了记录在案，他和你哥哥开了一家公司。结果证明是个好主意。约翰不仅是我认识的最聪明的人。我认为他在爱尔兰的大学入学考试中取得了最高的成绩，而且他也是一个我与他一起工作了几十年的人。

\[00:04:33\] Here\'s an earlier venture that we worked on together.

[00：04：33]这是我们一起工作过的一个早期冒险项目。

\[00:04:38\] And so it\'s October 2009 we decide to work in this online
payments company. We decided to call it slash dev slash payments. The
API should be just as straightforward as any other node endeavor Fasth
were kind of OK had programming and definitely not at naming things. But
everyone else seriously have been targeting their product. They told us
a finance sector product they were targeting chief foes and business
people. And we thought the international just moving in a completely
different direction. We decided to target makers the people actually
building things. We thought that Internet payments was a technology
problem and we wanted to build a completely new stack for anybody
transacting online. So we worked nights and weekends. We were both in
college at the time I was at MIT. And John was off the road at Harvard
and so we\'d code together in the evenings between problem sets and
writing papers. January rolls around switch for both of those schools.
You sort of have that month off but of course anybody who knows Boston
knows a January in Boston is unbelievably freezing. And so we decide to
go somewhere else to work for the month. We read a few blogs that claim
the one Azarias was surprisingly a really good place to get things done.
It\'s it\'s pretty cheap it\'s really warm it\'s friendly. For some
reason I don\'t know why those Wi-Fi everywhere everything happens on a
really late schedule like the bars up until 5:00 AM nobody has dinner
until midnight and nothing starts before noon. It\'s Veazey a city on a
programers schedule. So we read all of this really great. We\'ve got to
run as our eyes. And so we did and we just worked nonstop in cafes for
three weeks. I still never seen a single one of the tourist attractions
and one Azarias or I presume they exist and then read like we could all
day and we go to dinner at 11:00 o\'clock or something and then go to
bed. I can\'t emphasize this enough if you want to get something done
consider going to an Atari\'s. On January 9. We got our first production
user for sloughed slushed such payments. Like I say it. This is only a
few weeks after we started working on it but we really wanted to get
production users shaping the product as quickly as we could. The user
was a friend of ours. I called Ross Bouchet who was working in a company
called Tweetie north at the time. Results also actually wisely funded.
Funnily enough he actually became the seventh person to work at stright
but that\'s a separate story. Here\'s a screenshot of what DIAF payment
looked like at the time and this screenshot you can see that John and I
are definitely programmers and not designers but OK. So January 9th we
now have one user. This great story from the early days of Amazon how a
celebrated when they got their first buyer who wasn\'t any of their
moms. And you know Ross wasn\'t exactly our mom but he was a good
friend. So we definitely weren\'t out of the woods just yet. So we went
back to school and we can do to work on debt payments in our spare time.
There was this one cafe that I worked out of so much they took pity on
me and I\'m still Facebook friends with a bunch of the Bristow\'s. Yeah
like strivings that kind of unusual company. We\'re about technology but
roles about payments and the technology side requires good reliability
and you know clean baby eyes and a really nice product and have lots of
technology things Wheatley\'s hoped to know something about. But the
Peyman side requires working with banks and dealing with credit card
companies and just generally handling a slew of finance industry issue
issues. We really had no new experience with no idea how to handle. We
love meetings where I sort of sat somebody down and said Right. So
payments how do they work. Programmers often and this is unfortunate
looked down at the folks who are trying to learn to code of. I want to
learn real for my web startup crowd but actually a lot of sympathy for
them because we were that bad. But in finance summer came around to of
six months and we moved out to Palo Alto though we hadn\'t actually yet
decided to take leave from school. We found a tiny bungalow just off
university and the living room and the kitchen became our office. It was
pretty hot didn\'t have any air conditioning and so John just slept in
the garden most nights wouldn\'t allow me to post a picture of this. And
by and large we just kept on writing code because I mean that\'s mostly
what sauteing a software company looks like in the early days or through
the writing code or you\'re talking to people who use the code or
you\'re wasting time. And here\'s a chart of our transaction volume over
the first six months. And that\'s not a technical error. If you look
really closely you can see a tiny little wiggly line at the bottom.
It\'s admittedly not wiggling all that much around this time though we
did have our first person join and we\'re based in Silicon Valley home
to the best international talent from Berlin to Beijing to Bangalore and
so of course we took full advantage of it. We heard a guy called Dara
Butley who was one of my smartest friends from college and he grew up in
a small town called Limerick in Ireland. About 2 miles from here John
and I grew up. Raised our first investment for our first real investment
I guess. Why see it obviously already invested. This was from from Peter
Till then we hadn\'t told very many people about DIAF payments and those
we had told had reacted mostly by telling us we were crazy. But of
course luckily Peter Teal is crazy. So he invested and it\'s been really
helpful to have him on board. Soon after that moved into our first
office which looked something like this. It\'s actually sort of said
Ramona and university and Parlato just sort of Cubitt cafe. It\'s
actually a converted house and because it was a house it had this
wonderful fireplace the world light in the winter. The fireplace looked
something like this which I think may have contravened some fire in the
workplace codes and baozi were just working nonstop. We acted to we we
became four people around this time. The first person fourth person was
a guy named Greg. I remember when Greg was sort of considering joining
and dropping out of school he asked me about our work schedule and
whether or not we worked weekends. Obviously we did work weekends but he
really didn\'t want to make this sort of scare him off and make it seem
like he\'d have to answer. So I sort of said well you know we usually
work some of the weekend we really care about work life balance and we
just cut me off means I\'m great. I\'m not on the same page and working
all day everyday. And so we knew he\'d fit in. We decide to change our
name. I can\'t even begin to list the problems that flashed such
payments had somehow it turned out that not everyone immediately got the
devil S analogy. Nobody was really able to get their head around the
whole slash thing and we started to get Mayeux with things like this.
And then there was the admittedly pretty inconvenient fact that Amazon
had launch a product an online payments product called Amazon dev pay
and so it precursory just wasn\'t going to work out and so we spent
hours brainstorming names and we eventually came up with the name stripe
and we didn\'t actually think that stripe was all that great an aim for
come up with it but we decided to just put a date in the calendar and if
we didn\'t come up with a better name by that date then we\'d stick with
stripe. And sure enough it became striped and actually a few months
later I learned that this is how Apple ended up with a name Apple with
the exact same thing. Jeremy reached the end of our first year mostly
intact. A bunch of Y Combinator companies started to use Stripe and
those was pretty good where we\'re getting some real feedback. And
here\'s another chart. This are transaction volume through the first
year. And so it\'s still kind of a ways to go. We spent January of 2011
our one year anniversary in Rio de Janeiro because January in South
America was becoming a tradition as anyone who\'s been to Rio de Janeiro
knows it\'s when most beautiful places on earth.

[00：04：38]所以2009年10月我们决定在这家在线支付公司工作。我们决定叫它斜杠开发削减付款。API应该和任何其他节点的努力一样简单，Fasth是某种程度上可以编程的，而不是在命名方面。但其他人都在认真地瞄准他们的产品。他们告诉我们一个金融部门的产品，他们的目标是主要敌人和商人。我们认为国际社会正在向一个完全不同的方向发展。我们决定把目标对准制造者-实际上是建造东西的人。我们认为互联网支付是一个技术问题，我们想为任何在线交易的人建立一个全新的堆栈。所以我们晚上和周末都工作。我在麻省理工学院的时候我们都在上大学。约翰离开了哈佛大学，所以我们在晚上一起写习题和写论文之间的代码。这两所学校的一月轮流上课。你有几个月的假期，但当然，任何知道波士顿的人都知道波士顿的一月是令人难以置信的寒冷。所以我们决定去其他地方工作一个月。我们读了一些博客，声称只有一个Azarias是一个非常好的地方来完成事情。很便宜，很暖和，很友好。出于某种原因，我不知道为什么到处都是Wi-Fi，一切都是按很晚的时间表进行的，就像酒吧直到早上5点，没有人要到午夜才吃晚饭，中午之前什么也不开始。这是维西，一个按节目编排的城市。所以我们读到了所有这些非常好的东西。我们得像眼睛一样奔跑。所以我们做到了，我们只是不停地在咖啡馆里工作了三个星期。我还从来没有见过一个旅游景点和一个阿扎里亚斯，或者我认为它们存在，然后像我们整天一样阅读，然后我们在11：00或什么时候去吃晚饭，然后睡觉。我不能强调这一点，如果你想要完成某件事，可以考虑去Atari‘s。1月9日。我们得到了我们的第一个生产用户的落水，这样的付款。就像我说的。这是仅仅几个星期后，我们开始工作，但我们真的想让生产用户尽快塑造产品。用户是我们的朋友。我打电话给罗斯·布切特，他当时在一家叫Twetie North的公司工作。结果实际上也得到了明智的资助。有趣的是，他实际上成了第七个在斯特赖特工作的人，但那是另外一个故事。这是一个关于diaf付款的截图，这个截图你可以看到，约翰和我绝对是程序员，不是设计师，但没问题。所以1月9日我们有了一个用户。这个伟大的故事发生在亚马逊的早期，当他们找到第一个不是妈妈的买家时，他们是多么有名。你知道罗斯不是我们的妈妈，但他是个好朋友。所以我们肯定还没脱离险境。因此，我们回到学校，我们可以做的工作，在我们的业余时间偿还债务。有一家咖啡馆是我工作的地方，他们很同情我，而我仍然是一群布里斯托的Facebook好友。是啊，就像拼搏，那种不寻常的公司。我们是关于技术的，但是关于支付和技术方面的角色需要很好的可靠性，你知道干净的婴儿眼睛和一个非常好的产品，并且有很多技术的东西，Wheatley希望了解一些东西。但佩曼方面要求与银行合作，与信用卡公司打交道，一般只需处理一系列金融业问题。我们真的没有新的经验，不知道如何处理。我们喜欢让我坐下来说对的会议。所以支付是如何运作的。程序员经常-这是不幸的-瞧不起那些试图学习代码的人。我想学习真实的我的网络创业人群，但实际上很多同情他们，因为我们是那么糟糕。但在金融界，夏天已经过去了六个月，我们搬到了帕洛阿尔托，尽管我们还没有决定从学校休假。我们在大学附近发现了一间小平房，起居室和厨房成了我们的办公室。天气很热，没有空调，所以约翰大部分晚上都睡在花园里，不允许我贴这张照片。总的来说，我们只是继续编写代码，因为我的意思是，这主要是软件公司早期的样子，或者是通过编写代码，或者你在和使用代码的人交谈，或者你在浪费时间。这是我们前六个月交易量的图表。这不是技术上的错误。如果你仔细观察，你会看到底部有一条小小的摇摆线。诚然，在这段时间里，我们并没有摇摆不定，尽管我们确实有第一人加入，我们总部位于硅谷，拥有最好的国际人才，从柏林到北京，再到班加罗尔，我们当然充分利用了这一点。我们听到一个叫达拉·布特利的家伙，他是我大学里最聪明的朋友之一，他在爱尔兰的一个叫利默里克的小镇长大。离这里大约2英里，我和约翰长大了。为我们的第一笔真正的投资筹集了我们的第一笔投资。为什么看到它显然已经投资了。这是彼得·蒂尔写的，当时我们并没有告诉很多人有关节食付款的事情，而我们告诉过的那些人的反应主要是告诉我们疯了。当然，幸运的是彼得·提尔疯了。所以他投资了，让他上飞机真的很有帮助。在那之后不久，我们的第一间办公室就变成这样了。实际上，拉莫纳、大学和帕拉托只是一种立体咖啡馆。它实际上是一座改造过的房子，因为它是一座房子，它有一个美妙的壁炉-冬天的世界之光。壁炉看起来像这样，我认为这可能违反了工作场所的一些规定，而且包子只是不停地工作。我们这个时候变成了四个人。第一人称第四人是一个叫格雷格的人。我记得格雷格在考虑加入和辍学的时候，他问我们的工作时间表，以及我们周末是否工作。很明显，我们周末确实工作过，但他真的不想让这种事吓跑他，让人觉得他必须回答。所以我说，嗯，你知道，我们通常在周末工作，我们真的很关心工作和生活的平衡，我们只是切断了我的关系，这意味着我很棒。我已经不一样了，每天都在工作。所以我们知道他会加入。我们决定改名。我甚至不能开始列出那些闪现这种付款的问题，如果事实证明不是每个人都立即得到了魔鬼S的类比的话。没有人真的能把他们的头绕在这整条斜线上，而我们开始用这样的东西来对付Mayeux。还有一个不可否认的非常不方便的事实，那就是亚马逊已经推出了一款名为Amazondev Pay的在线支付产品，所以它的先兆是不可能实现的，所以我们花了几个小时的头脑风暴名字，最终我们想出了stripe这个名字，我们并不认为这个stripe是想出它的伟大目标，但我们决定了。只要在日历上放一个日期，如果我们没有在那个日期之前想出一个更好的名字，我们就会坚持使用条纹。果然，它变成了条纹，实际上几个月后，我了解到，这就是苹果的最终名称-苹果的名字与之完全相同。杰瑞米到了第一年年底，基本上完好无损。一群Y组合公司开始使用Stripe，在这里我们得到了一些真正的反馈。这是另一张图表。这是第一年的交易量。所以这仍然是一段路要走。2011年1月，我们在里约热内卢度过了一周年纪念日，因为南美洲的一月正成为一种传统，任何去过里约热内卢的人都知道，这是世界上最美丽的地方。

\[00:12:11\] And of course we took full advantage of it.

[00：12：11]我们当然充分利用了它。

\[00:12:18\] At this point we\'re an invite only private beta and so
there probably is something obvious we could have done to grow at least
a little bit faster are you to launch a friend refers to invite only
private beta as the baby blankets of startups. And I think that\'s about
right. But the beta period was actually really helpful to stripe and
were Paul Buchheit saying that should start out by making hundred people
really happy rather than many more people. Only a little bit happy you
really took this to heart and took advantage of the small number of
users to really focus on them as much as we could and really try to
figure out what they wanted. Forgiveable not long after we launch the
first version of strife we had a Peter duty so we\'d all get called from
the site with down pretty standard and pretty reasonable. But then we
realized that any time a user gets any kind of error or like even if the
site is down that\'s actually a really bad experience for them and we
could probably make them much happier if we went and investigated the
error and sort of proactively reach out to them and help them fix it.

[00：12：18]在这一点上，我们只是一个私人的测试版，所以很明显，我们可以做一些事情，至少能更快地成长，你会不会把一个朋友当作初创公司的婴儿毯子来邀请私人测试版？。我认为这是正确的。但测试期实际上对条纹很有帮助，保罗·布切特(PaulBuchheit)曾说过，这应该从让一百人真正快乐开始，而不是让更多人快乐。只是有点高兴，你真的把这个放在心上，利用少数用户的优势，真正关注他们，尽可能多，并真正地试图找出他们想要什么。可原谅后不久，我们推出了第一个版本的冲突，我们有一个彼得的职责，所以我们都会被打电话从网站上下来，相当标准和相当合理。但后来我们意识到，每当用户遇到任何错误，甚至是网站瘫痪时，这对他们来说都是一次非常糟糕的体验。如果我们去调查错误，主动地联系他们，帮助他们解决错误，我们可能会让他们更开心。

\[00:13:14\] And so we changed the code a little bit so that any time
anyone hit any error it would send an e-mail that would go sort of
straight the top of everybody\'s inbox and I would also phone everybody
and we\'d go and fix it no matter what. And I really mean that I would
get out of bed if necessary. We\'re basically never without a laptop and
the means to tether. Here\'s a photo of one such incident. This is Greg
and I have gone to the cinema in Redwood City a user encountered an
error. And so of course out came our laptops and we had to go fix it. I
think Greg I think Greg is here so much.

[00：13：14]所以我们对代码做了一点改动，每当任何人遇到任何错误时，它都会发送一封电子邮件，这种邮件会直接发送到每个人的收件箱顶部，我也会给每个人打电话，不管发生什么，我们都会去修复它。我的意思是如果必要的话我会起床的。我们基本上从来没有笔记本电脑和捆绑的手段。这是一张这样的事件的照片。这是格雷格和我去了雷德伍德市的电影院，一个用户遇到了一个错误。所以，当然，我们的笔记本电脑出来了，我们必须去修理它。我想格雷格经常来这里。

\[00:13:46\] I mean I think he still feels a little bit bitter about
missing the start of the movie over this movie may or may not have been
Twilight Breaking Dawn start after high stress you need to unwind.

[00：13：46]我的意思是，我认为他仍然对错过这部电影的开头感到有点痛苦，因为这部电影可能是或可能不是“暮光之城”，黎明开始于你需要放松的高度压力之后。

\[00:14:00\] We also realize that ending with an engineer is basically
the best support experience possible. Like it\'s really frustrating to
have to go into to file a ticket and find the support email address and
then wonder does this come to reply to those who bought e-mails or if
they do reply. How long does it take them or all of these issues. Like
it\'s much nicer you can just start sort of directly chatting with
somebody. And it\'s also way more productive for us because we can then
go and sort of try to figure out what the underlying issue is rather
than having to sort of guess based on the user\'s initial description.
So we just opened up this chat system on our Web site where anyone can
jump in and just start asking questions and we actually still have this
today and that was it was really good but then we thought why stop
there. Isn\'t it really a really bad experience when somebody asks a
question and there\'s nobody there to answer them. And so we a hot pager
duty. And so we hooked it up so that if you asked a question in the
Streib chat room and there was nobody there to answer you it would go
and phone one of us after 30 seconds. And so I don\'t think many of you
will know this but like for many months that stripe if you asked a
question in our chat room there\'s no one there to answer someone would
be woken up if necessary to help you.

[00：14：00]我们也意识到，以工程师为结尾基本上是最好的支持经验。就像它真的很令人沮丧，必须要去提交一张罚单，找到支持的电子邮件地址，然后想知道这是来回复那些购买电子邮件的人，或者如果他们真的回复。他们需要多长时间或者所有这些问题。更好的是，你可以直接和别人聊天。这对我们来说也更有效率，因为我们可以尝试找出潜在的问题是什么，而不是根据用户的初始描述进行猜测。所以我们刚刚在我们的网站上打开了这个聊天系统，任何人都可以跳进来问题，实际上我们今天仍然有这个，这是真的很好，但是我们想为什么停在那里。当有人问题，却没有人回答问题时，这难道不是一次非常糟糕的经历吗？所以我们要负责传呼。所以我们把它连接起来，如果你在Streib聊天室问了一个问题，没有人回答你，30秒后，它会给我们中的一个人打电话。所以我不认为你们中的很多人会知道这一点，但就像几个月以来，如果你们在我们的聊天室问了一个问题，没有人会回答，如果有必要的话，他们会被唤醒来帮助你。

\[00:15:02\] We don\'t do that today.

[00：15：02]我们今天不这么做。

\[00:15:07\] So those strike wasn\'t yet publicly available to everyone.
We really tried to sort of turn up the dial on our users feedback and to
force ourselves to be extremely sensitive to what they wanted and what
their experience was like. We our users talking to us during every
waking hour. And if anything went wrong for them they were like
literally interrupting our sleep. The other thing that comes in bated
was the fact we weren\'t just building a fin software layer. We thought
that stripes would encompass everything from the API requests to have
the money ended up in your bank account and we wanted to able to define
the experience. And we wanted to be able to do it at scale. We were
really influenced by things like Amazon Web Services and easy to watch.
It\'s really interesting innovation because you see two is fantastic
you\'re a smaller company or a startup startup or a side project or
something like this but it scales right through to be a Netflix or a
Zynga or indeed an Amazon.

[00：15：07]所以那些罢工还不是每个人都能看到的。我们真的试着打开用户反馈的刻度盘，强迫自己对他们想要的东西和他们的体验非常敏感。在每个清醒的时间里，我们的用户都在和我们交谈。如果他们出了什么问题，他们就像是打断了我们的睡眠。另一件事是，我们不仅仅是在构建一个FIN软件层。我们认为条形码将包含从API请求到将钱放在您的银行帐户中的所有内容，我们希望能够定义这种体验。我们想要在规模上做到这一点。我们确实受到像AmazonWebServices这样的东西的影响，而且很容易观看。这是一个非常有趣的创新，因为你看到两个很棒，你是一个较小的公司，一个创业公司，一个类似的项目，但它一直延伸到一个Netflix，一个Zynga，甚至亚马逊。

\[00:15:58\] It\'ll work for a company of any size and we decided we
wanted to do that. But for internet payment infrastructure we wanted to
make something that was really easy to start with but something would
also work for the largest companies in the world. Until that meant
working with really good banks. The problem is that banks and startups
are basically the business equivalent of oil and water and figuring out
how to combine them is pretty hard. The best bank in the business is
like Wells Fargo which powers some of the largest payments companies in
the world and almost it was pretty tough to get them to talk to us or
even to return our e-mails. Their price hardware some strange kind of
Nigerian scam like Make Money Online Fast from the comfort of your own
home. So we asked a friend an investor and now a partner at Y
Combinator. Jeff Ralston to help out. Jeff had previously been CEO of a
company called Lalah an online music startup and they had negotiated
successfully with the record labels and we thought that if you could as
a technology startup negotiate successfully with the record labels you
could basically convince anyone in the world to do anything ever. And
here\'s a picture of Jeff on a conference call with Wells Fargo. That\'s
Dhara. They\'re on the other side and you might wonder why is Jeff on
the floor. Well Jeffrey on the floor. Because our office was also
flooded at the time. We also had a security audit that day sometimes
trucks are just like a reality TV show. It\'s like negotiate with one of
the biggest banks in the world. While Undergoing a security audit while
wading through water and the water is full of Trina\'s or something. But
thanks to Jeff and a bunch of others we eventually convinced Wells Fargo
to become one of our backhands in moving all of our systems to work out
of their platform. It was a couple of weeks of honestly really intense
work we had to hit a particular deadline. This is the night of our first
successful transaction. This is John after another particularly long all
nighter in general I mean this seriously. This is the unglamorous side
of startups that people do not get to see all that much. You really want
to make something work and lots of other people think that it\'s a bad
idea and it\'s really hard. And everything happens much much slower than
you\'d like and you\'ve sort of many late night discussions like this
and sort of soul searching debates and wondering like Is this actually a
good idea or maybe it is a good idea but it\'s just too hard for us to
pull off and Tharp\'s are hard. And the thing is this doesn\'t actually
go away. This is the thing I didn\'t realize before doing a startup. I
thought the two of you have all these doubts in the early days and then
it was hard to take off and things would get easy. But no matter how
successful you will have lots of doubts. The first American to win the
Tour de France was a guy called Greg Lamond and he has a quote I\'ve
always really liked. It doesn\'t get easier you just get to go faster
and it\'s kind of like this with startups like the startup might start
going faster. It doesn\'t really get easier. In our case we\'ve got the
pieces in place and we got to the point were ready to launch we launch
on the twenty ninth of September 2011. So just over a year ago at the
time striated in predict had been in production use for 19 months and
we\'ve been working on it fulltime for four year and three months.
We\'re 10 people whom we launched Eisele to fit all the names in a
tweet. And by the end of the year here\'s our daily transaction volume
looks like promising but launching is definitely not a panacea. But the
signs were positive and we kept going. And over the last few months two
and a half years in stripe has finally started to become an overnight
success. Jessica talked about how startups are roller coasters and
there\'s a lot of downs but there\'s also ups the next slide is our
daily transaction volume through today and it looks like this. From
being for people not all that long ago stripe is now 34 people. Which is
actually twice as many people as are in this picture because everything
is all behind them a start up and we haven\'t got around to taking our
newgroup shot yet and many thousands of companies are using Stripe and a
lot of new things go live everyday. I mean it\'s a bunch of well-known
brands like Foursquare and boxy and Hipmunk and the Afaf and New York
MoMA but loved less well-known ones too. And they actually tend to be
sort of just as interesting as things like good eggs which enables you
to buy directly from local farmers or Samasource which brings computer
based work to people living in poverty or even stuff like the Bedford
cheese shop which is now just selling its cheese online. I guess I\'m
just hungry and I\'m making these slides she seemed like a good idea. If
anyone here ever looked into the history of container shipping sir I
know there\'s a bit of context for trom cheese container shipping and
the shipping container like with those 40 foot shipping containers. On
some level they\'re the most mundane thing in the world and we see them
around all the time but there were actually an absolutely enormous
innovation 60 years ago before shipping containers transportation was a
massive issue with physical goods transportation costs often accounted
for up to 25 percent of the final cost of a physical item. Overall
transportation costs and shipping costs were like 10 percent of the
value of all the imports in theU.S. Think about that read 10 percent.
That means your margins 20 percent just by bringing your goods to
another market. You cut your profit in half. So unsurprisingly most
manufacturing happens at a very close to our physical price was
consumed. And so the shipping container and then in the mid 1950s
essentially eliminated the cost of shipping physical goods. It cut the
costs of loading and unloading ships by 95 percent. And it\'s now at the
point for and actually cutting this from aU.S. government report. It\'s
better to assume that moving goods is essentially costless. Really the
history here is Vaselines a few kind of good books about it. But the
point is this technological breakthrough is sort of this elimination of
friction. And in particular this abstraction over geography. It played
an enormous role in facilitating the rise of Singapore and South Korea
and Taiwan and Japan and China as manufacturing hubs and my point is
really that a technology that doesn\'t just monetize itself but actually
enables new commerce can really enormous impact the shipping container
literally reshape the world economy. We sometimes describe we\'re doing
with stripe as building economic infrastructure for the Internet. It\'s
not very flashy but for most of human history we\'ve had to buy from the
people beside us. But thanks to the Internet that\'s no longer true. We
have a new way to abstract over place. Anyone can now build a global
business. But yet while the Internet has revolutionized how we
communicate and how we collaborate and how we share we\'ve only sort of
started to explore how it can change what we create and how we transact
and what kind of business is possible. And a lot of the other companies
whose founders are speaking today are are pretty good examples of that
thrived. We simply want to turn payment\'s into a ubiquitous utility. We
won more commerce on the internet but it\'s still really early days and
honestly most the time we\'re not thinking at these kinds of problems
we\'re trying to figure out how to decrease the load on DBI 3 or trying
to get some particular design just right and working through the 20th
iteration or wondering if some particular product is a is a good idea or
having some debate in Gmail that\'s so long We\'ve overflowed the
Gemalto thread limit. And it\'s now become a completely new thread.
It\'s all the day to day stuff. You know it turns out that all the high
level stuff the the larger motivations and and the bigger ideas and the
day to day implementation like the debates and the tweaking and the
iterations both of them are really addictive and that\'s why we keep
doing this. Thank you.


[00：15：58]它将为任何规模的公司工作，我们决定这样做。但对于互联网支付基础设施，我们想要做的东西，是真的很容易开始，但也会对世界上最大的公司工作。直到这意味着要和真正好的银行合作。问题是，银行和初创企业基本上相当于石油和水，要想把它们结合起来是相当困难的。业务中最好的银行是富国银行(WellsFargo)，富国银行为世界上一些最大的支付公司提供了动力，几乎很难让它们与我们交谈，甚至很难回复我们的电子邮件。他们的价格，硬件，一些奇怪的尼日利亚骗局，像网上赚钱快速从您自己的舒适的家。于是我们问了一位朋友，一位投资者，现在是YCombinator的合伙人。杰夫·拉斯顿来帮忙。杰夫以前是一家名为Lalah的在线音乐初创公司的首席执行官，他们成功地与唱片公司进行了谈判。我们认为，如果你能作为一家技术初创企业，成功地与唱片公司谈判，你基本上可以说服世界上的任何人做任何事情。这是杰夫和富国银行电话会议的照片。那是达哈拉。他们在另一边，你可能会想为什么杰夫在地板上。杰弗里躺在地上。因为我们的办公室当时也被淹了。那天我们还进行了一次安全审查，有时卡车就像真人秀一样。这就像和世界上最大的银行之一谈判一样。当你在水中涉水时进行安全审计时，水中充满了Trina‘s之类的东西。但多亏了杰夫和其他一些人，我们最终说服富国银行成为我们的反手之一，把我们所有的系统都移出了他们的平台。这是几个星期的真诚的紧张工作，我们必须在一个特定的最后期限。这是我们第一次成功交易的夜晚。这是约翰，一个接一个，通宵，我的意思是认真的。这是创业公司平淡无奇的一面，人们看不了那么多。你真的想让一些东西发挥作用，很多人认为这是个坏主意，而且真的很难。每件事发生的速度都比你想象的要慢得多，你像这样在深夜里讨论了很多次，还想知道这到底是个好主意，还是一个好主意，但对我们来说太难了，而Tharp的想法也很难。问题是这件事并没有消失。这是我在创业之前没有意识到的。我以为你们两人在最初的日子里都有这些疑虑，然后很难摆脱，事情会变得容易。但无论你多么成功，你都会有很多疑问。第一个赢得环法自行车赛的美国人是一个叫格雷格·拉蒙德的人，他有一句我一直很喜欢的话。它不会变得更容易，你只要走得更快，就像这样，初创公司可能会更快地发展起来。这并不是很容易。在我们的例子中，我们已经做好了准备，准备在2011年9月29日发射。所以就在一年多以前，在预测的时候，我们已经投入生产使用了19个月，我们已经全职工作了四年零三个月。我们是10个人，我们推出了Eisele，把所有的名字都放在推特上。到今年年底，我们每天的交易量看起来很有希望，但推出肯定不是万灵药。但迹象是积极的，我们继续前进。在过去的几个月里，两年半的条纹终于开始在一夜之间取得成功。杰西卡谈到了创业公司是如何过山车的，有很多的下降，但也有上升，下一次下滑是我们今天的每日交易量，看起来是这样。就在不久以前，条纹已经是34个人了。这实际上是这张照片中人数的两倍，因为一切都在他们的背后，我们还没来得及尝试我们的新团队，成千上万的公司都在使用Stripe，每天都会有很多新的东西出现。我的意思是，这是一群知名品牌，如Foursquare和Boxy，Hipmunk，Afaf和纽约现代艺术博物馆，但也喜欢不太知名的人。事实上，它们和好鸡蛋一样有趣，它可以让你直接从当地农民那里购买，或者把电脑工作带给生活贫困的人，甚至像贝德福德奶酪店，它现在只是在网上销售奶酪。我想我只是饿了，我在做这些幻灯片-她看起来是个好主意。如果说这里有谁研究过集装箱运输的历史，先生，我知道这里有一些关于特伦奶酪集装箱运输的背景，还有像40英尺集装箱那样的集装箱。在某种程度上，它们是世界上最平凡的东西，我们一直都看到它们，但在60年前，在集装箱运输成为一个巨大问题之前，我们确实有了一项巨大的创新，实物运输成本往往占到实物最终成本的25%。总体运输成本和运输成本大约是美国所有进口商品价值的10%。想想看，这个数字是10%。这意味着，你的利润20%，只要把你的产品带到另一个市场。你把利润减半了。因此，毫不奇怪，大多数制造业发生在一个非常接近我们的实物价格被消费。因此，集装箱运输，然后在20世纪50年代中期，实质上消除了运输实物货物的成本。它使船舶装卸成本降低了95%。现在，美国政府的一份报告已经将这一事实删掉了。最好假设货物运输基本上是无成本的。真的，这里的历史就是关于它的几本好书。但关键是这个技术上的突破是某种程度上消除了摩擦。尤其是对地理的抽象。它在促进新加坡、韩国、台湾、日本和中国作为制造业中心的崛起方面发挥了巨大的作用。我的观点是，一种不仅能使自身货币化，而且实际上能够实现新商业的技术，能够对航运集装箱真正重塑世界经济产生巨大影响。我们有时会把我们的做法描述为互联网建设经济基础设施。这并不是很华而不实，但在人类历史的大部分时间里，我们不得不从我们身边的人那里买东西。但多亏了互联网，\不再是真的了。我们有了一种抽象概念的新方法。现在，任何人都可以建立一家全球性的企业。然而，尽管互联网已经彻底改变了我们的沟通方式、协作方式和共享方式，但我们只是开始探索它如何改变我们的创造和交易方式，以及什么样的业务是可能的。许多创始人今天发表讲话的其他公司都是这方面的一个很好的例子。我们只是想把支付变成一种无处不在的实用工具。我们在互联网上赢得了更多的商业，但它还真的还处于早期阶段，而且老实说，大多数时候我们并不是在考虑这些问题，我们试图找出如何减少dbi 3的负载，或者试图得到一些正确的特定设计，并在第20次迭代中工作，或者想知道某个特定的产品是否是一个好主意，还是有一些争论。在Gmail中，我们已经超过了Gemalto线程的限制。现在它变成了一个全新的线索。日复一日的事情。你知道，所有高层次的东西，更大的动机，更大的想法，以及日复一日的实现，比如辩论、调整和迭代，都是令人上瘾的，这就是我们一直这样做的原因。谢谢。

