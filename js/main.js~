var game = new Phaser.Game(800, 600, Phaser.AUTO, 'game', { preload: preload, create: create });



function preload () {
    game.load.image('school', 'assets/background2.jpg');
    game.load.image('mainmenu', 'assets/mainmenu.png');
    game.load.image('play', 'assets/play.png');
    game.load.image('textbox', 'assets/textbox.png');
    game.load.image('intro','assets/intro.png');
    game.load.image('next','assets/next.png');
    game.load.image('kitty1','assets/kitty1.png');
    game.load.image('p1op1','assets/p1op1.png');
    game.load.image('p1op2','assets/p1op2.png');
    game.load.image('kitty12','assets/kitty12.png');
    game.load.image('p1op3','assets/p1op3.png');
    game.load.image('p1op4','assets/p1op4.png');
    game.load.image('kitty2','assets/kitty2.png'); 
    game.load.image('p2op1','assets/p2op1.png');
    game.load.image('p2op2','assets/p2op2.png');
    game.load.image('kitty3','assets/kitty3.png'); 
    game.load.image('p3op1','assets/p3op1.png');
    game.load.image('p3op2','assets/p3op2.png');   
    game.load.image('kitty31','assets/kitty31.png');
    game.load.image('kitty4','assets/kitty4.png'); 
    game.load.image('p4op1','assets/p4op1.png');
    game.load.image('p4op2','assets/p4op2.png'); 
    game.load.image('p4op3','assets/p4op3.png'); 
    game.load.image('kitty41','assets/kitty41.png');
    game.load.image('kitty5','assets/kitty5.png');
    game.load.image('p5op1','assets/p5op1.png'); 
    game.load.image('p5op2','assets/p5op2.png');
    game.load.image('kitty51','assets/kitty51.png');
    game.load.image('kitty6','assets/kitty6.png'); 
    game.load.image('p6op1','assets/p6op1.png');
    game.load.image('p6op2','assets/p6op2.png'); 
    game.load.image('kitty61','assets/kitty61.png');
    game.load.image('kitty7','assets/kitty7.png'); 
    game.load.image('p7op1','assets/p7op1.png');
    game.load.image('p7op2','assets/p7op2.png'); 
    game.load.image('p7op3','assets/p7op3.png'); 
    game.load.image('kitty71','assets/kitty71.png'); 
    game.load.image('kitty72','assets/kitty72.png'); 
    game.load.image('kitty8','assets/kitty8.png'); 
    game.load.image('p8op1','assets/p8op1.png');
    game.load.image('p8op2','assets/p8op2.png'); 
    game.load.image('kitty81','assets/kitty81.png'); 
    game.load.image('kitty82','assets/kitty82.png'); 
    game.load.image('p8op3','assets/p8op3.png'); 
    game.load.image('kitty9','assets/kitty9.png'); 
    game.load.image('p9op1','assets/p9op1.png');
    game.load.image('p9op2','assets/p9op2.png'); 
    game.load.image('kitty91','assets/kitty91.png'); 
    game.load.image('kitty92','assets/kitty92.png'); 
    game.load.image('kitty10','assets/kitty10.png'); 
    game.load.image('p10op1','assets/p10op1.png');
    game.load.image('p10op2','assets/p10op2.png'); 
    game.load.image('kitty101','assets/kitty101.png'); 
    game.load.image('p101op1','assets/p101op1.png');
    game.load.image('kitty102','assets/kitty102.png'); 
    game.load.image('p102op1','assets/p102op1.png');
    game.load.image('kitty103','assets/kitty103.png'); 
    game.load.image('kitty104','assets/kitty104.png'); 
    game.load.image('body','assets/body.png');
    game.load.image('closedsmile','assets/closedsmile.png');
    game.load.image('opensmile','assets/opensmile.png'); 
    game.load.image('hmface','assets/hmface.png'); 
    game.load.image('whatface','assets/whatface.png'); 
    game.load.image('uhhuhface','assets/uhhuhface.png'); 
    game.load.image('smallopen','assets/smallopen.png'); 
    game.load.image('mmface','assets/mmface.png'); 
    game.load.image('ohface','assets/ohface.png'); 
    game.load.image('smallclosed','assets/smallclosed.png'); 
    game.load.image('sadface','assets/sadface.png'); 
    game.load.image('blush1','assets/blush1.png'); 
    game.load.image('blush2','assets/blush2.png'); 
    game.load.image('blush3','assets/blush3.png'); 
    game.load.image('sweatdrop','assets/sweatdrop.png'); 
    game.load.image('omgface','assets/omgface.png'); 
    game.load.image('okayending','assets/okayending.png');
    game.load.image('badending','assets/badending.png');
    game.load.image('goodending','assets/goodending.png');
    
}

var background;
var play;
var textbox;
var maintxt;
var next;
var op1;
var op2;
var op3;
var body;
var face;

function create() {

	//the main menu of the game
	background = game.add.sprite(0, 0, 'mainmenu');
	play = game.add.sprite(150,450, 'play');
  
	//  Enables all kind of input actions on this image (click, etc)
  	  play.inputEnabled = true;
  	  play.events.onInputDown.add(intro, this);

}

//The first phase of the game.
function intro () {
	/*<You are a new student at Kittytown High. Today is
	your first day. Your objective? To find love of course!
	As if on cue, a rather perky feline walks in and 
	takes a seat by you.>*/
	background.loadTexture('school',0);
	play.destroy();
	body = game.add.sprite(250,150,'body');
	body.visible = false;
	face = game.add.sprite(307,61, 'closedsmile');
	face.visible = false;
	textbox = game.add.sprite(2,404,'textbox');
	maintxt = game.add.sprite(20, 420, 'intro');
	next = game.add.sprite(325, 530, 'next');
	next.inputEnabled = true;
	next.events.onInputDown.add(phase1, this);
}

function phase1 ()
{
	next.inputEnabled = false;
	next.visible = false;
	body.visible = true;
	face.visible = true;
	
/*	^-^
	Hello, you must be the new student! I'm Kitty.
	You look older than a highschool student though.
	Can I call you Sempai?
	 	-Sure!		-Whatever.	*/
	//launch main
	maintxt.loadTexture('kitty1',0);
	op1 = game.add.image(150,490,'p1op1');
	op1.inputEnabled = true;
	op1.events.onInputDown.add(phase12, this);
	op2 = game.add.image(150, 530, 'p1op2');
	op2.inputEnabled = true;
	op2.events.onInputDown.add(phase12, this);
	op3 = game.add.sprite(150, 540, 'p4op3');
	op3.visible = false;
	op3.inputEnabled = false;
	    

}

function phase12  ()
{
	next.inputEnabled = false;
	next.visible = false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('opensmile',0);
/*	:)
	Great! Our first class is biology. Are you familiar
	with the subject?
		-Yeah, sort of. ->4
		-Yes, /very/ familiar. ->2	*/
	maintxt.loadTexture('kitty12',0);
	op1.loadTexture('p1op3',0);
	op1.events.onInputDown.add(phase4, this);
	op2.loadTexture('p1op4',0);
	op2.events.onInputDown.add(phase2, this);
		
}

function phase2 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('hmface',0);
/*	:|
	Oh?
		-Yes, especially feline biology. ->3
		-I mean, I already learned it at my last school. ->4	*/
	maintxt.loadTexture('kitty2',0);
	op1.loadTexture('p2op1',0);
	op1.events.onInputDown.add(phase3, this);
	op2.loadTexture('p2op2',0);
	op2.events.onInputDown.add(phase4, this);
}

function phase3 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('whatface',0);
/*	B|
	...
		-K-kidding!
		-... ->BAD	*/
	maintxt.loadTexture('kitty3',0);
	op1.loadTexture('p3op1',0);
	op1.events.onInputDown.add(phase31, this);
	op2.loadTexture('p3op2',0);
	op2.events.onInputDown.add(badEnding, this);	
	
}

function phase31 ()
{
	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('uhhuhface',0);
/*	BI
	Uh,huh.
		->4	*/
	maintxt.loadTexture('kitty31',0);
	next.events.onInputDown.add(phase4, this);	
}

function phase4 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = true;
	op1.inputEnabled = true;
	op2.visible = true;
	op2.inputEnabled =true;
	op3.visible = true;
	op3.inputEnabled = true;
	face.loadTexture('smallopen',0);
/*	:>
	Okay, well let me know if you have any questions.
		-Actually, can I have your number? ->5
		-You make friends easily, don't you. ->6
		-Yeah, when's lunchtime?	*/

	
	maintxt.loadTexture('kitty4',0);
	op1.loadTexture('p4op1',0);
	op1.y = 460;
	op1.events.onInputDown.add(phase5, this);
	op2.loadTexture('p4op2',0);
	op2.y = 500;
	op2.events.onInputDown.add(phase6, this);
	op3.events.onInputDown.add(phase41, this);
}

function phase41 ()
{
	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('mmface',0);
/*	:I
		At noon. 	*/
	maintxt.loadTexture('kitty41',0);
	next.events.onInputDown.add(phase7, this);	
}

function phase5 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = true;
	op1.inputEnabled = true;
	op2.visible = true;
	op2.inputEnabled =true;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('ohface',0);
/*	:o
	What do you want my number for?
		-You know, for homework and stuff.
		-I collecting pretty-kitty digits.	*/
	maintxt.loadTexture('kitty5',0);
	op1.loadTexture('p5op1',0);
	op1.y = 490;
	op1.events.onInputDown.add(phase51, this);
	op2.loadTexture('p5op2',0);
	op2.y = 530;
	op2.events.onInputDown.add(phase51, this);
}

function phase51 ()
{
	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('hmface',0);
/*	:|
	Um okay.
	<Kitty gives you her phone number.>
		->7				*/
	maintxt.loadTexture('kitty51',0);
	next.events.onInputDown.add(phase7, this);	
}

function phase6 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = true;
	op1.inputEnabled = true;
	op1.y = 490;
	op2.visible = true;
	op2.inputEnabled =true;
	op2.y = 530;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('ohface',0);
/*	:o
	What do you mean?
		-You start talking to me though you barely
		know me. ->8
		-I mean, you seem really popular is all!	*/
	maintxt.loadTexture('kitty6',0);
	op1.loadTexture('p6op1',0);
	op1.events.onInputDown.add(phase8, this);
	op2.loadTexture('p6op2',0);
	op2.events.onInputDown.add(phase61, this); 
}

function phase61 ()
{
	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('closedsmile',0);
/*	^-^
	Oh! Why, thank you!
		->7	*/
	maintxt.loadTexture('kitty61',0);
	next.events.onInputDown.add(phase7, this);
 
}

function phase7 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = true;
	op1.inputEnabled = true;
	op2.visible = true;
	op2.inputEnabled =true;
	op3.visible = true;
	op3.inputEnabled = true;
	face.loadTexture('mmface',0);
/*	<You both sit in silence for a moment.>

	:I
	-*poke her whiskers* ->71
	-*stare* ->8	
	-I'm hungry. ->72	*/
	maintxt.loadTexture('kitty7',0);
	op1.loadTexture('p7op1',0);
	op1.y = 460;
	op1.events.onInputDown.add(phase71, this);
	op2.loadTexture('p7op2',0);
	op2.y = 500;
	op2.events.onInputDown.add(phase8, this);
	op3.loadTexture('p7op3',0);
	op3.events.onInputDown.add(phase72, this);

}

function phase71 ()
{
	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('smallclosed',0);
/*	<3
	Tee-hee, stop that, silly!
		->9	*/
	maintxt.loadTexture('kitty71',0);
	next.events.onInputDown.add(phase9, this);

}

function phase72 ()
{
	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('mmface',0);
/*	:I
	...Yeah...
		->OKAY  */	
	maintxt.loadTexture('kitty72',0);
	next.events.onInputDown.add(okayEnding, this);

}

function phase8 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = true;
	op1.inputEnabled = true;
	op1.y = 490;
	op2.visible = true;
	op2.inputEnabled =true;
	op2.y = 530;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('blush1',0);
/*	o//o
	...do I bother you?
		-Kinda.	
		-No. I don't mind.	*/
	maintxt.loadTexture('kitty8',0);
	op1.loadTexture('p8op1',0);
	op1.events.onInputDown.add(phase81, this);
	op2.loadTexture('p8op2',0);
	op2.events.onInputDown.add(phase82, this); 

}

function phase81 ()
{
	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('sadface',0);
/*	<:'(
	Oh, I'll stop talking to you then.	
		->BAD	*/
	maintxt.loadTexture('kitty81',0);
	next.events.onInputDown.add(badEnding, this);

}

function phase82 ()
{
	body.visible=true;
	face.visible=true;
	maintxt.visible=true;
	textbox.visible=true;
	background.loadTexture('school',0);
	
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = true;
	op2.inputEnabled =true;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('blush2',0);
/*	>//>
	T-that's good.
		-Actually, there's something I've been meaning to ask you.->10
		*/
	
	maintxt.loadTexture('kitty82',0);
	op2.loadTexture('p8op3',0);
	op2.y = 500;
	op2.events.onInputDown.add(phase10, this);

}

function phase9 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = true;
	op1.inputEnabled = true;
	op1.y = 490;
	op2.visible = true;
	op2.inputEnabled =true;
	op2.y = 530;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('opensmile',0);
/*	:)
		-There's something I've been meaning to ask you.-10
		-So, about biology...	kitty9,p9op1,p9op2*/
	maintxt.loadTexture('kitty9',0);
	op1.loadTexture('p9op1',0);
	op1.events.onInputDown.add(phase10, this);
	op2.loadTexture('p9op2',0);
	op2.events.onInputDown.add(phase91, this); 

}

function phase91 ()
{
	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('omgface',0);
/*	0.0
	Oh! Class is starting!	kitty91 */
	maintxt.loadTexture('kitty91',0);
	next.events.onInputDown.add(phase92, this);

}

function phase92 ()
{
	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('opensmile',0);
/*	:)
	We'll talk later, okay?
		->OKAY		kitty92*/
	maintxt.loadTexture('kitty92',0);
	next.events.onInputDown.add(okayEnding, this);

}

function phase10 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = true;
	op1.inputEnabled = true;
	op1.y = 490;
	op1.x = 100;
	op2.visible = true;
	op2.inputEnabled =true;
	op2.x = 100;
	op2.y = 530;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('ohface',0);
/*	:o
	What is it?
		-Do you get the feeling that we've known each other?
		-Do you think I'm cute?		*/
	maintxt.loadTexture('kitty10',0);
	op1.loadTexture('p10op1',0);
	op1.events.onInputDown.add(phase101, this);
	op2.loadTexture('p10op2',0);
	op2.events.onInputDown.add(phase104, this); 

}

function phase101 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = true;
	op2.inputEnabled = true;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('blush1',0);
/*	o//o
	I...Yes! I do!
		-And that we were made for each other?!	kitty101,p101op1*/
	maintxt.loadTexture('kitty101',0);
	op2.loadTexture('p101op1',0);
	op2.y = 500;
	op2.events.onInputDown.add(phase102, this);

}
function phase102 ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = true;
	op2.inputEnabled = true;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('blush3',0);
/*	0//0
	Yes! I feel like...like you're the one for me!
		-Kitty!			kitty102,p102op1*/
	maintxt.loadTexture('kitty102',0);
	op2.loadTexture('p102op1',0);
	op2.y = 500;
	op2.events.onInputDown.add(phase103, this);

}
function phase103 ()
{	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('blush3',0);
/*	T//T
	S-sempai!
		->GOOD		kitty103*/
	maintxt.loadTexture('kitty103',0);
	next.events.onInputDown.add(goodEnding, this);

}
function phase104 ()
{
	next.inputEnabled = true;
	next.visible = true;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	face.loadTexture('sweatdrop',0);
/*	^^'
	Um..Oh! Class is starting!	kitty104*/
	maintxt.loadTexture('kitty104',0);
	next.events.onInputDown.add(phase92, this);

}

function badEnding ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	body.visible=false;
	face.visible=false;
	maintxt.visible=false;
	textbox.visible=false;
	background.loadTexture('badending',0);

}

function okayEnding ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	body.visible=false;
	face.visible=false;
	maintxt.visible=false;
	textbox.visible=false;
	background.loadTexture('okayending',0);
}

function goodEnding ()
{
	next.inputEnabled = false;
	next.visible = false;
	op1.visible = false;
	op1.inputEnabled = false;
	op2.visible = false;
	op2.inputEnabled =false;
	op3.visible = false;
	op3.inputEnabled = false;
	body.visible=false;
	face.visible=false;
	maintxt.visible=false;
	textbox.visible=false;
	background.loadTexture('goodending',0);
}

