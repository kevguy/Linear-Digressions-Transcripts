| Person | Transcripts |
| :-- | :-- |
| Katie: | Hey Ben. |
| Ben: | Hey...hey Katie. Normally I say that. |
| Katie: | Yeah, we're going Freaky Friday with this one, you get to be the … you get to be the smarty pants in this episode and say something technical to me. |
| Ben: | I haven't prepared, this is… we’ve done 77 episodes I think at this point. |
| Katie: | Sounds right. |
| Ben: | We've... we've never started with “Hey Ben.”. |
| Katie: | That also sounds accurate. |
| Ben: | So... I'm wondering if you want to say the thing. |
| Katie: | Oh… oh… oh yeah, okay, sure. |
| Ben: | Say the thing, Katie. |
| Katie: | Okay, okay. You're listening to Linear Digressions. |
| Katie: | How did I do? Was that okay? |
| Ben: | Yeah, you did great, good job. |
| Katie: | This podcast topic is something that I found myself wondering about this week and I was like, “Hey, I know somebody who knows all about this, it’s Ben.” So why don’t you take it from there? |
| Ben: | Cool, yeah. Today’s podcast topic is very meta. We're talking about podcasting, and how podcasts work. We're going to... it's going to be a little bit lighter on the data science machine learning kind of stuff, we will get to a little bit of that and talking about what to do when you don't have a lot of data may be, which, as it turns out, when it comes to podcast, as a publisher you really don't get very much data. But yeah, we'll just... I guess we’ll do a whirlwind tour and talk about how one makes some podcast. |
| Katie: | Or peek behind the curtain if you will. |
| Ben: | Peek behind the curtain. So right now, I’m sitting in a room in my house, and it's very hot in this room cuz I've got the windows shut and everything, and probably you have the same thing too. This is... this is where the... I don’t know, how the sausage is made, not very romantic, but what we do is both of us record our side of it, right? So I can see my voice being recorded here, and you know, Katie, you can see your voice recorded in front of you, and we’re on a Skype call. |
| Katie: | Right. So we can hear each other through the Skype call but each of us is just recording one side of the conversation so... my… I am watching the sound wave as I'm recording right now and there's a big empty spot and that's where you're talking. I have it in my headphones so it's not getting sorta feed back into the mic but then, obviously they're sort of two halves of conversation and that needs to be reconciled somehow. |
| Ben: | Right, and the reason we do it this way is because... if I was recording all of it for example, I get very high quality of me and I get bad quality… I get the Skype call Quality of you, Katie, so... so yeah, once we're done with this episode, we will both put our halves into a shared Dropbox folder, I’ll pull both of those files in, I’ll mix them them, do a little bit of stereo stuff. So if you're listening in headphones, you can kind of hear me in the right channel a little bit more, and Katie's in the reft Channel. And also, whenever weird things happen, like a helicopter went by in the last episode that we recorded... so... we mark a little thing and then we can remove sounds like that, especially if the other person’s talking during it. |
| Katie: | Yep, so and then I take that sort of the combined file… |
| Ben: | The commerged file. |
| Katie: | Yeah, the merged file. But it’s still pretty raw and there's usually some places where we have to stop and think about something, or we’ll maybe... have to rephrase that a couple times and so there's a little bit of light editing that has to be done and also we had to add the intro and outro that sort of thing. And then I upload it to SoundCloud and then magic happens. |
| Ben: | (laughs) Magic happens. |
| Katie: | And somehow, somehow it goes from my computer out into all corners of the world and... also relatedly, I sometimes, I get a little bit of information back from SoundCloud about how many downloads we got for each episode and like... by time how well is each episode’s doing this sort of thing, which I… you know, sometimes I look at cuz they're kind of fun to watch and to think about and to try to get a little bit of feedback sort of indirectly on... on how we're doing sort of through our stats. And so I was realizing this week that I have no idea or I have only the lightest of ideas how this actual distribution process works and then also especially how the data comes back the other way, I can imagine me just sending files out into the ether but the fact that there's then a feedback mechanism to tell me sort of... who’s downloading those files and... and in what quantities that is something that I find very interesting. |
| Ben: | So, it all starts with that upload to SoundCloud. And the reason we use SoundCloud is that SoundCloud has a feature which will automatically publish a podcast for you. Now we could do this all manually and it would be a little bit of a pain in the butt, but it's totally doable and actually I do another podcast, if you're interested in kind of these more technical explanations of not data science topics, it's called GeekSpeak. That's one word, and if you search iTunes or if you go to GeekSpeak.org, you can subscribe there. When that show first started podcasting, actually I think it started podcast that it was the first... tech show... that we know of this start the podcast thing as it started podcasting before Leo Laporte's show which claims to be the first one that was podcasting, so that's kind of fun. But we would... we would write the XML file ourselves. Now what's the XML file? XML file is basically a file that says, “Hey, these are all the episodes. Here is what they're called. Here's the author. Here's the description that you’re seeing your little podcatcher or in iTunes or whatever. And here is a URL, and if you go to that URL, you can download the audio, so you can download the MP3 file. |
| Katie: | So the XML is all the metadata, and sort of tells you what's going on, and then, but the actual heavy duty file itself is something that you go download from some place once you get sort of the instructions to do so from an XML file. |
| Ben: | Right, the XML is not only the metadata. I guess it's kind of the… it's just the data of the episode as an entity but the actual recording that... you know, that... that everybody is listening to in their earphones and on speakers right now, that's actually coming from a different source. So the... so here's what happens: SoundCloud is the place where all of our MP3 files live. So if you want to go and directly download any of our episodes, you can do that directly by going to soundcloud.com and using their interface or, you can look at the RSS feed and you can find those URLs and you can just download them. |
| Katie: | Wait, what's the difference between the RSS feed and the XML file? |
| Ben: | Oh, excuse me, sorry. RSS is a code word for XML as it pertains to publishing. |
| Katie: | Oh, okay. |
| Ben: | And as it turns out, RSS actually stands for Rich Site Summary, which used to be RDF Site Summary, blah blah blah... but a lot of people say that it's called Really Simple Syndication, because it's supposed to be a really simple way of taking some kind of syndicated content like a publication, this could be a news website if you wanted to, it could be a podcast, it could be a vlogcast, which is a video podcast, and you can publish this file and it's encoded in the XML format. And that tells whoever is consuming this content where to find all of these things. |
| Katie: | Okay. So the reason that I was thinking about this earlier this week, then maybe you can shed some light is... there's all these aggregators that seem to be places where these RSS feeds get collected and then I'm thinking of things like iTunes but there's also Stitcher and I don't know... there's probably a whole bunch of them that I'm not as familiar with. And those little places are where you actually go to search for podcasts, and they can you tell you what's out there and and you can sometimes listen to them or download them or what have you. And so it always just seemed like a sort of magic that you put your... you put your RSS feed kind of in the right place and this was something that you did when we first started up this podcast, so it always seems like a little bit of black magic to me, but you put your RSS in the right place and then just like boom, it's... it's all the places where it's supposed to be. One of our listeners asked if we could put it on Google Play and I was a little bit like, “Huh, that's funny. I didn't realize that there were major aggregators that we weren't on, so to speak, that it didn't get just magically picked up the way that all the... it seems to be picked up by all these other things. I guess thinking back a little bit, when we first went on iTunes, I think there was also a process that we had to go through, I think… I remember that we had to wait a day or two for some approvals to go through and get officially added to the iTunes Store. So it seems to be not just this aspect of we're going to create this RSS feed and then put it out into the world but there's also the services that people seem to use a lot have also sometimes this curation aspect to them or you have to go in and manually start of push it forward to you know... just some of these like bigger aggregation sites or publication sites or... I don't even know what you call it, but yeah… |
| Ben: | Yeah, yeah, now I see your point, it’s the “How does anyone actually find this RSS feed that I created?” So I'm going to take a brief step back, and I'll answer that question in just one second. SoundCloud because they provide that make-a-podcast feature, when we upload things because it knows that they're part of our podcast, it'll create that X... that… RSS file... XML file, or RSS feed for us but then, there's actually another tool which we put in between, and it's called FeedBurner and it's free, and I think... I think Google runs it. And basically what it'll do is it'll say, “Okay, if you point me to an XML file... an RSS file... RSS feed, I'll take that file in, do some extra awesome cool stuff with it, like make it really optimized for iTunes, make it have all of this additional metadata, and also do some analytics and tracking for you. And then the thing that you point everyone else to, that thing that you put iTunes to, is your FeedBurner XML file. So, in a nutshell, we've got SoundCloud, we upload a file, SoundCloud makes an XML file which has a bunch of metadata of where to find this thing. FeedBurner says, “Oh hey, you update the SoundCloud XML file, let’s check every like 4 hours or something. I'll just bring them this new version, add all of this cool stuff to make it even better and... and track things for you.” And then iTunes says, “Oh hey, that FeedBurner XML file, that URL for Linear Digressions feed, that got updated. So we're going to pull in the new XML file” And then, your iPhone says, “Oh hey, iTunes, have you... like do you have any updates for me for any of the podcasts that I subscribe to?” And iTunes says, “As a matter of fact I do, here's the newest RSS feed, go download whatever you want to download.” So that's... that's the full... I guess the full pipeline right? But like you said they're all of these other aggregators right? |
| Katie: | So, let me… before we get there, just so I understand, so then when... when I click on my iPhone I say yes, download, what it does is in the same way that we have sort of this message that gets passed along in one direction when I publish, when I download, I tell iTunes, “Please download.” and then iTunes, I'm assuming it'll tell FeedBurner, “Please get this for me.” and then FeedBurner… |
| Ben: | No… |
| Katie: | No? |
| Ben: | Actually no… |
| Katie: | No? Okay. |
| Ben: | Because the XML file has the URL of where this file lives. |
| Katie: | Oh, so I go straight to SoundCloud? |
| Ben: | Yeah. |
| Katie: | Oh… |
| Ben: | Yeah... yeah, so... so this XML file that says this is where the stuff is gets passed from entity to entity to entity to entity, and then when you eventually get it on your device, your device says, “Oh, just go to the URL that's in the... in the thing.” You don't have to go all the way back around. And the benefit of this is that MP3 files are big, right? |
| Katie: | Yeah. |
| Ben: | And XML files are very small. Now if you go... when you actually open one up and try to read it, it looks really really long, it doesn't look so small, but trust me, it is way way smaller than... than the file that is bringing you the sound of our voices right now. So, this means that things like FeedBurner can operate and you can basically use it for free because it doesn't have any bandwidth costs, it's just passing XML files around rather than piping MP3 traffic back and forth for everything. |
| Katie: | Okay. |
| Ben: | So, let's just touch on the aggregator thing. There're all of these different websites that want people to subscribe to your podcast or find your podcast through them. So Stitcher is a good one, right? You can download their app, actually don't know what the monetization model is, but they may have a paid version of the app, they may show you ads, I'm not really sure. But all of these different players have incentive to try to get themselves in between the listener, the… the soon-to-be listener, and the podcast creator. And because the XML files are just out there, they can just go around and try and scoop up all the XML files that they possibly can find, and put them in a nice pretty web page and then try to get people to go to that web page to download GeekSpeak or Linear Digression or RadioLab or whatever it is, rather than going directly to our website. And actually they do provide a service. Yhey provide basically the same service that iTunes provides, and also the same service that Google Play provides, which is that if I want to download... let's say I get a new phone, and I want to download Radiolab, I want to download Linear Digressions, GeekSpeak, Song Exploder, that's another really good one. |
| Katie: | Oh that’s a good one. |
| Ben: | Yeah, and let's say it’s American Life, okay? So those five podcasts. So I can go and I can subscribe to them manually, one by one, by going to their websites and finding the little link that says Feed URL here or whatever they call it, copy that URL, put it into my podcast app, whether that's on my computer or my phone or whatever, and I can basically just subscribe directly that way, but it's a pain in the butt, right? So if you have an aggregator, which has all of my favorite podcasts in one place and a nice search feature and a little quick... you know, one click button to subscribe, that's really compelling. And that's why iTunes exists, that's why all of these other entities exists... exist, and that's why Google play or Google has been getting into this with Google Play, because they want to be that one-stop shop for all of your music needs and they do books and all that other stuff and podcasts. |
| Katie: | Okay, and so... just so... I understand. So I think I remember going through the process of getting this approved for iTunes, I went through the process of getting us on Google Play this week, it was really easy but there was obviously a little bit of a review stuff in there. Did we ever have to go through some kind of review process like that for Stitcher? Do you remember? I'm just curious. |
| Ben: | I do actually. Stitcher... funny enough, Stitcher emailed me. |
| Katie: | Oh… okay. |
| Ben: | And said, “Hey, do you want to be on our website?” And the only reason I said yes is because I've heard their ads everywhere, and I figure if I'm hearing their ads everywhere, then probably... a bunch of other people are hearing their ads and probably subscribing to podcasts through them, so you know... I might as well be. |
| Katie: | Yeah, sure. Why not? |
| Ben: | And also, it doesn't... it doesn't harm us at all, to be on Stitcher or you know... PodCatcher… whatever, like I don't know, we can be on all the services and it doesn't cost us anything extra. All they're doing is just passing around our RSS feed saying here’s where our files are. |
| Katie: | Yeah, so that makes sense, actually. I was just Googling us, cuz I wasn't sure if we were on Stitcher, so I just Googled for Linear Digressions for Stitcher, and sure enough we are, obviously. But I also didn't remember us getting on there, and so I think sometimes there’re RSS feeds that just get picked up, you know, potentially without people like us even being aware of, which is fine. That's no problem. |
| Ben: | Yes, that stuff really happen. |
| Katie: | But I wasn’t sure if that was something that we had to… that was sorta like setup by hand or... or exactly how we got on Stitcher just cuz that seem to be like an interesting case that I didn't remember it. |
| Ben: | Yeah, it's a… it’s kinda a crazy world. Let’s dive into the statistics bit, and I actually don't have a ton... a ton to say about this other than giving these stats is actually... rather I should say getting these stats reliably and knowing what they mean is a little bit tricky. |
| Katie: | Yes, well this is... this is my naïve impression of it. So when I go into SoundCloud I can see there's a little tab that says stats and it gives you a few numbers... that gives you your downloads by day and then those get broken out... sometimes episode by episode, so you can see that... we usually release on a Sunday night and so on Monday there's usually a big spike when people are sort of downloading it fresh, and then it tapers off really fast and then there's another big spike on Monday and then it tapers off and... and so the first thing I think I would notice is that, clearly... clearly this data has to get here from somewhere, it sounds like FeedBurner maybe a little bit involved in that, but in general this is not something that I understand how these… how these stats can be... |
| Ben: | So let me just give you… yeah I’ll give the TL:DR about this. The TL:DR is there’re two kinds of stats that we would care about.The first stat I'll go into first and this is not the one that you're talking about right now, this is the one with FeedBurner and it's called subscriptions, or subscribers I should say. And this is trying to measure as best as it can, the number of people who have subscribed to to our podcasts. So that's not just like having... have downloaded one episode or download a couple episodes, but like are subscribed and are consistently downloading every episode that we put up. |
| Katie: | And is that information that it would get from like iTunes or something. How does it know? |
| Ben: | No, because FeedBurner is upstream. |
| Katie: | Right. |
| Ben: | So FeedBurner passes thing down to iTunes. Now iTunes does know how many people download our podcast through iTunes, but it doesn't know how many people download our podcast, right. |
| Katie: | Yes. |
| Ben: | I have an Android phone, so for at least... at least me, I'm not downloading it from iTunes. So, FeedBurner is the last place... it’s basically the place where it forks out from, right? FeedBurner is the… |
| Katie: | Everything goes to FeedBurner, but then after that, there are no guarantees. |
| Ben: | Right, yeah. FeedBurner is kind of the source for all of these different aggregators for iTunes, for people subscribing directly. So FeedBurners is really the place where you want to get these… these metrics. The difficulty is that it's really really hard to measure because, the only thing you really know is how many people are downloading the feed, right? |
| Katie: | Right. |
| Ben: | Because... because remember, if someone downloads the feed and then goes and downloads 200... we don't have 200, but 20 episodes, or 50 episodes, or 1 episode, or no episodes, FeedBurner has no idea about that. FeedBurner only knows that it told some device somewhere “here is how you get to all the different episodes if you choose to”, right? |
| Katie: | Okay. |
| Ben: | So that... that would be how many people access our feed on a daily basis, or on a weekly basis, and to make matters worse, different devices will fetch the feed at different frequencies, and you got a whole bunch of box which are box like Stitcher or like iTunes, where you're going in and fetching this feed and downloading it down to see if it's changed. So this is kind of a really weird number, and it's a number that I've just decided to not trust at all because there's a lot of magic going on, because a FeedBurner... people basically have to make wild guesses, like okay, what percentage do... do we think our box see, you know, maybe they’re coming from certain IP addresses, maybe we can filter this out, but in terms of like... is this a unique user that's visiting... that's getting our feed you know, 7 times, like once every day, or is this seven unique users? That's a really tricky thing to figure out. |
| Katie: | Yeah, in other words, if I'm a data scientist and I’m trying to come up with some kind of analysis that tells me how well is podcast is going… like the... the FeedBurner numbers are going to be pretty... not just noisy but they could have some pretty serious systematic bias in them, so they're not something that I would probably want to use this like the ground truth in and any kind of like analytics I would try to do for example. |
| Ben: | Right, yeah and in this age of … oh my god, everyone is tracking me, it turns out with podcasts no... nobody is tracking you because nobody can. SoundCloud also has stats, what you were talking about, and that is not measuring anything to do with the feed. That’s measuring actual episode downloads, because remember, SoundCloud is the source for the MP3s. So if you and go and download our podcast, our RSS feed from iTunes, and that RSS feed, that XML file, says, “Hey, this URL is where you download Um detector 2, the dynamic somethin’ somethin’” |
| Katie: | Dynamic time warp. |
| Ben: | The dynamic… that’s right, let’s do the time-warp again. When they follow that URL, SoundCloud will be on the other end of that, and it'll be like, “Oh yeah, here's the file. And oh, by the way, maybe I'll just collect a little information about you and who you are.” And this isn't like scary stuff, this isn't like Google, Facebook, Apple, Amazon, you know, taking a lot of data and then doing things with it. This is really really basic simple stuff. |
| Katie: | Yeah, I mean, the (inaudible) stuff that's get fed up to me at least, I see how many downloads we get by day, and I also get very rough geographical information, so I have some idea of how many people listen to us in the United States, let’s say, versus in England or Canada or whatever. |
| Ben: | Yeah, now this data can also be noisy. For example, I'm looking at the last 14 days. And last 14 days we've had 32.4 thousand plays, which means the number of people who downloaded or played on Soundcloud directly. |
| Katie: | Okay. |
| Ben: | What do you think the top city for downloading was? |
| Katie: | Um... so I think I remember I looked at this at some point, and it was like... I thought when I looked at it before it was like San Francisco or San Jose or something like that. |
| Ben: | Right, so San Francisco is number 5. |
| Katie: | Okay. |
| Ben: | Number 4 is Toronto, number 3 is London, number 2 is New York, this... this is all like, “okay that's all reasonable”. Number 1 is Riverside California. Why Riverside California? |
| Katie: | What? |
| Ben: | What’s in Riverside California? Also, do you want to know the numbers? So San Francisco's 345, Toronto is 348, London is 388 over the course of the last 2 weeks, New York, 489 people, so if you're in New York, you probably... you might have a very small chance but a better chance than anyone else at finding other fellow Linear Digressions listeners. Riverside California had 13831. |
| Katie: | Oh... that sounds wrong. |
| Ben: | That sounds wrong, so, either we have a bot with… I don't know what incentive downloading our episodes 13000 times, or we just have a really strangely large influx of data scientist in the Riverside who just discovered our podcast, or that number’s just totally ridiculously wrong, right? |
| Katie: | Yeah, I actually recall like this story, this... this is kind of apocryphal, but there's always a story about… there were some kind of analysis they were trying to do like what's the... what's the state that has the highest… we will try to keep it a little bit PG, but I think in this particular case, certain types of internet-based malfeasance that you could imagine people, you know, shenanigans that people might get up to on the internet, and they're trying to break this down by state, or maybe like by state but then divided like per capita, which... which state is the one that's up to the most kind of shady business on the internet. |
| Ben: | Yeah. |
| Katie: | And... and Kansas as it turns out, is just through the roof, it was… |
| Ben: | Kansas? |
| Katie: | 10 times as high as like the next highest state. And… |
| Ben: | Alright. |
| Katie: | Yeah, so everyone was like, “that's weird.” And a bunch of people are coming up with all kinds of... kind of hand-wavey post hoc, let's... let's speculate wildly about the people who live in Kansas. |
| Ben: | Yeah. |
| Katie: | Turns out what it was, is that there was just a bunch of IP addresses that sort of were not particularly well defined, necessarily like where they are coming from, or where they were sort of... places where all the traffic was being routed through, that wasn't particularly geographically well-defined. And so, what happened to be doing in these cases is it just assigned them the IP address that was in the geographical center of the United States, they’re just like, “Okay, this is coming from the United States, we don't have any more information from that, stick a pin in the middle of the United States and we will just say it's coming from there.” |
| Ben: | Right. |
| Katie: | And as it turns out, geographically Kansas is in the middle of the United State. So there was all this kind of other random stuff that because of particular details of the way that people were... kind of basically disguising internet traffic, it was making it look like it was going through Kansas even though Kansas has nothing to do with it, so I wonder… |
| Ben: | It’s very possible. |
| Katie: | If something... I don't know, if that's what's going on in Riverside, but that might be my… a guess of mine. |
| Ben: | Like let's imagine that a huge chunk of the mobile listeners, for some reason, the way that SoundCloud is getting the location is causing something like that, then maybe it's 13831 people who are listening on... you know, some sort of mobile device or Riverside California, and you know, that's... that's half our listenership, so you definitely have to take a lot of this with a grain of salt, it’s basically what I'm saying. And I also wanted to... if you're OK with closing up this episode, I wanted to share number with you. |
| Katie: | Okay. |
| Ben: | Which is the total number of plays in the history of recorded time of Linear Digressions. |
| Katie: | Okay, it feels like a little bit weird and like… I feel like I'm talking about like how much money I make or something, like it's not but it… |
| Ben: | Yeah yeah, it is kind of weird. So we’ve been doing the podcast for you know… a year in change I guess? |
| Katie: | Well, more that that… like… the better part of two years at this point I think. We started the… we started in the fall of 2014? |
| Ben: | Twenty… fourteen? Well twenty… okay, so these are just SoundCloud plays, and I don't remember what we were doing before SoundCloud. |
| Katie: | I think we’re always on SoundCloud, weren’t we? |
| Ben: | Were we? I think SoundCloud... |
| Katie: | I think so. |
| Ben: | Oh yeah, I think SoundCloud had just released its podcast feature, and it was an invite-only beta kind of thing. |
| Katie: | Mm… yeah, fancy. |
| Ben: | And we got it, yeah. Anyway, 422000 plays. |
| Katie: | Ah, that’s so cool/ intimidating. |
| Ben: | Terrifying right? |
| Katie: | Yeah, a little bit. Well, thanks for sticking with us everybody. |
| Ben: | Yeah, it's been... it's been a fun ride, and I'm excited to the... for the rest of this year. I'm excited for… to get a little bit cooler so that way when I'm recording in this room it's not as hot. |
| Katie: | Ah, you mean like physically cooler? |
| Ben: | Yeah. |
| Katie: | Not like “cooler”? |
| Ben: | Oh no, it's already off-the-charts cool. |
| Katie: | (laughs)