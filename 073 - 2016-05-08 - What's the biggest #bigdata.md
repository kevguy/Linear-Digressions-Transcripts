| Person | Transcripts |
| :-- | :-- |
| Ben: |Hey Katie. |
| Katie: |Hi Ben. |
| Ben: |So I’ve been hearing this term “big data” and I don't... I don't really know what it means. |
| Katie: |Oh, so your problem is you're supposed to put a hashtag in front of it, it’s called #bigdata. (laughs) Is that a thing? |
| Ben: |Yeah, that's a real name. |
| Ben: | Alright, well, let's talk a little bit about data, Big Data, kind of the difference and how big is Big Data, I don't know. I feel strange saying that, but you are listening to Linear Digressions. |
| Ben: | Okay, so I guess we'll start with some projects that we've been talking about over the last many episodes. So way way way back when you were talking about writing an Um Detector because we had a lot of ‘um’s when we were recording a podcast and you have to go through and remove all of the ‘um’s and one of the problems you are running into if I remember it correctly is that you were dealing with a massive number of features, and also the ‘um’s might not be necessarily the same length, so they might be different... different features... different number of features. |
| Katie: | Right, so to unpack that a little bit. So the sampling rate for these microphones is 44 kilohertz, that's 44000 measurements per second. |
| Ben: |44.1 kilohertz or 48 kilohertz. Sorry, I'm an audio geek. |
| Katie: |Wait, how is it 44.1 or 48? |
| Ben: |So, actually the microphones… okay, going into geeky digressions audio world. Most microphones you can sample as fast as you want, the microphones themselves don't actually determine the sample rate, it's actually an exception because we're using the Blue Yeti microphones and those plug-in with USB and they've got their own little chip inside of the microphone, but the sample rates that you'll most often find are 44.1 kilohertz, 48 kilohertz, 96 kilohertz, which you don't see as often, or if you go to like a recording studio that's 192 kilohertz often times the recording. And what that means is let’s take 48 kilohertz instead of 44.1 cause actually the main reason 44.1 exists and is widely used is because that's what CDs use. But 48 kilohertz means that we are taking a measurement of the position of the diaphragm of the microphone 48000 times per second and because we're doing it so fast we're actually able to kind of create a reproduction of the movement of the microphone diaphragm and then when we take that and we type that into a speaker and we tell the speaker to move the diaphragm and its diaphragm in the same way, then it actually reproduces a pretty good approximation of sound, and that's how that all works. |
| Katie: |Oh, okay. |
| Ben: |So when you have 48000 samples per second and we're talking about data science… data, that's 48000 data points every second, that's a lot of features to take into account when you're trying to detect something like an um or do speech recognition or whatever it is. |
| Katie: |Yeah, and so usually when we record let’s say for a typical episode, it’s usually we have more raw material and then kind of edit it down, but it sort of that fall on compressed raw size is usually what a couple hundred Mbs I think? |
| Ben: |Yeah, and actually... if you... if you try and figure out how many samples there are in... let's say... twenty-minute episode and there may actually even be more than that because we've recorded a little bit longer and cut it down for everyone’s benefit. But that's 20 minutes times 60 seconds times 48000, I just did the math, that's 57.6 million data points in a 20-minute episode of Linear Digressions. |
| Katie: |Good math. And so then we edit it and we convert it from Mpeg format to MP3? Is that what we’re doing? |
| Ben: |Yeah...yeah. |
| Katie: |Oh, no, from aiff to mp3. |
| Ben: |Sorry, aiff, yeah. From aiff to mp3. Aiff is like totally uncompressed, mp3 is fairly well-compressed, it could be one-tenth the size. And that’s what allows you to download it rather than being so huge, it's actually a manageable size for you to download on your computer or your phone or even a 3g connection if you... if you needed to. |
| Katie: |Yeah, I think that… |
| Ben: |That’s data compression right there, so it’s taking out all of the stuff that you wouldn't notice if it was gone and... and it’s basically removing it or encoding it. |
| Katie: |Yeah, and I figured that compression stuff from aiff to an Mp3 roughly takes it down by roughly roughly an order of magnitude so that'll take us from maybe 200 to 20 or so and then, like you said, that's... that's manageable. |
| Ben: |Right. |
| Katie: |Okay, so that is just from our little set up that we have here, but obviously when people are talking about Big Data they usually talking about big centralized places that lots of people are contributing data to, or the potentially the data itself is very large. So I guess... I guess we should split it into two types of big data. So one is maybe something like Twitter or YouTube or you have lots and lots of people who are uploading, you know, all of them are creating data generating data and then uploading it to sort of this... this big network. And so each one of those files might be not ridiculously large, it may be a hundred megabytes... |
| Ben: |Yeah, like a tweet is gonna be not very big. |
| Katie: |Right, I think tweets are… once you include all the metadata I read that tweets are like 3 kilobytes a piece. And then videos obviously can range a whole lot in how big they are. And then there's also kind of the scientific Big Data and so for these I'm thinking about things like particle physics experiments which is something of course that I know very well, also astronomy has some ridiculously big... big data experiments that are sort of in construction right now. And I'm also thinking about genomic data which is still kind of really ramping up, its still fairly expensive to do things like genomic sequencing and there's the datasets don't always necessarily have huge numbers of rows in them but each one of those rows can be really really big in terms of the amount of data you need to have in it to do something like a full genome sequencing or an analysis of 4 genomes. |
| Ben: |Right, so I guess then... putting all of this into perspective, like to my feeble human brain. 57.6 million data points seems like a lot, but really in perspective, that's very very small compared to some of the experiments that are being run, some of the data sources that are that are constantly being contributed to like Twitter or whatever it is. 57.6 million is just change, it's nothing. |
| Katie: |Yeah, so let’s attach the numbers to this. I'm reading this paper, it's called “Big Data: Astronomical or Genomical?” And I will post the link to this on... in the show notes.And so they were comparing actually these four types of Big Data. They looked at astronomy Big Data, genomics Big Data, Twitter and YouTube. And so to attach some actual numbers to the things that they're talking about. So the first is astronomy and one of the big players in astronomy is the Australian Square kilometre array Pathfinder project. |
| Ben: |Yeah. |
| Katie: |And that is... it looks like currently up and running and they say that it has... it’s currently collecting 7 and a half terabytes per second of image taken... I mean, that’s insane. |
| Ben: |Per second? Okay… woah…. |
| Katie: |That’s nuts. |
| Ben: |Okay, let's... let's put that into perspective and compare it to... I guess our example with the episode of Linear Digressions. Like I said that was 7.6 million data points. If you divide that by 8, then you'll get the number of bytes and this is uncompressed. This is like biggest possible case for an episode of Linear… 20-minute episode of Linear Digressions would be 7200000, so 7.2 megabytes. And we're talking about terabytes, so 7 and about 7/2 megabytes versus 7/2 terabytes the difference between that is 6 orders of magnitude. 10 to the 6th versus 10 to the 12th. So that’s… |
| Katie: |A million. |
| Ben: |A million times right? |
| Katie: |Yeah, this is nuts. |
| Ben: |And that’s per second. |
| Katie: |Yeah, that’s per second. And that’s not even the full capacity of this thing. So… |
| Ben: |Oh. |
| Katie: |It’s running at that rate right now. And it looks like the projection is for it to be increased by another factor of a hundred in the next decade or so… 750 terabytes per second, 25 zettabytes per year. I don’t even know what a zettabyte is. |
| Ben: |Oh, I can tell you in a second. First, I just wanna just… give one more number, which is that 7 and a half terabytes would fill up pretty much an 8-terabyte hard drive, which is pretty much the biggest hard drive you can buy these days, that's about 200 bucks. That's not even taking into account how do you get all the data onto… like how do you capture all of that, right? So what was the thing that you just said? Zettabytes? |
| Katie: |Yeah, they say by 2025, the projected data collection of the telescope is 25 zettabytes per year. |
| Ben: |Alright, that is 10 to the 21. So going up the… what is it called… the decimal unit prefix tree right? You’ve got... 10 to the 1 is deca, and then hecto and then kilo is 10 to the 3, 10 to the 6 is mega, 10 to the 9 is giga, 10 to the 12 is tera, that is a terabyte. 10 to the 15 is peta. And then 10 to the 18 is exabyte. |
| Katie: |Okay. |
| Ben: |And then 10 to the 21 is zettabyte, right there. |
| Katie: |Oh wow, okay so... |
| Ben: |And that term, by the way, didn’t even reach adoption until 1991. So like back in the... back in the seventies, when they came up with peta and... and exa and started adopting that, I mean, no one could even imagine that we would ever need to use a term above that. |
| Katie: |(laughs) So we have to make up words? How much more do you know? |
| Ben: |We just have to make up a word, yeah. There’s also right above that. That's 10 to 21 is zettabyte, our zetta. And 10 to the 24 is yata, which really sounds like a joke. Yardi yardi yarda. |
| Katie: |Well, we’ll get there some day. |
| Ben: |Yeah. |
| Katie: |Okay, so astronomy. Completely insane amounts of data. |
| Ben: |(laughs) Right. |
| Katie: |Moving on, YouTube. So YouTube, it looks like the current numbers or something like, it so is about 300 hours of video are uploaded every minute. |
| Ben: |300 hours per minute. |
| Katie: |So you're just never gonna catch up with all of YouTube.And then, extrapolating out with say in the next 8 years, 6...7... 8, well, how many years is it till 2025? |
| Ben: |9 years. |
| Katie: |Yeah, 9 years. |
| Ben: |It’s 2016 right now. |
| Katie: |Yeah, next 9 years, they expected it might be something like 1,000 to 1,700 per minute, so that would be 1 to 2 exabytes of data. So exa is one level below zetta? |
| Ben: |Zeta. |
| Katie: |Right? Okay, so we're talking a factor of 1000 to 10000 less in the astronomy, from… |
| Ben: |So astronomy still wins over YouTube? |
| Katie: |Yeah, by a factor of 10000. |
| Ben: |That’s crazy. |
| Katie: |Yeah, that’s a lot. It is bananas how much data comes out of these scientific experiments. And I think that…particle physics is… is, well, we can come back to this...particle physics… is just to put it in context, is running a little bit behind. I think that… the LHC data output is something like 30 petabytes per year right now, although… you know, that’s right now, it’s supposed to in nine years. But I’ll say this, is that when we are working in the LHC there’s a vast amount of work that goes into actually selectively throwing away the data... |
| Ben: |Ah. |
| Katie: |Yeah, this is called the trigger, and so... |
| Ben: |Yeah, I was just gonna say like... you don’t necessarily… you said that particle physics is running a little bit behind, but really, you don’t want to be generating that much data because it's really expensive and it's also really really difficult like... how do you... how do you build something that can capture that amount of data per second, and then also store it, and then also be able to do analysis on it, that's just... it's really hard. |
| Katie: |Yeah, so the calculation that physics made is basically we’re gonna have very intense like … streaming data capacity that does a lot of our analysis… sort of on-the-fly. And then only the most interesting things get written to tape and then those are written to disk, I guess now. And those are the things that somebody like me has to go through and actually analyze. And so, to put things in perspective, there’s something like 40 million bunch crossings per second at the LHC, and the trigger will take it down to something like 200 bunch crossings per second that actually get recorded. So from whatever that reduction factor is, I can’t do that in my head right now, but 40 million to 200, that’s the data reduction that we have that gets us to 30 petabytes, very slender 30 petabytes per year. |
| Ben: |Oh my Gosh. That’s crazy. |
| Katie: |Yeah, it’s pretty nuts. Twitter, Twitter as we were sort of speculating, Twitter is… we think of it as big data, but it’s kind of the light weight of the group. So something like 500 million tweets per day are generated through the Twitter network, and as we said it was about 3 kilobytes. And Twitter is plateauing a little bit maybe compared to some of these other data generating processes but let's say they grow by a factor of 2 and a half between now and 2025, so that's the puts it in 1.2 billion tweets per day, that's about 1.3 petabytes per year. So that is a... full factor of 1000 less than what we're talking about from... from YouTube and then YouTube is a factor of 10000 below of what we're getting from astronomy. |
| Ben: |This stuff is really really hard to conceptualize, I mean, it's... that's a thousand times less and yet just a petabyte of data is more than you would ever have in your household, like by a lot. |
| Katie: |Yeah, well, so |
| Ben: |Yeah, no, I mean, maybe if you're an unusual person. |
| Katie: |Yeah, well, here’s… here’s… let’s… let’s get weird with this one for a second. |
| Ben: |Okay. |
| Katie: |So we talked about astronomy, we talked YouTube, we talked about Twitter. There was a fourth one that we’re gonna talk about and that is genomics. And the reason that I got a little bit squishy when you started talking about how people don't have this much data in their house is you have vast amounts of information that stored in your cells in the DNA. So if you think of your DNA, there's about 3 billion base pairs in the 23 chromosomes. |
| Ben: |3 billion you say? |
| Katie: |Yeah, uh huh. |
| Ben: |Okay. |
| Katie: |Yeah, so 3, not exactly 3 gigabytes of information, but like, if you make the… if you make that… approximation. |
| Ben: |It would be 3 giga… |
| Katie: |3 billion... |
| Ben: |Yeah, so you can make kind of like the quick hand wavy approximation that so there's... there's four types of a sort of base… gosh… I’m losing the word for a moment, the TCG and A. |
| Katie: |Right. |
| Ben: |The fundamental elements of DNA. like the base pairs or something? |
| Katie: |Yeah. |
| Ben: |But there’s four of them. And so you can say that each one of them takes like two bits to represent basically. |
| Katie: |Sure. |
| Ben: |Like ones and zeroes. So if you have 3 billion… 3 billion base pairs and then each one... each base pair is two bits of information, then you can get a 4 base pairs per byte and so what's 3 billion divided by 4. I feel like .75 billion 3 (inaudible) |
| Katie: |Let’s say a billion, it’s easier. |
| Ben: |Okay, we’ll say… |
| Katie: |It’s a gigabyte of data. |
| Ben: |It’s a gigabyte of data per cell. |
| Katie: |Per cell. |
| Ben: |And then I just have to Google this, how many cells are in your body? These are the numbers that I don’t know, But I will share them with you now. So this is... this is one of those things that's also kind of hard to estimate but somebody went in and kind of dated back the envelope thing. And the number they came up with was about 37 trillion cells, so what's... what's a gigabyte times 37 trillion, how many bytes is that of information in your body? |
| Katie: |Oh, okay. 37 trillion times, oh, so we can just use our little tree for this actually. Because 10 to the 12 is a trillion, 10 to the 9th is a billion, and if we add 9 + 12 we get twenty one that says zettabyte. So some number of zettabyte. Oh so, there we go. |
| Ben: |A zettabyte in your body? |
| Katie: |Um… was the number 37 trillion, you say? |
| Ben: |Oh yeah. |
| Katie: |Then we’ll say 37 zettabytes, that’s all. |
| Ben: |So, we do have a lot of data in your house as it turns out. It is walking around and listening to this podcast right now. |
| Katie: |You know, we don’t need to buy hard drives to I don’t know… we are born to happen to have all of the data. That’s... lucky us. |
| Ben: |Yeah, our body seems to be pretty good at like...packing it in. |
| Katie: |I'm sure a lot of it is quite redundant wouldn’t you say? |
| Ben: |Yes, yes. |
| Katie: |So like… |
| Ben: |If you're going to do something like sequence a genome, you have three billion base pairs and you say that like they're going to be mostly the same throughout all the different cells. There's important caveats to that which we should get to it in a second, but it turns out that doing genomic analysis and sequencing and alignment is… is pretty difficult, it can be a little bit noisy, and so one of the sources that I was reading says that in order to get those three billion base pairs correctly, you want to collect roughly 30 times as much data as that, so that would be 100 billion base pairs? |
| Katie: |Right. |
| Ben: |For doing the sequencing. And then once you start to figure out like how much... how much data that is, it's fairly expensive still to do genomic sequencing I think of full human gene, all those come down, an insane amount over the last decade or two. But a full human genome sequencing cost something like $1,000 and so it's not really accessible to most of the world right now. But there're 6 billion people, 7 maybe, walking around. And... and so, you can imagine that if the cost continues to fall and there're sort of scientific push for it, but there's potentially hundreds of millions or even billions of people who could have their genomes sequenced, each of them with potentially 100 billion base pairs that collected and so now we're talking about not just very very wide tables but very very long tables, and we are in an extraordinary high data, a kind of ratio, between those two pushing factors. Doing kind of again the number-crunching it's... it's really hard to extrapolate too far, just because genomic sequencing is still so young, that it's hard to know exactly how it's going to keep scaling like, do you assume that it keeps scaling at the rate that has been scaling so far historically? Or do you assume that it's going to scale like Moore's Law and so on, blah blah blah, cause you reach different conclusions depending on the assumptions that you make about the future performance of the field, but they make sort of an estimate that in 2025 for human genomes we might need something like to 2 to 40 exabytes, where does that put us relative to the astronomy? Is that still below the astronomy right now? |
| Katie: |It still is kind of below. Yeah. |
| Ben: |Okay, so it sounds like maybe astronomy is still winning. |
| Katie: |It’s still a winner. |
| Ben: |I just want to take a brief moment, now that we've gone through all of that, I want to take a brief moment I just kind of talked about how we've been talking about terabytes and petabytes and exabytes and zettabyte kind of interchangeably, but the jump from any one of them to the next 1 is a factor of a thousand. That’s just insane, like I can't even keep in my head what the number 1000 means right? I mean that the best I can imagine is like doing it with M&M's or something, 1 M&M versus 1000 M&M’s or something. But it's just that the numbers that we're talking about especially for astronomy, but really for any of these examples, are just gargantuan numbers. |
| Katie: |Yeah, it’s not just the collection and the storage that comes attached to these numbers but the reason that you're collecting all these data is because you want to be doing analytics on it and I think that this is where genomics like really pulls away from the pack in some senses because doing analytics on genomic data is really tough, you need to do things like alignment which is where you actually take these strings of DNA and then what you want to do is you want to put them in basically a matrix, so that you can have each row be like a person in the matrix and then you know the genes that are comparable across people are kind of sitting in the same places so you can compare them more directly. And that alignment process is very very difficult and you know, it's hard to get like consistent answers and it's very computationally expensive. And so doing analysis of this genomic data is I mean, it's extremely challenging now and it's only going to get harder. And so there's a lot of people who I think are looking very carefully, at like, when we have all these ideas about what we want to do if we could collect all this genomic data but do we have the computationally capacity to deal with it? And of course there's a lot of very smart people who are working on trying to make different types of like cloud computing platforms basically that can do genomic data storage and end analysis and things like that, but yeah, it's extreme... it's going to be extremely challenging to keep up with the rate at which we could be collecting these data. And then the second thing I'll say is that we... we kind of brush past this a little bit earlier, but how many... how many base pairs you really need to sequence per person and if we say that a full genome has three billion base pairs in it, we’re not really done there, because a lot of the reason that you're wanting to do this kind of science is because you're looking at like let’s take the example of cancer because I think that this is probably the single most, like complicated case but it's also one that I think is really driving the start of research so it's fairly good as as representative. |
| Ben: |Right, you're not just looking at 1 cell and then taking a bunch of similar representative samples and combining that together you're looking... you're trying to compare healthy cells and cancerous cells or something like that. |
| Katie: |Not just that, is that cancer is a disease of genetic variation and so the cells that you find, let's say you have a tumor, and a lot of people have been doing research on just this topic, if you take cells from like, let’s say it was in the middle of the tumor, those cells might be... have a certain mutation in them that allowed them to do something like angiogenesis, sorta build the blood vessels that supply the tumor with blood so that it can continue to grow. And that's a specific genetic mutation that you need to have for it to do that, build that, like feeding that network if you will, but then you could also imagine that the tumor... the cells around the periphery have a different mutation and that mutation allows them to kind of break off from the main tumor and then go elsewhere in the body and metastasizes the cancer. |
| Ben: |Oh I see. |
| Katie: |And so depending on where in the tumor you are, you can be... you can be looking at cells that have completely different sets of mutations and this is one of things that makes cancer so hard to treat is that it's really hard to get all of the… it's not like everything in the tumor can just be hit in the same way, there's different mutations that are contributing like a cell-by-cell basis and so then you're looking at something like... I will... we will need to collect hundred or a thousand times as much of the data to really get the full profile of all the different types of mutations we are dealing with here. So it only gets more complicated. So that's what's going on with #bigdata. |
| Ben: |#bigdata (laughs) yeah. |
| Katie: |Yeah, there's a lot out there. It's only going to get bigger. |
| Ben: |Wow. |
| Katie: |Yeah. |
| Ben: |That’s seriously bigger than our Um Detector dreams. |
| Katie: |Yes, I would say so. Well, the world wouldn’t be a very interesting place if an Um Detector was the biggest problem we had to deal with. |
| Ben: |Yeah, that’s a good point. |
| Katie: |Yeah, yeah. It was... it was very startling for me this weekend... kind of reading all of these papers and just realizing that you know, I come from LHC I come from physics, big data and it's really quite humbling to think about how much data is coming even from next generation scientific experiments and but also like I said just what’s stored inside of the cells that make up you and me and everybody else.
