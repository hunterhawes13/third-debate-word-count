## Synopsis

Third Presidential Debate word count using JavaScript to count the occurances of each word for both candidates and remove stop words. Stop words are natural language words which have very little meaning, such as "and", "the", "a", "an", and similar words.

Trump total non stop word count 779 words

Clinton tot non stop word count 1186 words

###Trump most used words

country - 26 occurances

bad - 17 occurances

hillary - 17 occurances

great - 16 occurances

percent - 15 occurances

mosul - 15 occurances

years - 14 occurances

dollars - 14 occurances

money - 13 occurances

borders - 13 occurances

happened - 13 occurances

iran - 12 occurances

putin - 12 occurances

millions - 12 occurances

isis - 11 occurances

obama - 11 occurances

jobs - 11 occurances

states - 11 occurances

disaster - 10 occurances

trade - 10 occurances

border - 10 occurances

left - 10 occurances

start - 9 occurances

russia - 9 occurances

amendment - 9 occurances

lot - 9 occurances

countries - 9 occurances

president - 9 occurances

talk - 9 occurances

women - 8 occurances

wall - 8 occurances

tremendous - 8 occurances

justices - 8 occurances

wanted - 8 occurances

iraq - 8 occurances

big - 8 occurances

deals - 8 occurances

strong - 7 occurances

world - 7 occurances

started - 7 occurances

violence - 7 occurances

good - 7 occurances

united - 7 occurances

happen - 7 occurances

give - 6 occurances

billion - 6 occurances



###Clinton most used words



donald - 28 occurances

country - 25 occurances

president - 23 occurances

women - 22 occurances

jobs - 18 occurances

work - 15 occurances

american - 13 occurances

kind - 12 occurances

clear - 11 occurances

tax - 11 occurances

america - 11 occurances

debt - 11 occurances

security - 10 occurances

government - 10 occurances

chris - 10 occurances

syria - 10 occurances

court - 10 occurances

election - 10 occurances

world - 10 occurances

plan - 9 occurances

years - 9 occurances

economy - 9 occurances

families - 9 occurances

dollars - 9 occurances

immigrants - 9 occurances

trump - 9 occurances

undocumented - 9 occurances

million - 9 occurances

stand - 9 occurances

rights - 8 occurances

great - 8 occurances

that - 8 occurances

money - 7 occurances

amendment - 7 occurances

united - 7 occurances



## Code Example


```

//Find 'em!
var wordRegExp = /\w+(?:'\w{1,2})?/g;
var words = {};
var matches;
while ((matches = wordRegExp.exec(text)) != null)
{
    var word = matches[0].toLowerCase();
    if (typeof words[word] == "undefined")
    {
        words[word] = 1;
    }
    else
    {
        words[word]++;
    }
}

// Sort 'em!
var wordList = [];
for (var word in words)
{
    if (words.hasOwnProperty(word))
    {
        wordList.push([word, words[word]]);
    }
}
wordList.sort(function(a, b) { return b[1] - a[1]; });

// lets see what donny had to say
var n = 1187;
var message = ["The top " + n + " words are:"];
for (var i = 0; i < n; i++)
{
    message.push(wordList[i][0] + " - " + wordList[i][1] + " occurance" +
                 (wordList[i][1] == 1 ? "" : "s"));
}
console.log(message.join("\n"));
```

## Motivation

To compare the vocabulary and frequency of word use of the two candidates. Findings conclude that Trump used 779 words not considered stop words. Clinton 1186 words not considered stop words.
## Installation

<!---Provide code examples and explanations of how to get the project.-->


## Contributors

Hunter Hawes
github: hunterhawes13
twitter: @tikishackfun

## Total Word Count 

###TRUMP
    "The top 779 words are:

country - 26 occurances

bad - 17 occurances

hillary - 17 occurances

great - 16 occurances

percent - 15 occurances

mosul - 15 occurances

years - 14 occurances

dollars - 14 occurances

money - 13 occurances

borders - 13 occurances


happened - 13 occurances

iran - 12 occurances

putin - 12 occurances

millions - 12 occurances

isis - 11 occurances

obama - 11 occurances

jobs - 11 occurances

states - 11 occurances

disaster - 10 occurances

trade - 10 occurances

border - 10 occurances

left - 10 occurances

start - 9 occurances

russia - 9 occurances

amendment - 9 occurances

lot - 9 occurances

countries - 9 occurances

president - 9 occurances

talk - 9 occurances

women - 8 occurances

wall - 8 occurances

tremendous - 8 occurances

justices - 8 occurances

wanted - 8 occurances

iraq - 8 occurances

big - 8 occurances

deals - 8 occurances

strong - 7 occurances

world - 7 occurances

started - 7 occurances

violence - 7 occurances

good - 7 occurances

united - 7 occurances

happen - 7 occurances

give - 6 occurances

billion - 6 occurances

paying - 6 occurances

run - 6 occurances

gave - 6 occurances

open - 6 occurances

report - 6 occurances

outsmarted - 6 occurances

twenty - 6 occurances

campaign - 6 occurances

respect - 6 occurances

assad - 6 occurances

deal - 6 occurances

signed - 6 occurances

plan - 6 occurances

clinton - 6 occurances

year - 6 occurances

taxes - 5 occurances

aligned - 5 occurances

pouring - 5 occurances

strongly - 5 occurances

syria - 5 occurances

vote - 5 occurances

appoint - 5 occurances

chris - 5 occurances

time - 5 occurances

companies - 5 occurances

tougher - 5 occurances

obamacare - 5 occurances

create - 5 occurances

nafta - 5 occurances

baby - 5 occurances

laws - 5 occurances

husband - 5 occurances

nuclear - 5 occurances

leaders - 5 occurances

business - 5 occurances

totally - 4 occurances

america - 4 occurances

china - 4 occurances

step - 4 occurances

allowed - 4 occurances

today - 4 occurances

outplayed - 4 occurances

worse - 4 occurances

japan - 4 occurances

drugs - 4 occurances

saudi - 4 occurances

arabia - 4 occurances

places - 4 occurances

coming - 4 occurances

thousands - 4 occurances

massive - 4 occurances

line - 4 occurances

nato - 4 occurances

waiting - 4 occurances

pay - 4 occurances

boy - 4 occurances

caused - 4 occurances

company - 4 occurances

greatest - 4 occurances

million - 4 occurances

frankly - 4 occurances

put - 4 occurances

false - 4 occurances

fbi - 4 occurances

general - 4 occurances

sad - 4 occurances

her - 4 occurances

donors - 4 occurances

shouldve - 4 occurances

changed - 4 occurances

law - 4 occurances

care - 4 occurances

prolife - 4 occurances

feel - 4 occurances

ceasefire - 4 occurances

repeal - 4 occurances

replace - 4 occurances

justice - 4 occurances

horrible - 3 occurances

unfair - 3 occurances

bringing - 3 occurances

ten - 3 occurances

growing - 3 occurances

amnesty - 3 occurances

businesses - 3 occurances

court - 3 occurances

happening - 3 occurances

trillion - 3 occurances

lied - 3 occurances

job - 3 occurances

experience - 3 occurances

department - 3 occurances

day - 3 occurances

cash - 3 occurances

idea - 3 occurances

kind - 3 occurances

based - 3 occurances

secure - 3 occurances

terrible - 3 occurances

destroying - 3 occurances

migration - 3 occurances

problem - 3 occurances

proud - 3 occurances

small - 3 occurances

stories - 3 occurances

gun - 3 occurances

tape - 3 occurances

renegotiate - 3 occurances

involved - 3 occurances

woman - 3 occurances

criminal - 3 occurances

fiction - 3 occurances

emails - 3 occurances

barack - 3 occurances

built - 3 occurances

hundreds - 3 occurances

germany - 3 occurances

haiti - 3 occurances

foundation - 3 occurances

anymore - 3 occurances

military - 3 occurances

american - 3 occurances

flag - 3 occurances

veterans - 3 occurances

angry - 3 occurances

warheads - 3 occurances

and - 3 occurances

all - 3 occurances

worst - 3 occurances

i - 3 occurances

problems - 3 occurances

illegally - 3 occurances

nice - 3 occurances

ad - 3 occurances

killed - 3 occurances

registered - 3 occurances

extremely - 3 occurances

decision - 3 occurances

fighting - 3 occurances

constitution - 3 occurances

thought - 3 occurances

cases - 3 occurances

aleppo - 3 occurances

excuse - 3 occurances

biggest - 3 occurances

rebels - 3 occurances

lots - 3 occurances

wait - 3 occurances

mexico - 3 occurances

machine - 3 occurances

apologize - 3 occurances

grow - 3 occurances

question - 3 occurances

build - 3 occurances

love - 3 occurances

rid - 3 occurances

lost - 2 occurances

youth - 2 occurances

making - 2 occurances

product - 2 occurances

communities - 2 occurances

education - 2 occurances

friends - 2 occurances

numbers - 2 occurances

toughest - 2 occurances

ninth - 2 occurances

suffer - 2 occurances

kick - 2 occurances

eighteen - 2 occurances

call - 2 occurances

gold - 2 occurances

standard - 2 occurances

puppet - 2 occurances

fifteen - 2 occurances

month - 2 occurances

turned - 2 occurances

position - 2 occurances

state - 2 occurances

win - 2 occurances

rest - 2 occurances

rip - 2 occurances

missiles - 2 occurances

womb - 2 occurances

russians - 2 occurances

meeting - 2 occurances

dollar - 2 occurances

loan - 2 occurances

agree - 2 occurances

prior - 2 occurances

middle - 2 occurances

record - 2 occurances

east - 2 occurances

birth - 2 occurances

statements - 2 occurances

created - 2 occurances

huge - 2 occurances

vacuum - 2 occurances

patrol - 2 occurances

sitting - 2 occurances

thousand - 2 occurances

largely - 2 occurances

debunked - 2 occurances

ice - 2 occurances

chicago - 2 occurances

rallies - 2 occurances

endorsed - 2 occurances

opinion - 2 occurances

honestly - 2 occurances

afford - 2 occurances

fame - 2 occurances

defend - 2 occurances

absolutely - 2 occurances

fictionalized - 2 occurances

uphold - 2 occurances

criminally - 2 occurances

congress - 2 occurances

fought - 2 occurances

south - 2 occurances

fourstar - 2 occurances

jail - 2 occurances

korea - 2 occurances

times - 2 occurances

presidency - 2 occurances

latinos - 2 occurances

charges - 2 occurances

enterprise - 2 occurances

giving - 2 occurances

treat - 2 occurances

horribly - 2 occurances

amount - 2 occurances

weapons - 2 occurances

lie - 2 occurances

moved - 2 occurances

contribute - 2 occurances

including - 2 occurances

tax - 2 occurances

buy - 2 occurances

college - 2 occurances

tuition - 2 occurances

fisher - 2 occurances

house - 2 occurances

houses - 2 occurances

talks - 2 occurances

deported - 2 occurances

moving - 2 occurances

clintons - 2 occurances

citizen - 2 occurances

powerful - 2 occurances

protecting - 2 occurances

took - 2 occurances

soros - 2 occurances

george - 2 occurances

protect - 2 occurances

questioned - 2 occurances

endorsement - 2 occurances

sat - 2 occurances

street - 2 occurances

ran - 2 occurances

media - 2 occurances

dishonest - 2 occurances

corrupt - 2 occurances

fact - 2 occurances

voters - 2 occurances

sudden - 2 occurances

absolute - 2 occurances

disgraceful - 2 occurances

upset - 2 occurances

allies - 2 occurances

regime - 2 occurances

months - 2 occurances

reading - 2 occurances

element - 2 occurances

surprise - 2 occurances

winner - 2 occurances

free - 2 occurances

wrong - 2 occurances

fifty - 2 occurances

write - 2 occurances

letter - 2 occurances

stupid - 2 occurances

john - 2 occurances

podesta - 2 occurances

bernie - 2 occurances

sanders - 2 occurances

judgment - 2 occurances

determination - 2 occurances

standpoint - 2 occurances

economy - 2 occurances

smarter - 2 occurances

florida - 2 occurances

backing - 2 occurances

york - 2 occurances

single - 2 occurances

terminate - 2 occurances

cut - 2 occurances

massively - 2 occurances

economic - 2 occurances

gdp - 2 occurances

political - 2 occurances

hacks - 2 occurances

bigger - 2 occurances

work - 2 occurances

mention - 2 occurances

mothers - 2 occurances

period - 2 occurances

week - 2 occurances

premiums - 2 occurances

election - 2 occurances

africanamericans - 2 occurances

blessed - 1 occurance

india - 1 occurance

unbelievable - 1 occurance

catastrophically - 1 occurance

number - 1 occurance

inappropriate - 1 occurance

level - 1 occurance

speed - 1 occurance

anemic - 1 occurance

process - 1 occurance

easily - 1 occurance

children - 1 occurance

league - 1 occurance

inefficient - 1 occurance

speaking - 1 occurance

citizens - 1 occurance

vietnam - 1 occurance

visited - 1 occurance

runs - 1 occurance

incredible - 1 occurance

conservative - 1 occurance

developed - 1 occurance

is - 1 occurance

cry - 1 occurance

pass - 1 occurance

factories - 1 occurance

thriving - 1 occurance

twentyfive - 1 occurance

bill - 1 occurance

brutally - 1 occurance

pivot - 1 occurance

bent - 1 occurance

amendments - 1 occurance

kicked - 1 occurance

finish - 1 occurance

sign - 1 occurance

transpacific - 1 occurance

partnership - 1 occurance

pour - 1 occurance

fathers - 1 occurance

relatives - 1 occurance

city - 1 occurance

scholars - 1 occurance

asked - 1 occurance

simple - 1 occurance

stop - 1 occurance

turn - 1 occurance

aspect - 1 occurance

radical - 1 occurance

islamic - 1 occurance

badly - 1 occurance

terrorism - 1 occurance

steel - 1 occurance

impossible - 1 occurance

mind - 1 occurance

supporter - 1 occurance

words - 1 occurance

sarcastic - 1 occurance

missing - 1 occurance

stolen - 1 occurance

mess - 1 occurance

manner - 1 occurance

represent - 1 occurance

assets - 1 occurance

worth - 1 occurance

billions - 1 occurance

listen - 1 occurance

trouble - 1 occurance

siege - 1 occurance

agents - 1 occurance

sixteen - 1 occurance

nra - 1 occurance

expanded - 1 occurance

phenomenal - 1 occurance

playing - 1 occurance

chicken - 1 occurance

real - 1 occurance

person - 1 occurance

earliest - 1 occurance

libya - 1 occurance

interpret - 1 occurance

opponent - 1 occurance

candidate - 1 occurance

means - 1 occurance

condemn - 1 occurance

met - 1 occurance

group - 1 occurance

friend - 1 occurance

honored - 1 occurance

damage - 1 occurance

appointing - 1 occurance

feeling - 1 occurance

reports - 1 occurance

clips - 1 occurance

wondering - 1 occurance

rally - 1 occurance

hampshire - 1 occurance

judges - 1 occurance

hired - 1 occurance

payed - 1 occurance

complaint - 1 occurance

violent - 1 occurance

fights - 1 occurance

individual - 1 occurance

wife - 1 occurance

spent - 1 occurance

overturned - 1 occurance

plane - 1 occurance

founders - 1 occurance

automatically - 1 occurance

act - 1 occurance

telling - 1 occurance

fistfights - 1 occurance

hurt - 1 occurance

riot - 1 occurance

minutes - 1 occurance

putting - 1 occurance

lies - 1 occurance

slightly - 1 occurance

mentions - 1 occurance

government - 1 occurance

possibly - 1 occurance

sleazy - 1 occurance

whatsoever - 1 occurance

destroyed - 1 occurance

generals - 1 occurance

subpoena - 1 occurance

admirals - 1 occurance

interpreted - 1 occurance

endorsing - 1 occurance

congressional - 1 occurance

read - 1 occurance

papers - 1 occurance

potentially - 1 occurance

serve - 1 occurance

medal - 1 occurance

lying - 1 occurance

honor - 1 occurance

recipients - 1 occurance

important - 1 occurance

appointed - 1 occurance

ripped - 1 occurance

defending - 1 occurance

spending - 1 occurance

qatar - 1 occurance

womens - 1 occurance

rights - 1 occurance

push - 1 occurance

gays - 1 occurance

buildings - 1 occurance

kill - 1 occurance

fortune - 1 occurance

bargain - 1 occurance

groups - 1 occurance

gesture - 1 occurance

takes - 1 occurance

century - 1 occurance

heroine - 1 occurance

hate - 1 occurance

agreements - 1 occurance

disgrace - 1 occurance

pores - 1 occurance

trump - 1 occurance

southern - 1 occurance

charities - 1 occurance

decide - 1 occurance

hear - 1 occurance

poisoning - 1 occurance

boats - 1 occurance

planes - 1 occurance

blood - 1 occurance

plenty - 1 occurance

palm - 1 occurance

beach - 1 occurance

meant - 1 occurance

continue - 1 occurance

dc - 1 occurance

talking - 1 occurance

proven - 1 occurance

disabled - 1 occurance

were - 1 occurance

entitled - 1 occurance

because - 1 occurance

liar - 1 occurance

ways - 1 occurance

that - 1 occurance

like - 1 occurance

mother - 1 occurance

past - 1 occurance

to - 1 occurance

take - 1 occurance

depreciation - 1 occurance

raise - 1 occurance

other - 1 occurance

stopped - 1 occurance

double - 1 occurance

shore - 1 occurance

acts - 1 occurance

drug - 1 occurance

proponent - 1 occurance

buffett - 1 occurance

lords - 1 occurance

public - 1 occurance

heller - 1 occurance

but - 1 occurance

explain - 1 occurance

most - 1 occurance

have - 1 occurance

done - 1 occurance

same - 1 occurance

thing - 1 occurance

date - 1 occurance

increase - 1 occurance

forced - 1 occurance

senator - 1 occurance

special - 1 occurance

interest - 1 occurance

change - 1 occurance

hombres - 1 occurance

apartment - 1 occurance

beautiful - 1 occurance

hotel - 1 occurance

singling - 1 occurance

watching - 1 occurance

rich - 1 occurance

ads - 1 occurance

paid - 1 occurance

race - 1 occurance

respond - 1 occurance

final - 1 occurance

pile - 1 occurance

amazing - 1 occurance

wrote - 1 occurance

article - 1 occurance

immediately - 1 occurance

poison - 1 occurance

minds - 1 occurance

heard - 1 occurance

find - 1 occurance

november - 1 occurance

eighth - 1 occurance

voter - 1 occurance

rolls - 1 occurance

imperative - 1 occurance

acceptable - 1 occurance

pew - 1 occurance

guilty - 1 occurance

crime - 1 occurance

rigged - 1 occurance

suspense - 1 occurance

attorney - 1 occurance

airplane - 1 occurance

tarmac - 1 occurance

arizona - 1 occurance

questions - 1 occurance

situation - 1 occurance

replica - 1 occurance

man - 1 occurance

watched - 1 occurance

felt - 1 occurance

credit - 1 occurance

starting - 1 occurance

attack - 1 occurance

late - 1 occurance

fan - 1 occurance

announce - 1 occurance

long - 1 occurance

douglas - 1 occurance

macarthur - 1 occurance

patton - 1 occurance

spinning - 1 occurance

graves - 1 occurance

stupidity - 1 occurance

stay - 1 occurance

days - 1 occurance

reason - 1 occurance

running - 1 occurance

office - 1 occurance

tough - 1 occurance

violated - 1 occurance

red - 1 occurance

sand - 1 occurance

mistakes - 1 occurance

eventually - 1 occurance

deaths - 1 occurance

upheld - 1 occurance

hard - 1 occurance

smart - 1 occurance

wonderful - 1 occurance

scalia - 1 occurance

obamas - 1 occurance

doubled - 1 occurance

national - 1 occurance

stupidest - 1 occurance

easy - 1 occurance

beneficiary - 1 occurance

outsmarting - 1 occurance

point - 1 occurance

no - 1 occurance

unfit - 1 occurance

wikileaks - 1 occurance

debt - 1 occurance

upreme - 1 occurance

beauties - 1 occurance

wellcrafted - 1 occurance

supreme - 1 occurance

sucked - 1 occurance

instincts - 1 occurance

catastrophe - 1 occurance

trauma - 1 occurance

slaughtered - 1 occurance

decisions - 1 occurance

humanitarian - 1 occurance

nightmare - 1 occurance

fallen - 1 occurance

go - 1 occurance

document - 1 occurance

pennsylvania - 1 occurance

loves - 1 occurance

ohio - 1 occurance

hicago - 1 occurance

bundles - 1 occurance

stage - 1 occurance

upstate - 1 occurance

thereabouts - 1 occurance

fled - 1 occurance

overthrow - 1 occurance

guy - 1 occurance

shape - 1 occurance

tens - 1 occurance

syrian - 1 occurance

refugees - 1 occurance

naturally - 1 occurance

trojan - 1 occurance

horse - 1 occurance

luck - 1 occurance

thanks - 1 occurance

for - 1 occurance

doing - 1 occurance

ridiculous - 1 occurance

defeat - 1 occurance

place - 1 occurance

ginsburg - 1 occurance

weeks - 1 occurance

vast - 1 occurance

swathes - 1 occurance

land - 1 occurance

ceasefires - 1 occurance

assume - 1 occurance

leadership - 1 occurance

higher - 1 occurance

bother - 1 occurance

duet - 1 occurance

separate - 1 occurance

audience - 1 occurance

raided - 1 occurance

lose - 1 occurance

industry - 1 occurance

sloppy - 1 occurance

tonight - 1 occurance

hiring - 1 occurance

bring - 1 occurance

peoplethose - 1 occurance

negotiators - 1 occurance

negotiate - 1 occurance

contribution - 1 occurance

dealing - 1 occurance

likes - 1 occurance

decades - 1 occurance

offshore - 1 occurance

engine - 1 occurance

expand - 1 occurance

disagree - 1 occurance

ronald - 1 occurance

reagan - 1 occurance

disagreed - 1 occurance

cutting - 1 occurance

rate - 1 occurance

rolling - 1 occurance

dying - 1 occurance

named - 1 occurance

cost - 1 occurance

seventeen - 1 occurance

die - 1 occurance

weight - 1 occurance

correct - 1 occurance

sixty - 1 occurance

seventy - 1 occurance

glad - 1 occurance

healthcare - 1 occurance

expensive - 1 occurance

price - 1 occurance

nasty - 1 occurance

raising - 1 occurance

control - 1 occurance

called - 1 occurance

bigleague - 1 occurance

depleted - 1 occurance

helped - 1 occurance

fixed - 1 occurance

earth - 1 occurance

illegal - 1 occurance

immigrants - 1 occurance

vets - 1 occurance


policemen - 1 occurance

disrespected - 1 occurance

order - 1 occurance

cities - 1 occurance

shot - 1 occurance

walking - 1 occurance

store - 1 occurance

high - 1 occurance

representatives - 1 occurance

lifetimes - 1 occurance"



###Clinton

"The top 1186 words are:

donald - 28 occurances

country - 25 occurances

president - 23 occurances

women - 22 occurances

jobs - 18 occurances

work - 15 occurances

american - 13 occurances

kind - 12 occurances

clear - 11 occurances

tax - 11 occurances

america - 11 occurances

debt - 11 occurances

security - 10 occurances

government - 10 occurances

chris - 10 occurances

syria - 10 occurances

court - 10 occurances

election - 10 occurances

world - 10 occurances

plan - 9 occurances

years - 9 occurances

economy - 9 occurances

families - 9 occurances

dollars - 9 occurances

immigrants - 9 occurances

trump - 9 occurances

undocumented - 9 occurances

million - 9 occurances

stand - 9 occurances

rights - 8 occurances

great - 8 occurances

that - 8 occurances

money - 7 occurances

amendment - 7 occurances

united - 7 occurances

americans - 7 occurances

pay - 7 occurances

fact - 7 occurances

time - 7 occurances

he - 7 occurances

isis - 6 occurances

children - 6 occurances

wealthy - 6 occurances

good - 6 occurances

system - 6 occurances

mosul - 6 occurances

talk - 6 occurances

states - 6 occurances

obama - 6 occurances

i - 6 occurances

national - 6 occurances

health - 6 occurances

haiti - 6 occurances

it - 6 occurances

thousand - 6 occurances

guns - 6 occurances

nuclear - 6 occurances

important - 6 occurances

russians - 6 occurances

thinks - 6 occurances

federal - 5 occurances

talking - 5 occurances

roe - 5 occurances

wade - 5 occurances

iraq - 5 occurances

hard - 5 occurances

behalf - 5 occurances

rigged - 5 occurances

social - 5 occurances

number - 5 occurances

home - 5 occurances

cut - 5 occurances

border - 5 occurances

corporations - 5 occurances

supreme - 5 occurances

reform - 5 occurances

foundation - 5 occurances

supported - 5 occurances

raise - 5 occurances

life - 5 occurances

ground - 5 occurances

opportunities - 5 occurances

of - 5 occurances

continue - 5 occurances

state - 5 occurances

lot - 5 occurances

making - 5 occurances

middle - 5 occurances

weapons - 5 occurances

energy - 5 occurances

defend - 5 occurances

woman - 5 occurances

military - 5 occurances

decisions - 5 occurances

support - 5 occurances

putin - 5 occurances

intelligence - 5 occurances

ways - 4 occurances

seventeen - 4 occurances

espionage - 4 occurances

attacks - 4 occurances

russian - 4 occurances

trade - 4 occurances

working - 4 occurances

trust - 4 occurances

workers - 4 occurances

campaign - 4 occurances

businesses - 4 occurances

proposing - 4 occurances

war - 4 occurances

mexican - 4 occurances

education - 4 occurances

college - 4 occurances

schools - 4 occurances

twenty - 4 occurances

put - 4 occurances

taxes - 4 occurances

person - 4 occurances

born - 4 occurances

will - 4 occurances

parents - 4 occurances

business - 4 occurances

countries - 4 occurances

penny - 4 occurances

agencies - 4 occurances

incomes - 4 occurances

terrible - 4 occurances

invest - 4 occurances


voted - 4 occurances


parenthood - 4 occurances

agreement - 4 occurances

planned - 4 occurances

putting - 4 occurances

debate - 4 occurances

case - 4 occurances

care - 4 occurances

dangerous - 4 occurances

clinton - 4 occurances

conflict - 4 occurances

protect - 4 occurances


family - 4 occurances

gun - 4 occurances

understand - 4 occurances

senate - 4 occurances

standing - 4 occurances

you - 4 occurances

is - 4 occurances

strongly - 4 occurances
have - 4 occurances

issue - 4 occurances

started - 4 occurances

civilian - 3 occurances

close - 3 occurances

find - 3 occurances


benefits - 3 occurances

massive - 3 occurances

responsibility - 3 occurances

mentioned - 3 occurances

look - 3 occurances


biggest - 3 occurances

nation - 3 occurances

a - 3 occurances

create - 3 occurances

hope - 3 occurances

small - 3 occurances

long - 3 occurances

lives - 3 occurances

immigration - 3 occurances

dozens - 3 occurances

pregnancy - 3 occurances

resources - 3 occurances

rid - 3 occurances

university - 3 occurances

worked - 3 occurances

recession - 3 occurances

fair - 3 occurances

greater - 3 occurances

mexico - 3 occurances

donalds - 3 occurances

met - 3 occurances

trillion - 3 occurances



worst - 3 occurances

feel - 3 occurances

act - 3 occurances

millions - 3 occurances



cost - 3 occurances

decision - 3 occurances

times - 3 occurances

cuts - 3 occurances

add - 3 occurances

us - 3 occurances



meet - 3 occurances

investments - 3 occurances


approach - 3 occurances

deal - 3 occurances

secretary - 3 occurances

powerful - 3 occurances

employers - 3 occurances

not - 3 occurances

increase - 3 occurances

cases - 3 occurances

china - 3 occurances

stage - 3 occurances

steel - 3 occurances

chinese - 3 occurances

medicare - 3 occurances

buy - 3 occurances


department - 3 occurances

experience - 3 occurances

borders - 3 occurances

kids - 3 occurances

justice - 3 occurances

called - 3 occurances

day - 3 occurances

happy - 3 occurances

reagan - 3 occurances

big - 3 occurances

bush - 3 occurances

rest - 3 occurances

issues - 3 occurances

move - 3 occurances

interests - 3 occurances

history - 3 occurances

young - 3 occurances

know - 3 occurances

returns - 3 occurances

income - 3 occurances

claims - 3 occurances

deported - 3 occurances

regulation - 3 occurances

highest - 3 occurances


means - 3 occurances

basically - 3 occurances



for - 3 occurances

nofly - 3 occurances

safe - 3 occurances
syrians - 3 occurances

give - 3 occurances

citizens - 3 occurances

force - 3 occurances

encouraged - 3 occurances

invasion - 3 occurances

comprehensive - 3 occurances

to - 3 occurances

zones - 3 occurances


growth - 3 occurances
situation - 3 occurances

race - 2 occurances

alliances - 2 occurances

safer - 2 occurances

frankly - 2 occurances

allies - 2 occurances

school - 2 occurances

class - 2 occurances

thrives - 2 occurances

online - 2 occurances

loophole - 2 occurances

program - 2 occurances

infrastructure - 2 occurances

high - 2 occurances

wage - 2 occurances

fight - 2 occurances

which - 2 occurances

idea - 2 occurances

problem - 2 occurances

but - 2 occurances

kinds - 2 occurances

matters - 2 occurances

job - 2 occurances

thirds - 2 occurances

saying - 2 occurances

going - 2 occurances

womens - 2 occurances

poverty - 2 occurances

abortions - 2 occurances

nominee - 2 occurances

preschool - 2 occurances

thinking - 2 occurances

toddlers - 2 occurances
real - 2 occurances

future - 2 occurances

wall - 2 occurances

bill - 2 occurances

didnt - 2 occurances

mother - 2 occurances

bernie - 2 occurances

sanders - 2 occurances

account - 2 occurances

top - 2 occurances

accepted - 2 occurances

share - 2 occurances

contribution - 2 occurances

paying - 2 occurances

analyzed - 2 occurances

produce - 2 occurances

contrast - 2 occurances

conclude - 2 occurances

senator - 2 occurances

reverse - 2 occurances

path - 2 occurances

adding - 2 occurances


me - 2 occurances

be - 2 occurances

before - 2 occurances

doubt - 2 occurances

bear - 2 occurances

actually - 2 occurances

dark - 2 occurances

shadows - 2 occurances

possibly - 2 occurances

represent - 2 occurances

running - 2 occurances

exploit - 2 occurances

administration - 2 occurances


repeatedly - 2 occurances

arkansas - 2 occurances

york - 2 occurances

control - 2 occurances

deficit - 2 occurances

inherited - 2 occurances
economic - 2 occurances

that's - 2 occurances

forced - 2 occurances

stay - 2 occurances

hurts - 2 occurances

open - 2 occurances

save - 2 occurances

lose - 2 occurances

sign - 2 occurances

year - 2 occurances

advice - 2 occurances

respect - 2 occurances

tradition - 2 occurances

test - 2 occurances

quoting - 2 occurances

shipped - 2 occurances

problems - 2 occurances

wikileaks - 2 occurances
aluminum - 2 occurances

bought - 2 occurances

las - 2 occurances

steelworkers - 2 occurances

vegas - 2 occurances

engaged - 2 occurances

reasonable - 2 occurances

raised - 2 occurances
presidency - 2 occurances

information - 2 occurances

briefly - 2 occurances

fund - 2 occurances

discrimination - 2 occurances

purpose - 2 occurances

sued - 2 occurances

major - 2 occurances
levels - 2 occurances

kill - 2 occurances

brought - 2 occurances

bin - 2 occurances

laden - 2 occurances
celebrity - 2 occurances

apprentice - 2 occurances

effort - 2 occurances

compare - 2 occurances

happening - 2 occurances

forward - 2 occurances

rallies - 2 occurances

reporter - 2 occurances

opportunity - 2 occurances

bring - 2 occurances

true - 2 occurances
influence - 2 occurances

judge - 2 occurances

fraud - 2 occurances

racketeering - 2 occurances

pattern - 2 occurances
admit - 2 occurances
rip - 2 occurances
deportation - 2 occurances
elections - 2 occurances
cyber - 2 occurances
charity - 2 occurances
proud - 2 occurances
treatment - 2 occurances
evidence - 2 occurances
percent - 2 occurances
astonishing - 2 occurances
community - 2 occurances
earthquake - 2 occurances
part - 2 occurances
released - 2 occurances
line - 2 occurances
run - 2 occurances
forty - 2 occurances
troubling - 2 occurances
hosting - 2 occurances
respond - 2 occurances
unprecedented - 2 occurances
eleven - 2 occurances
fbi - 2 occurances
lost - 2 occurances
primary - 2 occurances
democracy - 2 occurances
general - 2 occurances
game - 2 occurances
position - 2 occurances
iraqi - 2 occurances
forces - 2 occurances
regulations - 2 occurances
provide - 2 occurances
concluded - 2 occurances
weeks - 2 occurances
rocca - 2 occurances
vladimir - 2 occurances
raising - 2 occurances
zone - 2 occurances
choice - 2 occurances
defunding - 2 occurances
prevent - 2 occurances
refugees - 2 occurances
negotiation - 2 occurances
well - 2 occurances
order - 2 occurances
minutes - 2 occurances
do - 2 occurances
ten - 2 occurances
awesome - 2 occurances
said - 2 occurances
law - 2 occurances
was - 2 occurances
has - 2 occurances
what - 2 occurances
come - 2 occurances
google - 2 occurances
and - 2 occurances
hear - 2 occurances
him - 2 occurances
now - 2 occurances
because - 2 occurances
fighters - 2 occurances
fighting - 2 occurances
way - 2 occurances
nightclub - 2 occurances
threat - 2 occurances
smarter - 2 occurances
criticizing - 2 occurances
dollar - 2 occurances
enforcement - 2 occurances
grow - 2 occurances
fairer - 2 occurances
with - 2 occurances
commitment - 2 occurances
peace - 2 occurances
affordable - 2 occurances
accounts - 1 occurance
jeopardy - 1 occurance
professionals - 1 occurance
sworn - 1 occurance
absolutely - 1 occurance
striking - 1 occurance
ironic - 1 occurance
conflicting - 1 occurance
carry - 1 occurance
term - 1 occurance
cavalier - 1 occurance
casual - 1 occurance
ban - 1 occurance
korea - 1 occurance
saudi - 1 occurance
arabia - 1 occurance
terrifying - 1 occurance
bottom - 1 occurance
confirm - 1 occurance
happened - 1 occurance
responsible - 1 occurance
launching - 1 occurance
discovered - 1 occurance
so - 1 occurance
stepping - 1 occurance
heller - 1 occurance
personal - 1 occurance
regulate - 1 occurance
in - 1 occurance
an - 1 occurance
scare - 1 occurance
they - 1 occurance
would - 1 occurance
rhetoric - 1 occurance
terribly - 1 occurance
codes - 1 occurance
or - 1 occurance
his - 1 occurance
finger - 1 occurance
button - 1 occurance
language - 1 occurance
unfortunate - 1 occurance
country's - 1 occurance
tear - 1 occurance
choices - 1 occurance
referenced - 1 occurance
honor - 1 occurance
asia - 1 occurance
europe - 1 occurance
traveling - 1 occurance
east - 1 occurance
disagreed - 1 occurance
applied - 1 occurance
north - 1 occurance
based - 1 occurance
growing - 1 occurance
giving - 1 occurance
middleclass - 1 occurance
governments - 1 occurance
district - 1 occurance
columbia - 1 occurance
ii - 1 occurance
trying - 1 occurance
advanced - 1 occurance
manufacturing - 1 occurance
compete - 1 occurance
romania - 1 occurance
lgbt - 1 occurance
clean - 1 occurance
accordance - 1 occurance
climate - 1 occurance
change - 1 occurance
faith - 1 occurance
medical - 1 occurance
serious - 1 occurance
goings - 1 occurance
safely - 1 occurance
store - 1 occurance
girl - 1 occurance
help - 1 occurance
sent - 1 occurance
thats - 1 occurance
where - 1 occurance
two - 1 occurance
accept - 1 occurance
carla - 1 occurance
are - 1 occurance
worried - 1 occurance
from - 1 occurance
them - 1 occurance
minimum - 1 occurance
live - 1 occurance
constitution - 1 occurance
fulltime - 1 occurance
equal - 1 occurance
saving - 1 occurance
peoples - 1 occurance
starts - 1 occurance
fundamentally - 1 occurance
defending - 1 occurance
technical - 1 occurance
upset - 1 occurance
colleges - 1 occurance
operate - 1 occurance
apprenticeships - 1 occurance
prepare - 1 occurance
sending - 1 occurance
debtfree - 1 occurance
injure - 1 occurance
tuition - 1 occurance
loaded - 1 occurance
public - 1 occurance
talked - 1 occurance
action - 1 occurance
homes - 1 occurance
takes - 1 occurance
enacted - 1 occurance
gains - 1 occurance
precautions - 1 occurance
citizen - 1 occurance
fifteen - 1 occurance
nominates - 1 occurance
phoenix - 1 occurance
individual - 1 occurance
subject - 1 occurance
independent - 1 occurance
experts - 1 occurance
advises - 1 occurance
arms - 1 occurance
commonsense - 1 occurance
presence - 1 occurance
officers - 1 occurance
consents - 1 occurance
breaks - 1 occurance
marriage - 1 occurance
rounding - 1 occurance
nra - 1 occurance
causing - 1 occurance
dislocation - 1 occurance
seen - 1 occurance
trains - 1 occurance
truly - 1 occurance
buses - 1 occurance
trickledown - 1 occurance
economics - 1 occurance
on - 1 occurance
steroids - 1 occurance
lobby - 1 occurance
keeping - 1 occurance
side - 1 occurance
process - 1 occurance
equality - 1 occurance
lead - 1 occurance
another - 1 occurance
translate - 1 occurance
namely - 1 occurance
advocate - 1 occurance
largest - 1 occurance
ads - 1 occurance
regret - 1 occurance
lived - 1 occurance
include - 1 occurance
fifty - 1 occurance
v - 1 occurance
needed - 1 occurance
costed - 1 occurance
eighteen - 1 occurance
husband - 1 occurance
violent - 1 occurance
billion - 1 occurance
surplus - 1 occurance
eliminating - 1 occurance
office - 1 occurance
deport - 1 occurance
wonderful - 1 occurance
disaster - 1 occurance
depression - 1 occurance
talks - 1 occurance
investing - 1 occurance
building - 1 occurance
skill - 1 occurance
training - 1 occurance
guarantees - 1 occurance
meeting - 1 occurance
promised - 1 occurance
breakdown - 1 occurance
clintons - 1 occurance
plans - 1 occurance
affect - 1 occurance
aftertax - 1 occurance
constitutional - 1 occurance
combination - 1 occurance
inherit - 1 occurance
level - 1 occurance
catastrophe - 1 occurance
touch - 1 occurance
represented - 1 occurance
choked - 1 occurance
physically - 1 occurance
distraught - 1 occurance
team - 1 occurance
personally - 1 occurance
steps - 1 occurance
saved - 1 occurance
credit - 1 occurance
deserves - 1 occurance
positions - 1 occurance
dug - 1 occurance
twitter - 1 occurance
intimate - 1 occurance
enable - 1 occurance
higherpaying - 1 occurance
beginning - 1 occurance
difficult - 1 occurance
string - 1 occurance
moving - 1 occurance
upstate - 1 occurance
final - 1 occurance
laws - 1 occurance
tpp - 1 occurance
much - 1 occurance
introducing - 1 occurance
days - 1 occurance
twelve - 1 occurance
including - 1 occurance
workplace - 1 occurance
illegal - 1 occurance
dumping - 1 occurance
citizenship - 1 occurance
limited - 1 occurance
markets - 1 occurance
fought - 1 occurance
stood - 1 occurance
places - 1 occurance
necessarily - 1 occurance
hotel - 1 occurance
crocodile - 1 occurance
tears - 1 occurance
technology - 1 occurance
pull - 1 occurance
prosecutor - 1 occurance
deploy - 1 occurance
enforce - 1 occurance
agreements - 1 occurance
buying - 1 occurance
undermined - 1 occurance
product - 1 occurance
imagine - 1 occurance
untrue - 1 occurance
debunked - 1 occurance
numerous - 1 occurance
thank - 1 occurance
ownership - 1 occurance
bashing - 1 occurance
calling - 1 occurance
nineteen - 1 occurance
seventies - 1 occurance
childrens - 1 occurance
defense - 1 occurance
rapists - 1 occurance
criminals - 1 occurance
africanamerican - 1 occurance
drug - 1 occurance
dealers - 1 occurance
view - 1 occurance
racial - 1 occurance
apartment - 1 occurance
buildings - 1 occurance
borrowing - 1 occurance
fourteen - 1 occurance
father - 1 occurance
start - 1 occurance
beijing - 1 occurance
human - 1 occurance
insulted - 1 occurance
universe - 1 occurance
alicia - 1 occurance
machado - 1 occurance
goes - 1 occurance
eating - 1 occurance
machine - 1 occurance
arguing - 1 occurance
room - 1 occurance
monitoring - 1 occurance
raid - 1 occurance
bringing - 1 occurance
osama - 1 occurance
founding - 1 occurance
formal - 1 occurance
believe - 1 occurance
stringent - 1 occurance
permits - 1 occurance
undercut - 1 occurance
wages - 1 occurance
heard - 1 occurance
response - 1 occurance
held - 1 occurance
looking - 1 occurance
labor - 1 occurance
attractive - 1 occurance
assaulted - 1 occurance
attacked - 1 occurance
build - 1 occurance
writing - 1 occurance
story - 1 occurance
disgusting - 1 occurance
block - 1 occurance
belittling - 1 occurance
bigger - 1 occurance
dignity - 1 occurance
selfworth - 1 occurance
feels - 1 occurance
acts - 1 occurance
demonstrate - 1 occurance
expect - 1 occurance
tower - 1 occurance
pitting - 1 occurance
celebrate - 1 occurance
diversity - 1 occurance
lift - 1 occurance
underpaid - 1 occurance
grandchildren - 1 occurance
pushed - 1 occurance
uncomfortable - 1 occurance
immediately - 1 occurance
denying - 1 occurance
apologizes - 1 occurance
disabled - 1 occurance
mocked - 1 occurance
mimicked - 1 occurance
television - 1 occurance
khan - 1 occurance
man - 1 occurance
died - 1 occurance
serving - 1 occurance
gold - 1 occurance
star - 1 occurance
religion - 1 occurance
john - 1 occurance
mccain - 1 occurance
prisoner - 1 occurance
prefers - 1 occurance
captured - 1 occurance
exercising - 1 occurance
complained - 1 occurance
indiana - 1 occurance
trusted - 1 occurance
complain - 1 occurance
doesnt - 1 occurance
extent - 1 occurance
divisiveness - 1 occurance
mean - 1 occurance
vision - 1 occurance
incites - 1 occurance
violence - 1 occurance
applauds - 1 occurance
pushing - 1 occurance
pulling - 1 occurance
punching - 1 occurance
shouldnt - 1 occurance
stake - 1 occurance
furtherance - 1 occurance
countrys - 1 occurance
rank - 1 occurance
values - 1 occurance
proven - 1 occurance
thrilled - 1 occurance
mischaracterization - 1 occurance
secure - 1 occurance
renowned - 1 occurance
bipartisan - 1 occurance
ronald - 1 occurance
hivaids - 1 occurance
afford - 1 occurance
nominate - 1 occurance
partnership - 1 occurance
association - 1 occurance
environments - 1 occurance
healthier - 1 occurance
discussion - 1 occurance
able - 1 occurance
highranking - 1 occurance
quickly - 1 occurance
spend - 1 occurance
george - 1 occurance
donated - 1 occurance
programs - 1 occurance
rating - 1 occurance
watchdogs - 1 occurance
follow - 1 occurance
foundations - 1 occurance
foot - 1 occurance
portrait - 1 occurance
cancer - 1 occurance
read - 1 occurance
poorest - 1 occurance
hemisphere - 1 occurance
screenings - 1 occurance
hurricane - 1 occurance
devastated - 1 occurance
involved - 1 occurance
catastrophic - 1 occurance
agriculture - 1 occurance
sentence - 1 occurance
threaten - 1 occurance
raises - 1 occurance
candidate - 1 occurance
neighbors - 1 occurance
combined - 1 occurance
prove - 1 occurance
electric - 1 occurance
learned - 1 occurance
paid - 1 occurance
grid - 1 occurance
billionaire - 1 occurance
crosses - 1 occurance
horrifying - 1 occurance
direction - 1 occurance
benefit - 1 occurance
favor - 1 occurance
shutting - 1 occurance
conducted - 1 occurance
yearlong - 1 occurance
investigation - 1 occurance
emails - 1 occurance
unaccountable - 1 occurance
iowa - 1 occurance
caucus - 1 occurance
wisconsin - 1 occurance
defund - 1 occurance
republican - 1 occurance
emmy - 1 occurance
tv - 1 occurance
row - 1 occurance
tweeting - 1 occurance
emmys - 1 occurance
mindset - 1 occurance
funny - 1 occurance
thirty - 1 occurance
works - 1 occurance
free - 1 occurance
outcomes - 1 occurance
expected - 1 occurance
healthcare - 1 occurance
whining - 1 occurance
hacked - 1 occurance
finished - 1 occurance
shows - 1 occurance
denigrating - 1 occurance
appalled - 1 occurance
parties - 1 occurance
websites - 1 occurance
led - 1 occurance
turn - 1 occurance
army - 1 occurance
kurdish - 1 occurance
private - 1 occurance
special - 1 occurance
soldiers - 1 occurance
institutions - 1 occurance
occupying - 1 occurance
smart - 1 occurance
red - 1 occurance
flag - 1 occurance
waving - 1 occurance
punished - 1 occurance
reconstitute - 1 occurance
goal - 1 occurance
form - 1 occurance
fightive - 1 occurance
illusions - 1 occurance
press - 1 occurance
internet - 1 occurance
punishment - 1 occurance
headquarters - 1 occurance
hopeful - 1 occurance
advisors - 1 occurance
successful - 1 occurance
operation - 1 occurance
lots - 1 occurance
remain - 1 occurance
hotbed - 1 occurance
terrorism - 1 occurance
civil - 1 occurance
aided - 1 occurance
abetted - 1 occurance
iranians - 1 occurance
eye - 1 occurance
surge - 1 occurance
protects - 1 occurance
air - 1 occurance
terrorists - 1 occurance
fly - 1 occurance
push - 1 occurance
obtain - 1 occurance
central - 1 occurance
opposed - 1 occurance
die - 1 occurance
havens - 1 occurance
within - 1 occurance
electoral - 1 occurance
sets - 1 occurance
constant - 1 occurance
outflow - 1 occurance
confirmed - 1 occurance
gain - 1 occurance
leverage - 1 occurance
syrian - 1 occurance
abortion - 1 occurance
political - 1 occurance
track - 1 occurance
question - 1 occurance
evening - 1 occurance
once - 1 occurance
again - 1 occurance
finally - 1 occurance
implying - 1 occurance
background - 1 occurance
condemn - 1 occurance
checks - 1 occurance
rejects - 1 occurance
unlv - 1 occurance
questions - 1 occurance
mistake - 1 occurance
ago - 1 occurance
answered - 1 occurance
consistently - 1 occurance
denied - 1 occurance
happen - 1 occurance
very - 1 occurance
just - 1 occurance
want - 1 occurance
everybody - 1 occurance
disagreements - 1 occurance
go - 1 occurance
pretty - 1 occurance
opponent - 1 occurance
see - 1 occurance
sources - 1 occurance
verify - 1 occurance
can - 1 occurance
theres - 1 occurance
audio - 1 occurance
spout - 1 occurance
fall - 1 occurance
why - 1 occurance
does - 1 occurance
matter - 1 occurance
list - 1 occurance
told - 1 occurance
truth - 1 occurance
about - 1 occurance
guess - 1 occurance
believes - 1 occurance
makes - 1 occurance
better - 1 occurance
did - 1 occurance
vote - 1 occurance
really - 1 occurance
here - 1 occurance
all - 1 occurance
interplay - 1 occurance
sunni - 1 occurance
city - 1 occurance
baghdadi - 1 occurance
leadership - 1 occurance
breakup - 1 occurance
estimated - 1 occurance
digging - 1 occurance
underground - 1 occurance
prepared - 1 occurance
tough - 1 occurance
nato - 1 occurance
amazed - 1 occurance
launched - 1 occurance
attack - 1 occurance
conspiracy - 1 occurance
conspiracies - 1 occurance
supporting - 1 occurance
campaigned - 1 occurance
modern - 1 occurance
hasten - 1 occurance
aware - 1 occurance
legitimate - 1 occurance
concerns - 1 occurance
expressed - 1 occurance
favorite - 1 occurance
pte - 1 occurance
moscow - 1 occurance
washington - 1 occurance
sharing - 1 occurance
aligning - 1 occurance
efforts - 1 occurance
abandoned - 1 occurance
negotiations - 1 occurance
decided - 1 occurance
publicly - 1 occurance
blame - 1 occurance
russia - 1 occurance
cybermischief - 1 occurance
presidential - 1 occurance
huge - 1 occurance
concession - 1 occurance
leave - 1 occurance
dislocated - 1 occurance
strike - 1 occurance
interest - 1 occurance
vetted - 1 occurance
confidence - 1 occurance
slam - 1 occurance
door - 1 occurance
picture - 1 occurance
fouryearold - 1 occurance
boy - 1 occurance
aleppo - 1 occurance
blood - 1 occurance
coming - 1 occurance
face - 1 occurance
sat - 1 occurance
ambulance - 1 occurance
haunting - 1 occurance
careful - 1 occurance
vetting - 1 occurance
solve - 1 occurance
internal - 1 occurance
challenges - 1 occurance
stop - 1 occurance
radicalization - 1 occurance
muslim - 1 occurance
communities - 1 occurance
frontlines - 1 occurance
identify - 1 occurance
killer - 1 occurance
women's - 1 occurance
orlando - 1 occurance
pulse - 1 occurance
queens - 1 occurance
place - 1 occurance
heartbreaking - 1 occurance
emanates - 1 occurance
defeat - 1 occurance
painful - 1 occurance
slogan - 1 occurance
thought - 1 occurance
rushed - 1 occurance
recognize - 1 occurance
foreign - 1 occurance
decades - 1 occurance
interfere - 1 occurance
ad - 1 occurance
laughing - 1 occurance
stock - 1 occurance
puts - 1 occurance
fix - 1 occurance
convention - 1 occurance
asked - 1 occurance
grips - 1 occurance
prescription - 1 occurance
drugs - 1 occurance
whatsoever - 1 occurance
slow - 1 occurance
diminish - 1 occurance
visible - 1 occurance
economists - 1 occurance
call - 1 occurance
middleout - 1 occurance
rebuilding - 1 occurance
smartest - 1 occurance
reforms - 1 occurance
difference - 1 occurance
disagreement - 1 occurance
may - 1 occurance
experiences - 1 occurance
dad - 1 occurance
millionaire - 1 occurance
offy - 1 occurance
dads - 1 occurance
businessmandifference - 1 occurance
affects - 1 occurance
economychris - 1 occurance
record - 1 occurance
kremlin - 1 occurance
designed - 1 occurance
payroll - 1 occurance
assuming - 1 occurance
figure - 1 occurance
replenish - 1 occurance
fundmaking - 1 occurance
sufficient - 1 occurance
cap - 1 occurance
finding - 1 occurance
enhance - 1 occurance
lowincome - 1 occurance
disadvantaged - 1 occurance
current - 1 occurance
result - 1 occurance
additional - 1 occurance
dire - 1 occurance
consequences - 1 occurance
news - 1 occurance
deeply - 1 occurance
repeal - 1 occurance
extended - 1 occurance
solvency - 1 occurance
fundso - 1 occurance
repeals - 1 occurance
worse - 1 occurance
longterm - 1 occurance
drivers - 1 occurance
emphasize - 1 occurance
wellness - 1 occurance
entitlement - 1 occurance
spending - 1 occurance
decisionswatching - 1 occurance
tonight - 1 occurance
reaching - 1 occurance
democrats - 1 occurance
republicans - 1 occurance
independents - 1 occurance
talents - 1 occurance
skills - 1 occurance
ambition - 1 occurance
privileged - 1 occurance
disturbing - 1 occurance
protecting - 1 occurance
incredible - 1 occurance
lifes - 1 occurance
mission - 1 occurance
rising - 1 occurance
educations - 1 occurance
chance - 1 occurance
serve - 1 occurance"