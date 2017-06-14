| Person | Transcripts |
| :-- | :-- |
| Ben: | Hey Katie |
| Katie: | Hi Ben |
| Ben: | So you just got done running a marathon or… |
| Katie: | No, but I just got done running my Sunday long run which is 14 miles this week so that was like kinda actually... |
| Ben: | Oh my God, I can't even one-tenth of that, so... I can barely run one-tenth of that. I've been working on a home project. I feel like because we've both had some pretty intense weekends we should digress from our normal pattern of talking…. of talking about a topic in Data Science and instead, do Story Time with Katie Malone. What do you think? |
| Katie: | Sounds great. |
| Ben: | Alright, you are listening to Linear Digressions. |
| Ben: | Okay, so this is our first story time. What are you gonna... so what story are you going to tell? |
| Katie: | Well, so first we should say where we got the inspiration for this. |
| Ben: | Oh yes, let's do that. |
| Katie: | Okay, so this was a listener suggestion and we get a lot of really good emails, this is maybe the best email we’ve ever got. |
| Ben: | Yeah, it’s just... it was so heartwarming and touching and…made me cry. |
| Katie: | Yeah, no it didn’t. Did it really? |
| Ben: | It made me kind of tear up a little bit. Just a little bit. |
| Katie: | Okay, just a little bit. |
| Ben: | I don’t have a problem with crying but… |
| Katie: | You are not manly anyway. |
| Ben: | No no no, I’m not a particular…I’m not a particular manly man. But… |
| Katie: | (laughs) Um… this is an email from Jeff C. Thank you Jeff. The original email was “Hey guys, can you tell a good story about a time that I use machine learning to solve an interesting problem...” But then in the back and forth as a follow-up, he was saying how he listens to this podcast with his preteen daughter I think, which is completely awesome and… |
| Ben: | That’s incredible. |
| Katie: | Makes me just feel great about the world. So Jeff C., if you're listening, I hope you are, and I definitely hope you're listening with your daughter, so that I can tell her how great her dad is. Anyway... |
| Ben: | Oh no, you are gonna make me cry now. |
| Katie: | Oh my Gosh, Ben, keep it together. |
| Ben: | Oh God, I… it’s just… it’s been a weekend okay? |
| Katie: | Okay, how about we talk about email mining and energy fraud and maybe that will… |
| Ben: | That sounds great. |
| Katie: | Snap you outta this. |
| Ben: | That sounds great. |
| Katie: | Okay. |
| Ben: | Energy fraud. |
| Katie: | Yeah, so we talked about the… I think in one of our earlier episodes we talked about interesting datasets, we talked about the Enron emails dataset? |
| Ben: | Yeah, this was... this was way way back when we were... I think when we were in the first room that we were trying out... when we were recording in the offices at Udacity, and it was super echoey and it was... it was a really early episode I think. |
| Katie: | Yes, and so that dataset I have come to know and love because it was sort of the foundational data set for the introduction to machine learning course that I was teaching at Udacity, that I had just finished up with it at the time that we were starting this podcast. And… So, to give a little bit of backstory when I was building this course for Udacity, the ideas that we want to teach about machine learning and data science, and there's many different things that you can talk about in machine learning and data science. So having sort of like a season arc, so to speak for the whole course, is something that can help really tie it together... |
| Ben: | Definitely. |
| Katie: | And it gives them a reason to pay attention to some of all these details because they become relevant downstream when you're trying to tie it all together into one big interesting complicated chewy problem. |
| Ben: | Yeah, ultimately the course was really fantastic. Of course, part of that was your fantastic skill, part of that was also having a really good dataset that is relatively... I guess you could apply a number of different approaches to it. |
| Katie: | Yeah, so I had heard about the Enron dataset sorta known about it informally for a long time. It's one of these really famous datasets. And just to step back for a moment and tell this story. |
| Ben: | Right. |
| Katie: | So, in around the turn of the Millennium… like 2002 or so as I recall, there was this gigantic energy company that was called... well it was energy and all kind... all kinds of other stuff, it was very strange, this huge company called Enron. It was something like the 10 biggest company in the United States of the time or something, it was gigantic. |
| Ben: | Mm hmm… yeah. |
| Katie: | And it had all kinds of very tight political connections and there're just like a gigantic amount of money that this company was making. And to make a really long story short, there was a bunch of kind of dirty dealings that were going on inside, especially the very high levels of this company. So there was shady stuff that they were doing in the California energy market to kind of like... it caused all of... you remember those blackouts that were happening in California? |
| Ben: | Yeah...yeah. I remember that. I grown up in California. |
| Katie: | Yeah, that was Enron. |
| Ben: | That was Enron, yeah. |
| Katie: | They did this weird thing with the California energy grid to drive up energy prices and then sell things in just the right way. |
| Ben: | Yeah, super stitchy. |
| Katie: | They had this crazy... it was kind of like the last the last days of video rental stores like Blockbuster and Hollywood Video and stuff. This… this was you know within a decade or so Netflix would have taken over that market entirely. But they had this idea of using the internet to stream videos and have people like rent videos on the Internet which is basically what Netflix is, but they had this… |
| Ben: | Right. |
| Katie: | You know, it was kind of a crazy idea to do Netflix, like 10 years before anyone else did. It never worked. But... |
| Ben: | This was Enron? |
| Katie: | Yeah. |
| Ben: | This was...wow. So I didn't... I didn't know that part of the story. So this is just crazy weird company. |
| Katie: | Oh yeah, they were doing all kinds of stuff and then there was... |
| Ben: | Kinda like, maybe kinda like Amazon if Amazon was like having energy tie-end or something, I don't know. |
| Katie: | Yeah, it's... it's definitely a company that’s very hard to define exactly. What... it was...what it was because they were just doing so many different things. |
| Ben: | Right. |
| Katie: | And a fair amount of what was going on was also just out-and-out fraud. There was a lot of kind of weird things that their CFO was doing to make it look like they were a bunch of… I can’t remember exactly... I think it was something like they're a bunch of assets Enron held on its books that would have lowered the value of the company cuz there were like investments that Enron made that didn’t pan out and things like that. And so their CFO cooked up this really crazy thing where he would create subsidiary companies Enron and then he would sell the bad assets to the subsidiary companies like right before a reporting period so they didn't show up on the Enron books and then they would buy them back because the shell companies weren’t actually like meaningful independent entities from Enron itself. |
| Ben: | Yeah, it's super shady. |
| Katie: | And so, not surprisingly, the entire company ended up just com… well, yes, surprisingly, but not surprisingly I guess in retrospect, the entire company just ended up completely falling apart over the course of about a year. |
| Ben: | Right. |
| Katie: | And all of the top people were implicated like obviously the CFO, the Chief Operating Officer, the CEO and president and chairman and... Actually I’m not sure the CEO did, but the CEO and the president of the company ended up in jail and by my count roughly 30 or so people total ended up going to jail or being indicted or having some fairly serious like legal consequences for their role in this. And many many people lost their jobs and their pension funds all over the country that lost ton of money and it was just… it was a mess. |
| Ben: | Right. |
| Katie: | Okay. So that was the 2 minute introduction to Enron, so how is this relevant to machine learning? |
| Ben: | Right. |
| Katie: | So what really happened was during the course of the federal investigation, they subpoenaed a bunch of emails that the people in Enron had been sending to each other. And those emails then entered like the Congressional Record or something like this, they basically became public in a way that no email troll ever liked has been before or since. And probably in a way that, in all honesty, they maybe shouldn't have, if we knew a little bit more about that a lot of other people who... |
| Ben: | Right, but this was early days, right? So we didn't know... First of all, we didn't know how much could be extracted from a dataset like that... that wasn't necessarily explicitly in there. We also didn't really have many methods for anonymizing huge datasets like this. |
| Katie: | Yeah, and that anonymization... I mean there are lots of people who didn't do anything wrong but their emails got kind of sucked up in this and... you know... that... that's not good. |
| Ben: | Right. |
| Katie: | So… but those emails are sort of part of... they are in the wild now. And they've been studied from many different angles to give us ideas about how... how did people communicate in complex organizations, you know, what is the... what can we learn about how women are represented at the upper levels of these gigantic corporations, what was the social network structure like... all kinds of interesting things you can... you can ask with a dataset like this. So this is a super cool dataset and obviously like publicly available, and there's a lot of resources out there and a lot of background information that you can find out about and run just from Googling, which is basically how I know the things that I know about it. |
| Ben: | Mm hmm. |
| Katie: | So that I knew that this dataset seemed pretty cool. It's about 400000 emails and then it's organized, once you get the dataset it’s organized by certain mailbox so to speak, so you get in there and there's a hundred or so... hundred and fifty folders and each one of them is the name of a person. |
| Ben: | Wow. |
| Katie: | And then within that folder you’d find a bunch of emails like to that person. And there's some kind of big fish in there that you can find, like they have Kenneth Lay, they have Jeff Skilling. I don't think they have... |
| Ben: | So these are the people that went to jail? |
| Katie: | Yeah, Ken Lay was the president of the board and like chairman. Jeff Skilling was the CEO. Andrew Fastow was the CFO, the guy who was doing this weird shell company thing. His emails were not.. there wasn't like a folder named Andy Fastow… But that's roughly the structure of the dataset. |
| Ben: | Right. So like a very naive approach of trying to figure out what happened would just be to look at the people who went to jail and look at their folders and kind of study those emails, but that wouldn't really paint an entire like whole picture of what was going on or some of the other correspondences between people who were involved in shady stuff but didn't end up going to jail. |
| Katie: | Yeah, so… and just to step back for a second like the thing that I was interested in trying to do. I thought about it for a while what I wanted to do with this dataset. And the ideas I had was are there patterns in who people are sending emails to and/or what they're talking about that help us distinguish the accounts that are associated with what we ended up calling like persons of interest of people ended up either... what was our definition of a person of interest? A person of interest was a person who went to jail or was indicted or testified in exchange for prosecutorial immunity, so basically people who legally were somehow implicated in the fraud. |
| Ben: | Got it. |
| Katie: | And so, is there something in the emails that those people were sending or receiving that distinguish them from the mass of the company as a whole which we presume is by and large ignorant of the fraud and it’s innocent and then… but then, you know, you could imagine that like there were 30 or 35 people who ended up being a sort of persons of interest might not be every single person who was perhaps involved in what was going on here. So there's a little bit like fuzziness about what the actual label should be, but we could, the idea was let’s see if we can turn this into a supervised classification problem, where the emails are somehow the features that we have available to us. And then the labels that we want to find out are was this person a person of interest in the... in the legal case. |
| Ben: | So what was the like… what were the steps involved in taking this dataset and preparing it for this course basically? |
| Katie: | Yeah, so the first big one is something you already mentioned, which is that the number of persons of interest does not… that list doesn't map on very cleanly to the sub-folders within the Enron dataset. |
| Ben: | Oh I see. |
| Katie: | So I have this... |
| Ben: | So were you going through in like… cleaning... and cleaning this dataset up so that way it's a little more easy to work with? |
| Katie: | Yeah, so you have to like completely reformat it and in some ways. |
| Ben: | Ah. |
| Katie: | (laughs) So I have this kind of hand-curated list of 30 or 35 people who are my persons of interest. I have another... I'm trying to remember... I think like a hundred or so people that I have their email boxes that’s only overlap of less than 10 people between those two lists. And so I'm like well… you know... we can't really do this, we only have 10 people… 10 examples of Persons of Interest in here that we have their... their emails. The thing that... the emails are just in plain text so what it sort of looks like when you get in there and you start looking at the emails as each email as a file. They and just have like it’s a number: 1.txt, 2.txt, 3.txt, each one of those is an email. |
| Ben: | Okay. |
| Katie: | And then inside the file there’s gonna be the “to” line and the “from” line and the “BCC” line and then there's gonna be the text of the message, and there's a couple of… you know... the date or some other metadata. But the first thing that I was thinking about was like well... let's take the example of Andrew Fastow, I know I don't have Andrew Fastow’s email inbox,and so I’ll still be really interested in seeing the emails that are associated with his account. |
| Ben: | So some people may have sent emails to him or gotten emails from him and it might be in other people's account. |
| Katie: | Exactly. So what I have to do is I have to comb through all of the emails and I have to see do we have messages that were either from him or to him but there or where he cc'd on them or they’re showing up in somebody else's box. So you have to... and you have to ask that question of basically everyone... And when I say reformat it that's what I kind of mean is that we go through and we make a big list of everyone that we have in the entire... in the entire dataset, all of the people who were sending emails, all the people who are receiving emails, and then what emails map onto those senders and to those recipients and then we also had like I said CCs as well. So then you have this big long list of all the email addresses that are in this dataset, and then the emails that sort of are matched up with them. And you also have potentially the text of the messages as well but I haven't gotten to that point yet. And as we talked about text analysis can actually be pretty powerful, if you want to do something like tell the difference between two authors like supervised classification can actually… |
| Ben: | Yeah yeah, we talked about Satoshi Nakamoto I think. |
| Katie: | Mm hmm. |
| Ben: | The Bitcoin guy, we talked about JK Rowling, we talked about a number of those. |
| Katie: | Oh you forgot the best one. |
| Ben: | Oh what was the best one? |
| Katie: | Alexander Hamilton. |
| Ben: | Oh yeah. |
| Katie: | (inaudible) |
| Ben: | Of course (inaudible) |
| Katie: | And the star of my new favorite Broadway musical of all time. |
| Ben: | Yes, I’m excited about it too. |
| Katie: | Yeah, it’s coming to Chicago, I’m pumped. |
| Ben: | I got season tickets just because I had to... okay, let’s not go down this road (laughs) |
| Katie: | Wait, you can get season tickets to Hamilton? |
| Ben: | You… you can get...so… |
| Katie: | That doesn’t make any sense. |
| Ben: | So in the area where I lived, in San Jose, I think it's I don't know if it was coming to San Jose or if it's San Francisco it's... I think it's coming in San Francisco. But in order to be guaranteed to get Hamilton tickets in San Francisco you have to get season tickets, that's the way... that's the way they get you. |
| Katie: | Oh I see. |
| Ben: | That’s the way they got me. |
| Katie: | Yeah, so in Chicago, what I heard is that the pre-sale was just for groups, but I worked at a company that has a lot of theater nerds in it or like, oh, and also government nerds. And... |
| Ben: | Oh Jesus. Of course. |
| Katie: | So it was really easy to find 20 people who wanted to go see, anyway. |
| Ben: | Of course. |
| Katie: | Back on track. So… text analysis… of... let’s say the actual words that people are using in the messages like that would be on the table here potentially. |
| Ben: | That seems like a really simple thing to do too, it's just… I mean, a simple naive analysis would be you count up the different words that are used and you look at how frequently they use certain words versus other words. |
| Katie: | Yeah, so there were a few things that seemed kind of not great about that right after that if we were going to be doing it by... we’ll say... was organized by like author. So according to like when people are offering emails to other people, what are things that they're writing about. And so one of the things is that, there were... there were wildly different numbers of emails that we had associated with a different account, so we have lots and lots people that we only have one or two emails… |
| Ben: | Yes, that‘s statistically significant. |
| Katie: | Yeah, and then at the far end of the tail you had the most populous ones were more than 10,000. |
| Ben: | Shooo...yeah. |
| Katie: | And so it was a little bit hard to know the best way to like normalize that. And keep in mind I was doing this as sort of an example project for students in the Udacity course who presumably this is their first exposure to machine learning, so you don't want them to do anything that’s like totally crazy and weird. |
| Ben: | Yeah, yeah. So you're making... you're basically making a simple project and then you make instructions for them like, this is what you want to do first then, maybe you want to try this or this or this, and then the goal is for all of the students to be able to do the project that you made a sample project for. |
| Katie: | Yeah, so then I was like, well, what if we think of... my guess, and this is not supported by any research, this is a guess, is that maybe like, the text, the words that people are using when they're communicating is not as important for answering this question as just who they're talking to in the first place. |
| Ben: | I see. |
| Katie: | And so, what if I think about this, I still can't think about this as a text analysis program but to kinda keep things under control a little bit, instead of looking at the words they were using in the message, what if I look at every time they send an email to someone, I have that email address right? And so we think of all of those emails and email addresses as kind of like a vocabulary and the words that I used are all the email addresses that I'm corresponding with, and it’s the same… then you can use all the same infrastructure. |
| Ben: | Oh, so instead of counting words, you are counting email addresses that you see them send a message to… |
| Katie: | Yeah, but you can use… |
| Ben: | And so...yeah... |
| Katie: | You can use all the same packages and stuff so it’s still like (inaudible) pretty nicely. |
| Ben: | Oh nice. So you don't have to write all this from scratch? You can use all of the… all of the… |
| Katie: | The scikit and nltk. Yeah. |
| Ben: | That’s really cool. |
| Katie: | Yeah, so I was like, okay, sweet! So what I need to is I’m gonna start to look at the emails that people are sending to and from other people. Even then, like treating it as a text analysis problem, is still a little bit... a little bit too heavy-handed for my laptop to be completely honest. |
| Ben: | Oh. |
| Katie: | So I was like, okay, so let’s just make this even a little bit simpler. Let’s try to make an aggregated statistic for each person instead of having this like big long list of the vectorized counts of who sends all the emails to, blah blah blah... to make it a bit more intuitive. What if we just figure out how many emails they send to a person of interest, how many they receive from a person of interest, and how many they join “CC” with a person of interest. And you count this up over all the Persons of Interest as someone might be interacting with. So then you start to get and you can... and you can get the raw count and then you can also normalize it by like the total email volume of this person. And so then you start to get an idea of just whether they are interacting very frequently with the Persons of Interest or if they seem to be just not speaking with them at all. Which is now we are wandering like a little bit... it's changing the interpretation of what we're saying a little bit, we’re starting to say it’s like that people are interacting with Persons of Interest instead of they are using the same words as the Person of Interest. And you may end up getting slightly different answers for those two things. For example, maybe the number one person who interacts with Kenneth Lay is his secretary. You know, she’s probably not really involved in this. But, again, it’s sorta like bringing this a little bit under control so that we can start to move towards something that looks like a supervised learning problem. |
| Ben: | You know what’s really unique about this process, or about this project, is that you are not taking all of the tools out of your toolbox, and using any tool you want. In this particular project, you’re trying to use the simplest tools because the project that you’re doing is ultimately for beginners to do. And those beginners are gonna have a much more limited toolset both in terms of what they know, how to use. and what they also conceptually understand and would think to possibly apply. So it's kind of... it's kind of an unusual problem. |
| Katie: | Yeah, I mean, I think that a lot of the algorithms that you use in machine learning like they were designed with certain use cases in mind sometimes, but once you start to get to know the algorithms very well and you know the dataset, what you’re trying to do with it, then that all goes very well and you know the dataset what you're trying to do with it then a lot of the… sort of artistry of machine learning is figuring out how to find the tools that’s going to fit the problem that you have even if it doesn't map onto it like sort of perfectly and textbookly. But so now, I had sort of reduced my… I start out with this big sprawling like email text classification problem and now it had turned into like a bunch of labels and then the feature space is like… I don’t know… at this point...like with 7 columns or something, it's like the number of emails that you receive from a person of interest, the number of emails that you sent to a person of interest... you know... and it's... it's... it's collapsed down so much that it's hard to tell if we're even going to be able to get anything useful out. So then, I’m kind of reading about Enron in my spare time because I'm just like fascinated by it at this point, I'm taking up all these news articles from 2011… oh… sorry, 2001. I read this one article about... something about like you're not going to believe how much of a bonus these Enron guys were getting last year when the company was falling apart. I was like, interesting. And in the course of reading the article it became clear that whoever the reporter was for this article had seen a list that he come... that have been entered into the Congressional Record and had been like part of the Congressional testimony for the previous day and there was a list of all of these people at Enron and how much money they had made and how much money they had made in like a bunch of different categories, like their salary, their bonus, bunch of different kinds of stock options, whether or not they get reimbursed for travel. I'm probably forgetting some of these things… |
| Ben: | Yeah yeah. |
| Katie: | And I’m like, oh, that sounds... that sounds very interesting because now this is like a completely different type of data. This is money data, that if you can find a way to merge it in with the email data, and then you have the sort of 2 handles on this problem at the same time. I don't know how easy that merge is going to be and I don't know what it's going to look like, but like, I want to go find this dataset and see if I can try to, like, make that join. Cause then we’ll have just an entirely different picture of what might be going on here. So I forget how exactly but some kind of magical Google-Fu, I found this spreadsheet. |
| Ben: | (laughs) Google-Fu? |
| Katie: | Yeah. |
| Ben: | Google-Fu, it’s the best skill. |
| Katie: | I found the spreadsheet, it was like a PDF on some government transparency website. I wish then I could find one of those tools that like converts a PDF into a Google spreadsheet so that they can start to actually turn it into the table. And so, this list... this list has on it, I think a hundred and fifty or so people, has basically all of the Persons of Interest. So I was like, okay great, so I have money information for all the Persons of Interest, and there's a fairly tricky little operation now that I have to do to join in the email data because the email data is sorta indexed by email address and this financial information is indexed by name. And lucky for me, Enron has kind of a convention in the way that their email addresses are usually like first name last name @enron.com. So for a lot of them you could sort of go through the financial information, you can pull out the name, just concat the first name and last name and look for something that looks like that in your emails database. And that actually works for most of them. There were a bunch of stragglers that I had to go in and get them handled like people... people whose real name might be William but their Enron email address is like bill, whatever. Also sometimes you have two people with the same name, and you have to figure out you know one of them might be… |
| Ben: | Which is which. |
| Katie: | Yeah, one of them might be a secretary, the other one is a vice-president. And so from this, I have a bunch of information about who the shareholders are, who the vice presidents are, who's making... who's making tons of money. And then that was a much more interesting dataset to do this classification problem with. And it turns out that I was playing down with a bunch of different supervised classification algorithms where the inputs are how much money people are making and also sort of this email patterns turned out that the money is actually much more correlated with the whether you are a person of interest and the emails you have. |
| Ben: | Oh I see. |
| Katie: | So I put all those work and all those like great inspiration from the email addresses and then it turns out it's basically just money. But I never would have found the money if I hadn’t been thinking about these emails so carefully. |
| Ben: | Yeah. |
| Katie: | And that's basically where the story ends, like I said, this was a project for the Udacity students to go through, not necessarily with any heavy-handed interpretation at the back-end about who may or may not have been a person of interest in the Enron case, it was more experiences that you're going through and I'm thinking about this problem, what's the... what's the classification algorithm you wanna throw at it, or what are some of the performance metrics making sure you can set up your cross validation and all these other things that are just sort of... I'm grossing over right now, but they're really important for a especially first time students to get them all set up correctly, but we didn't... we wanted to make sure that like. the data was in a reasonably good format for students to be able to do this exercise. So obviously that meant there was a lot of work on my part, I wish… I wish... maybe now... thinking back I appreciate it even more than I did at the time I think. So yeah, that's the story how we found frauded Enron, I don’t know, not really, that’s not a valid statement. But… |
| Ben: | Yeah, we weren’t the ones who found the fraud. |
| Katie: | Oh yeah, no no no, that (inaudible). But I read a lot of people’s emails. |
| Ben: | Oh jeez. |
| Katie: | And that some of them were interesting. Most of them were boring. But some of them were fun. |
| Ben: | One...one interesting thing about this is I think when we first did an episode about this we didn't go into this much detail. But you said that this was an unprecedented dataset and I think we ended the episode with something like, you said, like, this is probably... we’re probably not never get another dataset like this. And then I think it was maybe a couple months after that, not all that long after that, and then the whole Sony hack thing happened |
| Katie: | Mm hmm. |
| Ben: | And then all of these emails were really out there. Now these were not entered into Congressional Record, they weren't legally leaked but definitely these humongous corpus emails from Sony execs and everything is indeed out there. So we'll probably continue to see datasets like this when companies get hacked but we’ll probably never see this again from any kind of legal channels because now we know enough… |
| Katie: | Yeah. |
| Ben: | To know that, you know, releasing these emails into the public is not a good idea because of how much data you can pull out of it, that’s not necessarily apparent. |
| Katie: | Yeah, I think the one thing, like the other place with big emails, I mean big banks with emails do come out fairly frequently. |
| Ben: | Yeah. |
| Katie: | It's just that it's a controlled release that's being done by the person who has the emails and so they're sort of like being really released voluntarily in a sense. So the things I'm thinking of in particular when I say this are like, Jeb Bush, when he started running for president had many years worth of correspondents that he had when he was governor of Florida. And he decided to release all of those emails as sort of an exercise in transparency and to show what a good leader he was and what a good executive... and so he... he actually published all of those emails on his website and (laughs) ended up taking them down eventually because there were some person identifiable information in there so they didn't even do a particularly good job of scrubbing them… |
| Ben: | Wow. |
| Katie: | But those datasets when you find them can still be...they can be fairly interesting, but you just had to keep in mind that this is the data that... that someone has decided it's okay for me to see, and that… then there's always like a slightly different way you have to think about that, if they're like, oh this is just like this data... this is all the data that there is, and this isn't like a controlled-release.
