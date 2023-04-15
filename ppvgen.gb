'      

'

'Note - NEWS ITEMS

'new feature for this version :)

'see lines 2600 onwards for examples of how to enter additional news items :)

'




dim f1,f2,f3,f4     
f1=loadtexture("font1.png")
font(f1)       
color(0,0,0)
textmode(text_buffered)  
resizetext(50,35)
f2=loadtexture("back.jpg") 
f3=loadtexture("back2.jpg")  
f4=loadtexture("back3.jpg")  
resizespritearea(400,300)
newsprite(f2) 
sprsetpos(400,300)
sprsetsize(400,300)
sprsetvisible(1)    

dim x,y,z,x2,y2,z2,x#,y#,z#,x3,y3,z3,x2#,y2#,z2#,rostersiz
dim i$,page,pscreen,currw,currb,currf,currfd,currm,totalm 
dim bi(256)(5)
dim bn,cgrp,csiz,gsiz,bt$,bl,by,sel,sel2 
dim bu$(256)
dim mx,my,ml,mw  
dim tmrule(22)(2),totaltm         
dim f,chk$           
dim timeout
dim house       
dim major 
dim size 
dim highlight 
dim belttry(8),belttryo(8),belts,beltsorig     
dim options(4),totopt
dim prom$:prom$="WWE"
dim star,stars             
dim slots(8),slot$(8)  
dim ruleslots(8),ruleslot$(8)

dim head$(48):dim new$(48):dim news,news2,currline,temp$

dim hist$(24)(300)
dim lines(24)
for x=1 to 24:for y=1 to 300:hist$(x)(y)="*":next:next
dim tothist:tothist=0  
dim realshow:realshow=0

dim table2(10):table2(1)=1

dim match(12)(11)  
dim stip(12)(3)
dim entry(12)(8)
dim text$(12)(26)     
dim chosen(64):dim left 
dim side$(12)(8)     
dim tried(12)
dim side(8)   
          
dim mode:mode=1          

dim table(21)(6)
for x=1 to 21:for y=1 to 6:read table(x)(y):next:next 
data 100,999,95,1,-19,-9
data 90,99,95,1,-19,-9
data 80,89,90,2,-18,-8
data 70,79,85,3,-17,-7
data 60,69,80,4,-16,-6
data 50,59,75,5,-15,-5
data 40,49,70,6,-14,-4
data 30,39,65,7,-13,-3
data 20,29,60,8,-12,-2
data 10,19,55,9,-11,-1
data -9,9,50,10,-10,0
data -19,-10,45,11,-9,1
data -29,-20,40,12,-8,2
data -39,-30,35,13,-7,3
data -49,-40,30,14,-6,4
data -59,-50,25,15,-5,5
data -69,-60,20,16,-4,6
data -79,-70,15,17,-3,7
data -89,-80,10,18,-2,8
data -99,-90,5,19,-1,9
data -999,-100,5,19,-1,9   
      
dim mrule(22),ma$(22) 
for x=0 to 22:read ma$(x):read mrule(x):next 
data "Regular",1
data "Gruesome Fighting",3,"Cage (Escape)",2,"Cage (Pinfall)",2
data "Exploding Deathmatch",3,"Landmine Deathmatch",3
data "BRoyal: Elim",2,"BRoyal: Elim+Over Top",2
data "BRoyal: 1stF SuddenDeath",2
data "BRoyal: Timed Entry",2,"BRoyal: Timed Entry+Over Top",2
data "2 Count",3,"3 Count",1,"Pinfall Only - no subm",2,"Submission Only - no pin",2
data "One Match",1,"Best Of 3",2,"DQ On",1,"DQ Off",2
data "Team - Eliminate all",2,"Team - 1st Fall",1,"Team - Tag",1,"Team - Tornado",2

dim xrule(11):for x=1 to 11:read xrule(x):next
data 2,1,2,2,2,2,2,2,2,1,1

dim belt$(8) 
dim bused(8)
dim bd(8)(4)
dim bh(8)(4)  
dim bmrule(8)(22)
for x=1 to 8
 read belt$(x)
 for y=1 to 4:read bd(x)(y):next
 for y=0 to 22:bmrule(x)(y)=1:next
 for y=1 to 4:bh(x)(y)=0:next
next 
data "WWE",1,1,1,1
data "World Hvy",1,1,1,1     
data "Inter/cont",1,2,1,1
data "US",1,2,1,1
data "ECW",1,2,1,1  
data "WWE Womens",1,3,3,1 
data "WWE Tag Tm",1,3,1,2
data "Wor Tag Tm",1,3,1,2 
bmrule(5)(17)=2
bh(1)(1)=2
bh(2)(1)=8
bh(3)(1)=12
bh(4)(1)=46
bh(5)(1)=19   
bh(6)(1)=38 
bh(7)(1)=31:bh(7)(2)=44
bh(8)(1)=45:bh(8)(2)=33 

dim wre$(64)  
dim orig(64)
dim wd(64)(6) 
  
for x=1 to 48
 read wre$(x)
 for y=1 to 6:read wd(x)(y):next     
next     

data "John Cena",1,170,1,1,1,1       
data "Triple H",1,152,1,1,2,1 
data "Snitsky",1,77,1,1,2,1 
data "Edge",1,157,1,2,2,1
data "Randy Orton",1,141,1,1,2,1  
data "Batista",1,141,1,1,1,1    
data "Shawn Michaels",1,145,2,2,1,1  
data "Chris Jericho",1,139,2,1,2,1  
data "The Great Khali",1,110,1,1,2,1 
data "The Big Show",1,134,1,2,2,2   
data "Rey Mysterio Jnr",1,128,2,1,1,1 
data "William Regal",1,122,1,1,3,1  
data "MVP",1,96,1,1,1,1 
data "Jeff Hardy",1,131,2,2,1,1   
data "Kane",1,125,1,2,1,2     
data "JB Layfield",1,124,1,1,2,1    
data "Mark Henry",1,88,1,1,2,1        
data "Chavo Guerrero",1,116,2,3,2,2   
data "Matt Hardy",1,102,2,2,3,1   
data "Big Daddy V",1,127,1,1,3,1 
data "John Morrison",1,106,2,3,3,2 
data "Mike Mizanin",1,92,1,3,3,2  
data "Bob Holly",1,97,1,3,2,1 
data "Cody Rhodes",1,79,1,3,2,1   
data "Paul London",1,100,2,3,1,1   
data "Brian Kendrick",1,98,2,3,1,1   
data "Curt Hawkins",1,61,1,3,2,1  
data "Zach Ryder",1,60,1,3,2,1 
data "Rob McAllister",1,71,1,3,3,1    
data "Rory McAllister",1,67,1,3,3,1   
data "Carlito",1,114,2,3,2,1
data "Santino Marella",1,70,1,3,2,1   
data "CM Punk",1,115,2,2,1,2
data "Funaki",1,63,2,2,3,1    
data "Mr Kennedy",1,113,1,2,2,1   
data "Finlay",1,120,1,2,3,1
data "Mickie James",1,50,3,2,3,3     
data "Beth Phoenix",1,40,3,2,3,3
data "Victoria",1,30,3,2,3,3
data "Ashley",1,0,3,2,3,3
data "Melina",1,10,3,2,3,3
data "Maria",1,20,3,2,3,3 
data "The Undertaker",1,160,1,1,1,1    
data "Primo",1,80,1,3,2,1 
data "Kofi Kingston",1,115,1,3,1,1
data "Shelton Benjamin",1,120,1,1,1,1
data "Kelly Kelly",1,15,3,2,3,3
data "Vladimir Kozlov",1,135,1,1,2,1
    
for x=49 to 64
 read wre$(x)
 for y=1 to 6:read wd(x)(y):next     
next

data "Hulk Hogan",1,145,1,2,1,1
data "Vince McMahon",1,130,1,2,2,2
data "Shane McMahon",1,115,2,2,2,2
data "Floyd Mayweather",1,133,2,1,1,4
data "Mick Foley",1,100,1,2,3,2
data "Steve Austin",1,150,1,1,1,1
data "Stephanie McMahon",1,50,3,2,2,3 
data "Honky Tonk Man",1,66,1,1,3,1
data "Roddy Piper",1,75,1,2,1,1
data "Jim Duggan",1,75,1,2,1,1
data "Ron Simmons",1,125,1,2,1,1  
data "Brock Lesnar",1,170,1,1,3,4 
data "Ric Flair",1,135,1,1,1,1
data "K-Fed",1,50,1,2,2,1 
data "Kurt Angle",1,185,1,1,1,1
data "Jerry Lawler",1,75,1,2,2,1  

for x=1 to 64               
 orig(x)=wd(x)(2)
next    
    
dim fa$(24)
dim fm(24)(4) 
for x=1 to 24:fa$(x)="Unnamed":next
fa$(1)="La Familia"
fa$(2)="The Highlanders"       
fa$(3)="Kendrick/London"
fa$(4)="Carlito/Primo"    
fa$(5)="Holly/Rhodes"
fa$(6)="Morrison/Mizanin"   
fa$(7)="Kingston/Punk" 
fa$(8)="McMahon Family"

fm(1)(1)=4
fm(1)(2)=18
fm(1)(3)=27
fm(1)(4)=28  
fm(2)(1)=29
fm(2)(2)=30
fm(3)(1)=25
fm(3)(2)=26
fm(4)(1)=31
fm(4)(2)=44
fm(5)(1)=23
fm(5)(2)=24
fm(6)(1)=21
fm(6)(2)=22 
fm(7)(1)=45
fm(7)(2)=33 
fm(8)(1)=50
fm(8)(2)=51
fm(8)(3)=55

dim wrefac(64)(24)

for x=1 to 12
 for y=1 to 26:text$(x)(y)="*":next
 for y=1 to 8:side$(x)(y)="*":next
next     

gosub checksort 
gosub checkspecsort
gosub setuptitlefactions

editmenu:   
gosub clear     
printr "*PPVGen 2.2* - Main Menu"
gsiz=1:bl=0
bt$="-MatchType Settings":by=23:gosub button 
bt$="-Edit Roster":by=14:gosub button    
bt$="-Edit Factions":by=18:gosub button 
bt$="-Edit Championships":by=12:gosub button    
bt$="Save":by=34:bl=0:gosub button        
bt$="Load":by=34:bl=5:gosub button
bt$="-Generate Regular Show":by=25:bl=0:gosub button  
bt$="-Generate PPV":by=27:bl=0:gosub button 
bt$="-Generate Major PPV":by=29:bl=0:gosub button 
bt$="-Promotion "+prom$:by=10:bl=0:gosub button 
bt$="-ABOUT":by=4:bl=0:gosub button  
bt$="-Edit Special Roster":by=16:bl=0:gosub button 
if xrule(11)=0 then bt$="-News Items Disabled" else bt$="-News Items Enabled":endif 
by=6:bl=0:gosub button

drawtext() 
do
 gosub mouse  
 if sel=12 then goto special:endif 
 if sel=11 then
  gosub clear     
  printr "FireProR PPV Generator 2.2, by *Sad Git*, 2008":printr
  printr"Contact: udispc@yahoo.co.uk":printr 
  printr"FPR community: http://www.fireproclub.com/forum":printr
  printr"All BLUE onscreen text is clickable.":printr
  printr"Edit your promotion data and generate shows!":printr
  printr"See Readme file for full instructions..."
    
  drawtext()  
  gosub mouse
  goto editmenu 
 endif
 if sel=6 then   
  gosub loadgame
  if mode=1 then goto editmenu else goto showmenu:endif
 endif
 if sel=5 then    
  gosub savegame 
  goto editmenu
  endif    
 if sel=10 then
  cls
  printr "Enter a name for your Promotion":printr
  printr"(Or enter a blank field to return without change)":printr
  drawtext()
  color(0,0,128)
  input ">",i$
  color(0,0,0)
  if i$<>"" then prom$=left$(i$,35):endif 
  goto editmenu
 endif          
 if sel=13 then
  if xrule(11)=1 then xrule(11)=0:goto editmenu:endif
  xrule(11)=1:goto editmenu
 endif
 if sel=1 then  
  gosub promrules
  goto editmenu      
 endif 
 if sel=4 then goto belts:endif
 if sel=2 then page=1:goto roster:endif 
 if sel=3 then currf=1:goto factions:endif  
 if sel>6 and sel<10 then
  mode=2
  if sel=7 then house=1 else house=0:endif
  if sel=9 then major=1 else major=0:endif
  goto news
 endif 
loop 
 
card:  
for x=1 to 64
 for y=1 to 24
  wrefac(x)(y)=0
  for z=1 to 4
   if fm(y)(z)=x then wrefac(x)(y)=1:endif
  next    
 next
next

for x=1 to 10 
 for y=1 to 26:text$(x)(y)="*":next
 for y=1 to 8:side$(x)(y)="*":next
 for y=1 to 11:match(x)(y)=0:next  
 for y=1 to 8:entry(x)(y)=0:next  
 tried(x)=0
next  
totalm=0:left=0:stars=0
for x=1 to 64
chosen(x)=0
if wd(x)(1)=1 then 
 left=left+1
 if x>48 then stars=stars+1:endif
endif 
next      
if left<8 then 
 gosub clear                    
 printr "Please enable at least 8 wrestlers in your roster"
 printr "and try again."    
 drawtext()
 gosub mouse
 goto editmenu
endif    

'find size,rostersiz
rostersiz=(left-stars)   
for x=1 to 8:bused(x)=0:next
if major=0 then size=rnd()%3+14 else size=20:endif  

'set up table: roster position - ideal card position  
for x=2 to size                  
 y=(x-1):z=(size-1)
 x#=rostersiz-1
 x#=x#/z:x#=x#*y:x#=x#+1
 gosub fraction
 table2(x)=x#
next  

x=1
nextmatch:
if left<8 or x>size then   
 '(finalise)
 'rearrange matches  
 
 for y2=1 to totalm
 for x=1 to (totalm-1)
  'average rating
  x#=0:z#=0  
 
  for z=1 to match(x)(11)
   x2=entry(x)(z)
   x#=x#+wd(x2)(2)
  next      
  y#=match(x)(11)
  x#=x#/y#  

  for z=1 to match(x+1)(11)
   x2=entry(x+1)(z)
   z#=z#+wd(x2)(2)
  next 
  y#=match(x+1)(11)
  z#=z#/y#      
 
  if z#>x# then 
  
    'titles keep proper spot  
    
    x2#=1
    
    if match(x)(10)>0 then
     if bd(match(x)(10))(2)=1 and x>1 then x2#=0:endif
     if bd(match(x)(10))(2)=2 and x>5 then x2#=0:endif
    endif
    if match(x+1)(10)>0 then
     if bd(match(x+1)(10))(2)=2 and x<3 then x2#=0:endif  
     if bd(match(x+1)(10))(2)=3 and x<5 then x2#=0:endif  
    endif 
    
    'swap
  
    if x2#=1 then
    for y=1 to 11
     match(0)(y)=match(x+1)(y):match(x+1)(y)=match(x)(y):match(x)(y)=match(0)(y)
    next
    for y=1 to 8
     entry(0)(y)=entry(x+1)(y):entry(x+1)(y)=entry(x)(y):entry(x)(y)=entry(0)(y)
    next
    for y=1 to 3
     stip(0)(y)=stip(x+1)(y):stip(x+1)(y)=stip(x)(y):stip(x)(y)=stip(0)(y)
    next
    for y=1 to 8
     side$(0)(y)=side$(x+1)(y):side$(x+1)(y)=side$(x)(y):side$(x)(y)=side$(0)(y)
    next
    for y=1 to 26
     text$(0)(y)=text$(x+1)(y):text$(x+1)(y)=text$(x)(y):text$(x)(y)=text$(0)(y)
    next
    endif

  endif

 next  
 next  

 currm=1
 if xrule(11)=1 then gosub cardnews:endif
 goto showmenu
endif
timeout=0   
star=0

beltsorig=0
for y=1 to 8
 x3=1
 'Main title      
 if bd(y)(2)=1 and x>2 then x3=0:endif 
 if bd(y)(2)=1 and house=1 then x3=0:endif 
 'Midcard title
 if bd(y)(2)=2 and x<3 then x3=0:endif 
 if bd(y)(2)=2 and x>6 then x3=0:endif 
 'ucard title
 if bd(y)(2)=3 and x<5 then x3=0:endif 
 'champs available
 for z=1 to (bd(y)(4))
  if bh(y)(z)>0 then
   if wd(bh(y)(z))(1)=0 or chosen(bh(y)(z))=1 then x3=0:endif
  endif
 next
 'Sing/Tag settings correct    
  if bd(y)(4)=1 and xrule(1)=5 then x3=0:endif
  if bd(y)(4)>1 then
   if xrule(1)=1 then x3=0:endif
   if xrule(bd(y)(4))=3 then x3=0:endif
  endif
 'belt valid
 if bd(y)(1)=1 and bused(y)=0 and x3=1 then 
  belttryo(y)=1:beltsorig=beltsorig+1  
 else 
  belttryo(y)=0
 endif 

next

trymatch:    
  
for y=1 to 8:belttry(y)=belttryo(y):next
belts=beltsorig
     
timeout=timeout+1 
'for reference
tried(x)=tried(x)+1       
'safety cut-out
if timeout>500 then 
 currm=1
 if xrule(11)=1 then gosub cardnews:endif
 goto showmenu
endif  

'sing/team?  
x3=rnd()%4 'no show weighting for s/t
x3=x3+xrule(1) 
if x3>4 then match(x)(2)=2 else match(x)(2)=1:endif 

matchbase:

'base type 
if match(x)(2)=1 then
 x3=rnd()%5
 if x3=0 then match(x)(1)=0:endif 
 if x3=1 then match(x)(1)=1:endif 
 if x3=2 then match(x)(1)=rnd()%2+2:endif
 if x3=3 then match(x)(1)=rnd()%2+4:endif 
 if x3=4 then match(x)(1)=rnd()%5+6:endif
else
 x3=rnd()%3
 if x3=0 then match(x)(1)=0:endif
 if x3=1 then match(x)(1)=rnd()%2+2:endif
 if x3=2 then match(x)(1)=rnd()%2+4:endif
endif

'proscribed/rare base rules
if mrule(match(x)(1))=3 then goto trymatch:endif
if mrule(match(x)(1))=2 then 
 if house=1 and rnd()%64>0 then goto trymatch:endif   
 if house=0 and major=0 and rnd()%16>0 then goto trymatch:endif
 if house=0 and major=1 and rnd()%4>0 then goto trymatch:endif
endif     

if match(x)(2)=1 then  
 'singles match    
 match(x)(7)=0
 match(x)(8)=0
 '# of competitors
 if match(x)(1)<6 then match(x)(3)=2:endif
 if match(x)(1)=6 then match(x)(3)=4:endif       
 if match(x)(1)=7 then match(x)(3)=(rnd()%3+2)*2:endif
 if match(x)(1)=8 then match(x)(3)=rnd()%2+3:endif 
 if match(x)(1)=9 then match(x)(3)=6:endif
 if match(x)(1)=10 then match(x)(3)=8:endif 
 match(x)(11)=match(x)(3)
 '# of falls    
 matchfalls:
 if match(x)(1)=0 and match(x)(3)=2 then 
  gosub getx3  
  x3=x3+xrule(6) 
  if x3>4 then match(x)(5)=2 else match(x)(5)=1:endif 
 else 
  match(x)(5)=1
 endif 
endif  

if match(x)(2)=2 then 
 'numbers     
  totopt=0
  for x3=2 to 5
   if xrule(x3)<3 then 
    totopt=totopt+1
    options(totopt)=x3-1
   endif
  next
  if totopt=0 then goto trymatch:endif    
  weighting:
   x3=options(rnd()%(totopt)+1)
   if xrule(x3+1)=2 and rnd()%8>0 then goto weighting:endif
   if x3<4 then
    match(x)(3)=x3
    match(x)(11)=((match(x)(3)+1)*2) 
   else            
    z2=rnd()%100+1
    if z2<91 then match(x)(3)=4:endif 
    if z2>90 and z2<100 then match(x)(3)=5:endif 
    if z2=100 then match(x)(3)=6:endif 
    match(x)(11)=(match(x)(3)-1)
   endif
 'team rules and settings   
 match(x)(5)=1 
 'survivor series?  
 if match(x)(1)=2 or match(x)(1)=3 then  
  match(x)(7)=2
 else
  gosub getx3  
  x3=x3+xrule(8) 
  if x3>4 then match(x)(7)=1 else match(x)(7)=2:endif
 endif
 ttmatch:
 'tag/tornado
 if match(x)(1)=0 then 
  gosub getx3  
  x3=x3+xrule(9) 
  if x3>4 then match(x)(8)=2 else match(x)(8)=1:endif
 else 
  match(x)(8)=2
 endif 
endif 

falltype:  
if match(x)(1)=2 then 
 match(x)(4)=5   
else    
 totopt=0
 for x3=11 to 14
  z3=0
  if mrule(x3)=1 then z3=1:endif
  if mrule(x3)=2 then 
   if house=1 and rnd()%64=0 then z3=1:endif
   if house=0 and major=0 and rnd()%16=0 then z3=1:endif
   if house=0 and major=1 and rnd()%4=0 then z3=1:endif
  endif
  if z3=1 then
   totopt=totopt+1
   options(totopt)=x3-10
  endif 
 next
 if totopt=0 then goto trymatch:endif  
 match(x)(4)=options(rnd()%(totopt)+1)
endif
if match(x)(1)=1 then match(x)(4)=4:endif
  
dqtype:
'dq                    
x3=rnd()%4 'no show weighting for dq
x3=x3+xrule(7) 
if x3>4 then match(x)(6)=2 else match(x)(6)=1:endif
if match(x)(1)>0 and match(x)(1)<6 then match(x)(6)=2:endif
if match(x)(1)=8 then match(x)(6)=2:endif  

'belt rules  
x3=1          
for y2=1 to 8
 if belttry(y2)=1 then 
  'singles belt
  if bd(y2)(4)=1 then
   if match(x)(2)=2 then x3=0:endif
  else
   'team belt
   if match(x)(2)=1 then x3=0:endif 
   if match(x)(3)>3 then x3=0:endif
   z=bd(y2)(4):z=z*2
   if match(x)(11)<>z then x3=0:endif
  endif  
  'match types   
  if bmrule(y2)(match(x)(1))<>1 then x3=0:endif 
  if match(x)(4)<5 then
   if bmrule(y2)(match(x)(4)+10)<>1 then x3=0:endif
  endif       
  if match(x)(5)>0 and bmrule(y2)(match(x)(5)+14)<>1 then x3=0:endif
  if bmrule(y2)(match(x)(6)+16)<>1 then x3=0:endif
  if match(x)(7)>0 and bmrule(y2)(match(x)(7)+18)<>1 then x3=0:endif
  if match(x)(8)>0 and bmrule(y2)(match(x)(8)+20)<>1 then x3=0:endif  
  'remove belt
  if x3=0 then belttry(y2)=0:belts=belts-1:endif
 endif
next

'no belt left       
if belts=0 and beltsorig>0 and house=0 and rnd()%32>0 then goto trymatch:endif 
                    
y=1      
pickloop:
 y3=0
 x#=0     
 for y#=1 to 64      
   
  'legend?
  if y#>48 then
   if house=1 or major=0 or x<3 or match(x)(1)>6 then goto endloop:endif
   'legend reduce chance
   z#=rnd()%(stars*6)
   if z#>stars then
    goto endloop
   endif
  endif  

  if chosen(y#)=1 then goto endloop:endif
  if wd(y#)(1)=2 then goto endloop:endif  
     
  'restrict mix gender if woman not highly rated
  if y>1 then         
   for z2=1 to (y-1)   
    z3=(entry(x)(z2))
    if wd(y#)(3)=3 then
     if wd(z3)(3)<3 and wd(y#)(2)<100 then goto endloop:endif
    else
     if wd(z3)(3)=3 and wd(z3)(2)<100 then goto endloop:endif
    endif
   next   
  endif   
  
  if match(x)(3)>3 then   
   'handicap restrictions
   if y>1 then 
    if wd(entry(x)(1))(2)<wd(y#)(2) then goto endloop:endif   
   endif
  endif
  
  if y=2 and match(x)(2)=1 and match(x)(11)=2 then
   '1v1 not between faction or side   
   if wd(y#)(5)<>3 and wd(y#)(5)=wd(entry(x)(1))(5) then goto endloop:endif
   for x2=1 to 24    
    if wrefac(y#)(x2)=1 and wrefac(entry(x)(1))(x2)=1 then goto endloop:endif 
   next
  endif 
  
  'suitability rating
  
  x2=y#
           
  if y#>48 then 
  'legend find spot
   for x2=1 to rostersiz
    if (wd(y#)(2))>=(wd(x2)(2)) then goto found:endif
   next 
   x2=rostersiz
   found:    
   
   'legend high randomize
   x2=x2+(rnd()%(rostersiz))
   x2=x2-(rnd()%(rostersiz)) 
   if x2<1 then x2=1:endif
   if x2>rostersiz then x2=rostersiz:endif   

  endif 
  
  'calculate

  z#=rostersiz
  x2=x2-table2(x):x2=abs(x2)
  z#=z#-x2  
  z#=z#/rostersiz
  z#=z#*48    
        
  'team match factions
  if match(x)(2)=2 and y>1 then    
  
   if match(x)(3)>3 then   

    'handicap matches   
    'sides
    if wd(y#)(5)<>3 then
     if wd(y#)(5)=wd(entry(x)(1))(5) then goto endloop:endif 'opponent 
     'face/heel same side
     if y>2 then
      for y2=2 to (y-1)
       if wd(y#)(5)=1 and wd(entry(x)(y2))(5)=2 then goto endloop:endif 
       if wd(y#)(5)=2 and wd(entry(x)(y2))(5)=1 then goto endloop:endif 
      next
     endif
    endif
    'factions
    z=0
    z2=0        
    for x2=1 to 24     
     if wrefac(y#)(x2)=1 then 
      z=1
      if wrefac(entry(x)(1))(x2)=1 then goto endloop:endif 'single wrestler's faction
      if y>2 then
       for y2=2 to (y-1)   
        if wrefac(entry(x)(y2))(x2)=1 then 
         z2=1:z#=z#+64 
        endif   'existing team entrant faction
       next
      endif              
     endif
    next                   
    'no teammates in match
    if z=1 and z2=0 then  
     if y=match(x)(11) then goto endloop:endif ' last entrant 
    endif

   else          

    'tag matches
    if y<=(match(x)(11)/2) then x3=1 else x3=2:endif   
    'sides
    if wd(y#)(5)<>3 then
     for y2=1 to (y-1)           
      if y2<=(match(x)(11)/2) then z3=1 else z3=2:endif    
      if x3=z3 then     
      'teammates
       if wd(y#)(5)<>wd(entry(x)(y2))(5) then goto endloop:endif
      else
      'opponents 
       if wd(y#)(5)=wd(entry(x)(y2))(5) then goto endloop:endif
      endif
     next
    endif
    'factions   
    z=0 
    z2=0  
    for x2=1 to 24     
     if wrefac(y#)(x2)=1 then
      z=1
      for y2=1 to (y-1) 
       if wrefac(entry(x)(y2))(x2)>0 then   
        if y2<=(match(x)(11)/2) then z3=1 else z3=2:endif 
        if x3=z3 then
         'faction teammate, same
         z2=1:z#=z#+64
        else
         'faction teammate, opposite
         goto endloop
        endif
       endif
      next  
     endif
    next
    'last entrant no teammates
    if y=match(x)(11) or y=(match(x)(3)+1) then
     if z=1 and z2=0 then goto endloop:endif 
    endif

   endif 
   
  endif  
  
  if house=1 then z#=z#+rnd()%256:endif
  if house=0 and major=0 then z#=z#+rnd()%64:endif       
  if house=0 and major=1 then z#=z#+rnd()%16:endif
  
  'normal wrestlers
  if wd(y#)(6)=1 then
   if match(x)(1)=1 then z#=z#-16:endif
  endif
  'h/core wrestlers
  if wd(y#)(6)=2 then
   if match(x)(6)=1 then z#=z#-8 else z#=z#+8:endif
  endif
  'pure wrestlers
  if wd(y#)(6)=3 then
   if match(x)(6)=2 then z#=z#-8 else z#=z#+8:endif
  endif
  'MMartists
  if wd(y#)(6)=4 then
   if match(x)(1)<>1 then z#=z#-8 else z#=z#+16:endif  
   if match(x)(6)=1 then z#=z#-8:endif
  endif  
  
  'neutral side penalty
  if wd(y#)(5)=3 then z#=z#-4:endif
 
  'valid titleholder 
  z3=0
  for x2=1 to 8
   for x3=1 to 4
    if bh(x2)(x3)=y# and belttry(x2)=1 then z3=1:endif
   next
  next
  if z3=1 then z#=z#+8:endif
  
  'cruiser(woman)/heavy already in match bias
  if y>1 then  
   x2=wd(y#)(3):if x2=3 then x2=2:endif   
   x3=wd(entry(x)(1))(3):if x3=3 then x3=2:endif
   if x2=x3 then z#=z#+8:endif
  endif   

  'tag/single pref
  if wd(y#)(4)=3 then 
   if match(x)(2)=2 and match(x)(3)<4 then z#=z#+16:endif
   if match(x)(2)=2 and match(x)(3)>3 and y<>1 then z#=z#+16:endif
  endif    
  if wd(y#)(4)=1 then 
   if match(x)(2)=1 then z#=z#+16:endif
   if match(x)(2)=2 and match(x)(3)>3 and y=1 then z#=z#+16:endif
  endif  
  if wd(y#)(4)=2 then z#=z#+16:endif 
  
  'enter wrestler in match
  if z#>x# then y3=y#:x#=z#:endif       
  ' don't enter
  endloop:    

 next    

 if y3>0 then     
  left=left-1:chosen(y3)=1:entry(x)(y)=y3  
  if y3>48 then star=1:endif
 else 
  goto redomatch     
 endif 

if y<match(x)(11) then 
 y=y+1
 goto pickloop 
endif  

'double check factions (for all except last entrant in team) 
if match(x)(2)=2 then
 if match(x)(3)>3 then  
  for y=2 to (match(x)(11)-1) 
   x#=0:y#=0
   for z=1 to 24
    if wrefac(entry(x)(y))(z)=1 then  
     x#=1     
     for y2=2 to (match(x)(11))
      if y2<>y then
       if wrefac(entry(x)(y2))(z)=1 then y#=1:endif
      endif
     next
    endif
   next 
   if x#=1 and y#=0 then goto redomatch:endif
  next
 else
  for y=1 to (match(x)(11))  
   x#=0:y#=0
   for z=1 to 24
    if wrefac(entry(x)(y))(z)=1 then 
     x#=1    
     if y>(match(x)(11)/2) then
      x2=(match(x)(11)/2)+1:x3=match(x)(11)
     else
      x2=1:x3=(match(x)(11)/2)
     endif
     for y2=x2 to x3
      if y2<>y then
       if wrefac(entry(x)(y2))(z)=1 then y#=1:endif
      endif
     next
    endif
   next
   if x#=1 and y#=0 then goto redomatch:endif 
  next
 endif
endif


'belt by entrants   
 
if star>0 then
 'legend in match (no title)
  goto stips
endif

for y2=1 to 8   
 if belttry(y2)=1 then     
  x3=1  
  
  'heavy belt restrict
  if bd(y2)(3)=4 then
   for z=1 to match(x)(11)
    if wd(entry(x)(z))(3)<>1 then x3=0:endif
   next
  endif  
  'cruiserweight belt restrict
  if bd(y2)(3)=2 then
   for z=1 to match(x)(11)
    if wd(entry(x)(z))(3)=1 then x3=0:endif
   next
  endif  
 'women's belt restrict  
  if bd(y2)(3)=3 then
  for z=1 to match(x)(11)
   if wd(entry(x)(z))(3)<>3 then x3=0:endif
  next
  endif

 'existing belt holder in match 
  if bh(y2)(1)>0 then
   if match(x)(2)=1 then     
    y=0
    for z=1 to (match)(x)(11)
     if entry(x)(z)=bh(y2)(1) then y=1:endif
    next 
    if y=0 then x3=0:endif
   else 
    y=0        
    'side 1  
    y3=0
    for z=1 to (bd(y2)(4))
     for z3=1 to (bd(y2)(4))  
      if bh(y2)(z)=entry(x)(z3) then y3=y3+1:endif
     next
    next 
    if y3=(bd(y2)(4)) then y=1:endif
    'side 2  
    y3=0
    for z=1 to (bd(y2)(4))
     for z3=(1+(bd(y2)(4))) to ((bd(y2)(4))*2)  
      if bh(y2)(z)=entry(x)(z3) then y3=y3+1:endif
     next
    next 
    if y3=(bd(y2)(4)) then y=1:endif     
    'team champions check      
    if y=0 then x3=0:endif 
   endif   
  endif          

  if x3=0 then belttry(y2)=0:belts=belts-1:endif
 endif      
next          

'no belt left      
if belts=0 and beltsorig>0 and house=0 and rnd()%32>0 then goto redomatch:endif
 
'assign belt  
if belts>0 then      
 do
  y2=rnd()%8+1          
  if belttry(y2)=1 then   
   match(x)(10)=y2
   bused(y2)=1 
   goto stips
  endif 
 loop
endif

stips:    

'randomise timed BR entry  
if match(x)(1)=9 or match(x)(1)=10 then
 for y=1 to (match(x)(11))
  z=rnd()%(match(x)(11))+1
  z2=rnd()%(match(x)(11))+1
  x2=entry(x)(z)
  entry(x)(z)=entry(x)(z2)
  entry(x)(z2)=x2
 next
endif  

stip(x)(1)=0   

if star=1 then goto finishmatch:endif 

'losergetsfired stip

if match(x)(2)=1 and match(x)(11)=2 and xrule(11)=1 and house=0 then  
 if major=0 then y=80:endif  
 if major=1 then y=20:endif  
 if rnd()%y=0 then stip(x)(1)=1:endif
endif   

'losing factions stip

if match(x)(2)=2 and match(x)(3)<4 and xrule(11)=1 then 
 x3=0:z3=0 
 for x2=1 to 16 
  y2=0:y3=0
  for y=1 to (match(x)(11))        
   if wrefac(entry(x)(y))(x2)=1 then     
    if y>(match(x)(11)/2) then y3=y3+1 else y2=y2+1:endif 
   endif
  next
  if y2=(match(x)(11)/2) then x3=x2:endif 
  if y3=(match(x)(11)/2) then z3=x2:endif    
 next  
 if x3>0 and z3>0 then  
  if house=1 then y=160:endif  
  if house=0 and major=0 then y=40:endif  
  if house=0 and major=1 then y=10:endif  
  if rnd()%y=0 then stip(x)(1)=2:stip(x)(2)=x3:stip(x)(3)=z3:endif
 endif
endif   

finishmatch:

y=1 
if match(x)(10)>0 then text$(x)(y)=text$(x)(y)+"*"+ucase$(belt$(match(x)(10)))+" CHAMPIONSHIP*":y=y+2:endif   
if stip(x)(1)=1 then text$(x)(y)=text$(x)(y)+"*LOSER GETS FIRED!*":y=y+2:endif 
if stip(x)(1)=2 then text$(x)(y)=text$(x)(y)+"*LOSING GROUP MUST SPLIT UP!*":y=y+2:endif             
if match(x)(2)=1 then   
 text$(x)(y)=text$(x)(y)+"(SINGLES" 
else 
 if match(x)(3)<4 then text$(x)(y)=text$(x)(y)+"("+(match(x)(11))+"-MAN TAG" else text$(x)(y)=text$(x)(y)+"(HANDICAP 1 V "+(match(x)(3)-2):endif
endif              
if match(x)(1)=0 then 
 text$(x)(y)=text$(x)(y)+")":y=y+1
else 
 text$(x)(y)=text$(x)(y)+" / "
endif                 
if match(x)(1)=1 then text$(x)(y)=text$(x)(y)+"GRUESOME FIGHTING)":y=y+1:endif
if match(x)(1)>5 and match(x)(1)<11 then text$(x)(y)=text$(x)(y)+match(x)(3)+"-MAN ":endif
if match(x)(1)=4 or match(x)(1)=5 or match(x)(1)=8 then text$(x)(y)=text$(x)(y)+ucase$(ma$(match(x)(1)))+")":y=y+1:endif 
if match(x)(1)=2 or match(x)(1)=3 then text$(x)(y)=text$(x)(y)+"STEEL CAGE)":y=y+1:endif
if match(x)(1)=6 or match(x)(1)=7 then text$(x)(y)=text$(x)(y)+ucase$(ma$(6))+")":y=y+1:endif   
if match(x)(1)=9 or match(x)(1)=10 then text$(x)(y)=text$(x)(y)+ucase$(ma$(9))+")":y=y+1:endif 
y=y+1  

if match(x)(2)=1 then
 for y2=1 to (match(x)(3))
  text$(x)(y)=text$(x)(y)+"*"+wre$(entry(x)(y2))+"*":y=y+2          
  if match(x)(2)=1 and match(x)(11)=2 and y2=1 then text$(x)(y)=text$(x)(y)+"  Vs":y=y+2:endif
 next
else 
 if match(x)(3)<4 then
  z=1:x2=(match(x)(3)+1)
  for y2=1 to x2
   text$(x)(y)=text$(x)(y)+"*"+wre$(entry(x)(z))+"*":y=y+1  
   z=z+1
  next
  y=y+1:text$(x)(y)=text$(x)(y)+"  Vs":y=y+2
  for y2=1 to x2
   text$(x)(y)=text$(x)(y)+"*"+wre$(entry(x)(z))+"*":y=y+1   
   z=z+1
  next  
  y=y+1
 else
  text$(x)(y)=text$(x)(y)+"*"+wre$(entry(x)(1))+"*" :y=y+1
  y=y+1:text$(x)(y)=text$(x)(y)+"  Vs":y=y+2
  z=2:x2=(match(x)(3)-2)
  for y2=1 to x2
   text$(x)(y)=text$(x)(y)+"*"+wre$(entry(x)(z))+"*":y=y+1   
   z=z+1
  next  
  y=y+1
 endif
endif      

x2=y
if match(x)(4)=5 then text$(x)(y)=text$(x)(y)+"(ESCAPE ONLY)":y=y+1:endif     
if match(x)(4)=1 then text$(x)(y)=text$(x)(y)+"(2 COUNT)":y=y+1:endif     
if match(x)(4)=3 then text$(x)(y)=text$(x)(y)+"(PINFALL ONLY - NO SUBM)":y=y+1:endif 
if match(x)(4)=4 then text$(x)(y)=text$(x)(y)+"(SUBMISSION ONLY - NO PIN)":y=y+1:endif   
if match(x)(1)=7 or match(x)(1)=10 then text$(x)(y)=text$(x)(y)+"(OVER ROPE ON)":y=y+1:endif
if match(x)(5)=2 then text$(x)(y)=text$(x)(y)+"(BEST OF 3 MATCHES)":y=y+1:endif
if match(x)(6)=2 then text$(x)(y)=text$(x)(y)+"(NO DISQUALIFICATION)":y=y+1:endif
if match(x)(7)=1 then text$(x)(y)=text$(x)(y)+"(ELIMINATE ALL / SURVIVOR)":y=y+1:endif
if match(x)(8)=2 then text$(x)(y)=text$(x)(y)+"(TORNADO ON)":y=y+1:endif      
if y=x2 then y=y-1:endif 
text$(x)(y)="--------------------------------------------------"

'sides 
for y=1 to 8:side$(x)(y)="*":next
if match(x)(2)=1 then
 for y=1 to (match(x)(11))
  side$(x)(y)=side$(x)(y)+wre$(entry(x)(y))
 next
else   
 if match(x)(3)=1 or match(x)(3)=4 then z2=16:endif 
 if match(x)(3)=2 or match(x)(3)=5 then z2=10:endif
 if match(x)(3)=3 or match(x)(3)=6 then z2=7:endif
 if match(x)(3)<4 then    
  for y=1 to (match(x)(3)+1)
   if y>1 then side$(x)(1)=side$(x)(1)+"/":endif   
   side$(x)(1)=side$(x)(1)+left$(wre$(entry(x)(y)),z2)
  next   
  for y=1 to (match(x)(3)+1)
  if y>1 then side$(x)(2)=side$(x)(2)+"/":endif   
   side$(x)(2)=side$(x)(2)+left$(wre$(entry(x)(1+y+match(x)(3))),z2)
  next  
 else                          
  side$(x)(1)=side$(x)(1)+wre$(entry(x)(1))      
  for y=2 to (match(x)(3)-1)      
   if y>2 then side$(x)(2)=side$(x)(2)+"/":endif   
   side$(x)(2)=side$(x)(2)+left$(wre$(entry(x)(y)),z2) 
  next  
 endif
endif 
for y=1 to 8:side$(x)(y)=side$(x)(y)+"*":next

totalm=totalm+1:x=x+1
goto nextmatch  

showmenu: 
if currm<1 then currm=totalm:endif
if currm>totalm then currm=1:endif
gosub clear                    
if totalm=0 then
 printr "Couldn't generate any matches. Please check your"
 printr "settings and try again."    
 drawtext()
 gosub mouse
 goto editmenu
endif
printr "Match "+currm+" of "+totalm:printr   
for x=1 to 26
 printr mid$(text$(currm)(x),2,49)
next
locate 0,30:print"Match Won By:" 
gsiz=1
bt$="Prev":by=32:bl=0:gosub button 
bt$="Next":by=32:bl=5:gosub button 

bt$="Export-Text":by=32:bl=10:gosub button 
bt$="Autoresults":by=32:bl=22:gosub button
bt$="Finish":by=32:bl=34:gosub button
bt$="Save":by=34:bl=0:gosub button        
bt$="Load":by=34:bl=5:gosub button   
if match(currm)(9)=0 then 
 bt$="Unresolved" 
else          
 if match(currm)(9)=100 then
  bt$="(Match Tied)"
 else
  bt$=side$(currm)(match(currm)(9))
 endif
endif
by=30:bl=14:gosub button
drawtext()
do
 gosub mouse     
 if sel=7 then
  gosub loadgame   
  if mode=1 then goto editmenu else goto showmenu:endif
 endif
 if sel=6 then
  gosub savegame 
  goto showmenu
 endif
  if sel=1 or sel=-100 then currm=currm-1:goto showmenu:endif
  if sel=2 or sel=-200 then currm=currm+1:goto showmenu:endif 
  if sel=4 then
   z3=currm
   for currm=1 to totalm
    if match(currm)(9)=0 then gosub auto:endif
   next
   currm=z3
   goto showmenu
  endif
  if sel=5 then
   gosub clear
   printr"Finish this show and return to Main Menu?":printr
   printr"(Unresolved matches will have results generated"
   printr"for them, and Ratings and Champions will be" 
   printr"updated)"
   gsiz=1
   bt$="Yes":bl=0:by=34:gosub button
   bt$="No":bl=4:by=34:gosub button   
   drawtext()
   do
    gosub mouse  
    if sel=1 then       
     for currm=1 to totalm
      if match(currm)(9)=0 then gosub auto:endif     
      'reassign belts
      if match(currm)(10)>0 and match(currm)(9)<>100 then
       if match(currm)(2)=1 then
        'single
        bh(match(currm)(10))(1)=entry(currm)(match(currm)(9))
       else
        'tag          
        if match(currm)(9)=1 then x=0 else x=(match(currm)(3)+1):endif
        for y=1 to (match(currm)(3)+1)
         bh(match(currm)(10))(y)=entry(currm)(y+x)
        next
       endif                         
      endif   
      
     'loser fired
      if stip(currm)(1)=1 then
       if match(currm)(9)=1 then wd(entry(currm)(2))(1)=2:endif
       if match(currm)(9)=2 then wd(entry(currm)(1))(1)=2:endif
      endif 
      
      'team broken up
      if stip(currm)(1)=2 then 
       currf=0
       if match(currm)(9)=1 then 
        for y=1 to 4:fm(stip(currm)(3))(y)=0:next
       endif
       if match(currm)(9)=2 then 
        for y=1 to 4:fm(stip(currm)(2))(y)=0:next
       endif
      endif
      
      'update rating
      gosub ratingscalc 

     next      

     'ratings min/max
     for x=1 to 64
      if wd(x)(2)<0 then wd(x)(2)=0:endif
      if wd(x)(2)>200 then wd(x)(2)=200:endif 
      if wd(x)(2)>(orig(x)+50) then wd(x)(2)=(orig(x)+50):endif 
      if wd(x)(2)<(orig(x)-50) then wd(x)(2)=(orig(x)-50):endif
     next     

     'sort new rankings
     gosub checksort 
     gosub checkspecsort

     'update history       
     for x=1 to 23:hist$(x)=hist$(x+1):lines(x)=lines(x+1):next
     z=1            
     for x=1 to 300:hist$(24)(x)="*":next    
     hist$(24)(z)="*--------------------------------------------------":z=z+2  
     hist$(24)(z)="*SHOW "+(realshow+1)+" "
     if house=1 then 
      hist$(24)(z)=hist$(24)(z)+"(regular show)"
     else
      if major=1 then hist$(24)(z)=hist$(24)(z)+"(major ppv)" else hist$(24)(z)=hist$(24)(z)+"(ppv)":endif
     endif
     z=z+2
     hist$(24)(z)="*--------------------------------------------------":z=z+1
     for currm=1 to totalm
      y=1   
      addline:           
      if text$(currm)(y)<>"--------------------------------------------------" then 
       hist$(24)(z)=text$(currm)(y):y=y+1:z=z+1:goto addline      
      else   
       z=z+1
       if match(currm)(9)=100 then
        hist$(24)(z)="*Result: match tied"
       else       
        i$=left$(side$(currm)(match(currm)(9)),(len(side$(currm)(match(currm)(9)))-1)) 
        i$=right$(i$,(len(i$)-1))
        hist$(24)(z)="*Result: won by "+i$
       endif           
       z=z+1
       if x<>totalm then hist$(24)(z)=text$(currm)(y):z=z+1:endif 
      endif
     next     
     lines(24)=z+8
     if tothist<24 then tothist=tothist+1:endif 
     realshow=realshow+1
     
     f=openfilewrite("Archive.txt") 
     writeline(f,"Recent shows")
     writeline(f,"")
     y=(25-tothist)
     for z=y to 24
      for x=1 to lines(z)        
       if z<>24 or x<(lines(z)-9) then 
        writeline(f,right$(hist$(z)(x),(len(hist$(z)(x))-1))) 
       endif
      next
     next 
     closefile(f)

     mode=1    
     gosub setuptitlefactions
     goto editmenu
    endif
    if sel=2 then goto showmenu:endif
   loop
  endif 

  if sel=3 then  
   gosub clear
   printr"Input the name of this show's text file:-":printr
   printr"(Or enter a blank field to cancel export)" 
   printr
   drawtext()   
   color(0,0,128)
   input ">",i$
   color(0,0,0)  
   if i$<>"" then 
    chk$=findfirstfile(i$+".txt") 
    if chk$<>""then
     gosub clear
     printr"Filename already exists. Overwrite?"
     gsiz=1
     bt$="Yes":bl=0:by=34:gosub button
     bt$="No":bl=4:by=34:gosub button  
     drawtext()
     do
      gosub mouse  
      if sel=1 then goto ovrtext:endif
      if sel=2 then goto showmenu:endif
     loop
    endif   
    ovrtext:
    f=openfilewrite(i$+".txt") 
    writeline(f,prom$+" presents:"):writeline(f,"")
    writeline(f,"'"+ucase$(i$)+"'"):writeline(f,"") 
    writeline(f,"--------------------------------------------------")
    for x=1 to totalm
     y=1   
     export:           
     if text$(x)(y)<>"--------------------------------------------------" then 
      writeline(f,mid$(text$(x)(y),2,49)):y=y+1:goto export      
     else                 
      if x<>totalm then writeline (f,text$(x)(y)):endif 
     endif
    next
    closefile(f)
   cls:printr"File Exported":drawtext():sleep(1000)
   endif    
   goto showmenu
  endif  
 if sel=8 then
  gosub clear   
  printr"Enter a Winner for this Match:-":printr
  gsiz=1:bl=0   
  bt$="(Cancel)":by=2:gosub button   
  bt$="(Auto-Generate)":by=4:gosub button   
  bt$="(Match Tied)":by=6:gosub button
  if match(currm)(2)=1 then
   for x=1 to (match(currm)(3))
    bt$=side$(currm)(x):by=(x*2)+6:gosub button
   next
  else
   bt$=side$(currm)(1):by=8:gosub button
   bt$=side$(currm)(2):by=10:gosub button
  endif
  drawtext()
  do
   gosub mouse                  
   if sel=2 then gosub auto:goto showmenu:endif
   if sel=1 then goto showmenu:endif
   if sel=3 then match(currm)(9)=100:goto showmenu:endif
   if sel>3 and sel<11 then   
    z=sel-3
    if match(currm)(2)=1 and z<=match(currm)(11) then match(currm)(9)=z:goto showmenu:endif
    if match(currm)(2)=2 and z<3 then match(currm)(9)=z:goto showmenu:endif
   endif
  loop
  goto showmenu
 endif
loop

factions:
gosub clear
printr"*Edit Factions*":printr   
printr"Viewing Faction ":printr
printr"Faction "+currf+" of 16":printr   
for x=1 to 4:printr"Member #"+x+": ":printr:next
gsiz=1:bl=11
for x=1 to 4
 by=(x*2)+4
 if fm(currf)(x)=0 then bt$="VACANT" else bt$=wre$(fm(currf)(x)):endif
 gosub button
next   
bl=0   
gsiz=1:by=28:bt$="Clear Faction":gosub button  
gsiz=1:by=30:bt$="Previous Faction":gosub button  
gsiz=1:by=32:bt$="Next Faction":gosub button
gsiz=1:by=34:bt$="Back to Previous Menu":gosub button  
gsiz=1:by=2:bl=16:bt$=fa$(currf):gosub button
drawtext()
do
 gosub mouse  
 if sel=5 then
  for y=1 to 4:fm(currf)(y)=0:next
  fa$(currf)="Unnamed"
  goto factions
 endif
 if sel=8 then goto editmenu:endif
 if sel=7 or sel=-200 then currf=currf+1
  if currf=17 then currf=1:endif
  goto factions
 endif
 if sel=6 or sel=-100 then currf=currf-1
  if currf=0 then currf=16:endif
  goto factions
 endif    
 if sel>0 and sel<5 then
  pscreen=2:y2=sel
  gosub pickwres  
  goto factions
 endif    
 if sel=9 then
   cls
   printr "Enter a new name for "+ucase$(fa$(currf)):printr
   printr"(Or enter a blank field to return without change)":printr
   drawtext()
   color(0,0,128)
   input ">",i$
   color(0,0,0)
   if i$<>"" then fa$(currf)=left$(i$,16):endif
   goto factions
 endif
loop

roster:
gosub clear    
sprsettexture(f3)
print"*Edit Roster* "
if page=1 then 
 printr"(Page 1/2)" 
 y=1:z=24
else 
 printr "(Page 2/2)"
 y=25:z=48
endif
printr
printr"Wrestler          Use Rat Class Side Sin/TT Prefs"       
gsiz=7
for x=y to z
 bt$=wre$(x):by=(x-y)+4:bl=0:gosub button
 if wd(x)(1)=1 then bt$="Yes" else bt$="---":endif
 bl=18:gosub button         
 bt$=wd(x)(2):bl=22:gosub button 
 if wd(x)(3)=1 then bt$="Heavy":endif 
 if wd(x)(3)=2 then bt$="Cruis":endif 
 if wd(x)(3)=3 then bt$="Woman":endif
 bl=26:gosub button     
 if wd(x)(5)=1 then bt$="Face":endif 
 if wd(x)(5)=2 then bt$="Heel":endif 
 if wd(x)(5)=3 then bt$="----":endif
 bl=32:gosub button  
 if wd(x)(4)=1 then bt$="Single":endif
 if wd(x)(4)=2 then bt$="Either":endif    
 if wd(x)(4)=3 then bt$="Tag Tm":endif   
 bl=37:gosub button 
 if wd(x)(6)=1 then bt$="Normal":endif    
 if wd(x)(6)=2 then bt$="H-Core":endif
 if wd(x)(6)=3 then bt$="PureWr":endif
 if wd(x)(6)=4 then bt$="MMArts":endif
 bl=44:gosub button 
next 
gsiz=1
if page=1 then bt$="Switch to Page 2" else bt$="Switch to Page 1":endif 
bl=0:by=32:gosub button
gsiz=1
bt$="Back To Previous Menu":by=34:bl=0:gosub button 
gsiz=1
bt$="Re-Sort Roster":by=30:bl=0:gosub button
drawtext()    
do
 gosub mouse      
 if sel>0 and sel<25 then
  if page=2 then sel=sel+24:endif
   if sel2=1 then        
    gosub clear   
    sprsettexture(f2)
    printr "Enter a new name for "+ucase$(wre$(sel)):printr
    printr"(Or enter a blank field to return without change)":printr
    drawtext() 
    color(0,0,128)
    input ">",i$
    color(0,0,0)
    if i$<>"" then wre$(sel)=left$(i$,16):endif
    goto roster
   endif    
   if sel2=3 then
    gosub clear   
    sprsettexture(f2)
    printr "Enter a new rating for "+ucase$(wre$(sel)):printr
    printr "(This affects how high up the card this wrestler ":printr "will appear)":printr    
    printr"Guidelines:-":printr  
    printr"Average: 100":printr 
    printr "Main Event: 125-175":printr  
    printr "Mid Card: 75-125":printr
    printr "Under Card: 25-75":printr 
    printr "Icon: 200":printr
    printr "Women 0-50":printr
    drawtext():color(0,0,128)
    input ">",x
    if x<0 then x=0:endif
    if x>200 then x=200:endif
    wd(sel)(2)=x
    orig(sel)=x
    color(0,0,0):goto roster
   endif
   if sel2=2 then 
    wd(sel)(1)=(3-wd(sel)(1)):goto roster
   endif 
   if sel2=4 then   
    if wd(sel)(3)=3 then wd(sel)(3)=1:goto roster:endif
    wd(sel)(3)=wd(sel)(3)+1:goto roster
   endif  
   if sel2=5 then   
    if wd(sel)(5)=3 then wd(sel)(5)=1:goto roster:endif
    wd(sel)(5)=wd(sel)(5)+1:goto roster
   endif 
   if sel2=6 then 
    if wd(sel)(4)=3 then wd(sel)(4)=1:goto roster:endif
    wd(sel)(4)=wd(sel)(4)+1:goto roster
   endif 
   if sel2=7 then 
    wd(sel)(6)=wd(sel)(6)+1
    if wd(sel)(6)>4 then wd(sel)(6)=1:endif 
    goto roster 
   endif    
 endif     

 if sel=25 then page=(3-page):goto roster:endif    
 if sel=-200 and page=1 then page=2:goto roster:endif
 if sel=-100 and page=2 then page=1:goto roster:endif
 if sel=26 then gosub checksort:sprsettexture(f2):goto editmenu:endif  
 if sel=27 then gosub checksort:goto roster:endif  
loop  

checksort:
for y=1 to 47
 for x=1 to 47
  if wd(x)(1)=2 and wd(x+1)(1)=1 then gosub resort:endif
 next
next
for y=1 to 47
 for x=1 to 47 
  if wd(x)(2)<wd(x+1)(2) and wd(x)(1)>=wd(x+1)(1) then gosub resort:endif
 next
next     
return   

resort:     
for x2=1 to 24
 for y2=1 to 4
  if fm(x2)(y2)=x then
   fm(x2)(y2)=x+1     
  else
   if fm(x2)(y2)=x+1 then
    fm(x2)(y2)=x
   endif
  endif
 next
next       
for x2=1 to 8
 for y2=1 to 4
  if bh(x2)(y2)=x then 
   bh(x2)(y2)=x+1
  else
   if bh(x2)(y2)=x+1 then
    bh(x2)(y2)=x
   endif
  endif
 next
next  
i$=wre$(x)
for z=1 to 6:wd(0)(z)=wd(x)(z):next
wre$(x)=wre$(x+1)
wre$(x+1)=i$       
for z=1 to 6
 wd(x)(z)=wd(x+1)(z)
 wd(x+1)(z)=wd(0)(z)
next    
orig(0)=orig(x)
orig(x)=orig(x+1)
orig(x+1)=orig(0) 
return

belts:
gosub clear     
printr"*Edit Championships*":printr
printr"Titles     Use * Cls #'s Holders             Rules"
gsiz=7
for x=1 to 8
 bt$=belt$(x):by=(x*2)+2:bl=0:gosub button    
 if bd(x)(1)=1 then bt$="Yes" else bt$="---":endif
 bl=11:gosub button
 if bd(x)(2)=1 then bt$="A":endif 
 if bd(x)(2)=2 then bt$="B":endif
 if bd(x)(2)=3 then bt$="C":endif
 bl=15:gosub button 
 if bd(x)(3)=1 then bt$="Opn":endif 
 if bd(x)(3)=2 then bt$="Cru":endif
 if bd(x)(3)=3 then bt$="Wom":endif
 if bd(x)(3)=4 then bt$="Hvy":endif
 bl=17:gosub button  
 bt$=bd(x)(4)+"v"+bd(x)(4)
 bl=21:gosub button 
 if bh(x)(1)=0 then 
  bt$="VACANT"
 else
  if bd(x)(4)=1 then bt$=wre$(bh(x)(1)):endif
  if bd(x)(4)=2 then bt$=left$(wre$(bh(x)(1)),9)+"/"+left$(wre$(bh(x)(2)),9):endif
  if bd(x)(4)=3 then
   bt$=left$(wre$(bh(x)(1)),5)+"/"+left$(wre$(bh(x)(2)),5)+"/"+left$(wre$(bh(x)(3)),5)
  endif
  if bd(x)(4)=4 then
   bt$=left$(wre$(bh(x)(1)),4)+"/"+left$(wre$(bh(x)(2)),4)+"/"+left$(wre$(bh(x)(3)),4)+"/"+left$(wre$(bh(x)(4)),4)
  endif
 endif
 bl=25:gosub button
 bt$="Chnge":bl=45:gosub button
next  
gsiz=1
bt$="Back To Previous Menu":by=34:bl=0:gosub button

drawtext()  
do
 gosub mouse    
 if sel>0 and sel<9 then
  if sel2=1 then
   gosub clear
   printr "Enter a new name for "+ucase$(belt$(sel))+" Championship":printr
   printr"(Or enter a blank field to return without change)":printr
   drawtext()
   color(0,0,128)
   input ">",i$
   color(0,20,0)
   if i$<>"" then belt$(sel)=left$(i$,10):endif
   goto belts
  endif 
  if sel2=2 then bd(sel)(1)=3-(bd(sel)(1)) 
   goto belts
  endif 
  if sel2=3 then
   if bd(sel)(2)=3 then bd(sel)(2)=1:goto belts:endif
   bd(sel)(2)=bd(sel)(2)+1:goto belts
  endif
  if sel2=4 then             
   if bd(sel)(3)=4 then bd(sel)(3)=1:goto belts:endif
   bd(sel)(3)=bd(sel)(3)+1:goto belts
  endif      
  if sel2=5 then              
   if bd(sel)(4)=4 then bd(sel)(4)=1:gosub vacate:goto belts:endif
   bd(sel)(4)=bd(sel)(4)+1:gosub vacate:goto belts
  endif  
  if sel2=7 then 
   pscreen=2    
   currb=sel    
   for x=0 to 5:tmrule(x)(1)=x:tmrule(x)(2)=bmrule(sel)(x):next               
   if bd(sel)(4)=1 then    
    for x=6 to 18:tmrule(x)(1)=x:tmrule(x)(2)=bmrule(sel)(x):next 
    totaltm=18 
   else                 
    for x=6 to 17:tmrule(x)(1)=x+5:tmrule(x)(2)=bmrule(sel)(x+5):next 
    totaltm=17
   endif
   rules:    
   gosub clear
   printr "Edit "+ucase$(belt$(currb))+" Championship Rules Employed:-" 
   printr 
   for x=0 to totaltm
    printr"     : "+ma$(tmrule(x)(1))
   next
   gsiz=1:bl=0    
   for x=0 to totaltm    
    if tmrule(x)(2)=1 then bt$="Allow" else bt$="-----":endif 
    by=x+2:gosub button 
   next
   gsiz=1
   bt$="Back To Previous Menu":by=34:bl=0:gosub button
  drawtext()
  do
   gosub mouse
   if sel>0 and sel<(totaltm+2) then              
    sel=sel-1
    tmrule(sel)(2)=(3-tmrule(sel)(2)):goto rules  
   endif  
   if sel=(totaltm+2) then    
    for x=0 to totaltm
     bmrule(currb)(tmrule(x)(1))=tmrule(x)(2)
    next
    goto belts
   endif  
  loop  
  endif  
  if sel2=6 then
   currb=sel:pscreen=1
   for y=1 to 4:bh(currb)(y)=0:next
   gosub pickwres
   gosub setuptitlefactions:goto belts
  endif 
 endif   
 if sel=9 then gosub setuptitlefactions:goto editmenu:endif
loop  

pickwres: 
if pscreen=1 then 
 x2=bd(currb)(4)  
 for x=1 to 4:bh(currb)(x)=0:next
endif
if pscreen=2 then 
 x2=1
endif
for x=1 to x2
 gosub clear
 if pscreen=1 then
  print"Pick "+ucase$(belt$(currb))+" Championship Holder #"+x
  if x2>1 then print" #"+x:endif  
  printr:printr 
 endif
 if pscreen=2 then  
  printr"Pick "+ucase$(fa$(currf))+" Member #"+y2
  printr
 endif   
 gsiz=2:bl=0     
 if pscreen=1 then z3=47 else z3=63:endif      
 for y=1 to z3 step 2
  bt$=wre$(y):by=((y/2)+2):bl=0:gosub button
  bt$=wre$(y+1):by=((y/2)+2):bl=24:gosub button
 next
 gsiz=1:by=0   
 if pscreen=1 then bl=len(belt$(currb))+29 else bl=len(fa$(currf))+16:endif
 bt$="(VACATE)":gosub button
 drawtext() 
 if pscreen=1 then z3=25 else z3=33:endif 
 do
  gosub mouse  
  if sel>0 and sel<z3 then 
   sel=sel*2
   if sel2=1 then sel=sel-1:endif
   if pscreen=1 then
    for z2=1 to 4
     if bh(currb)(z2)=sel then x=x-1:goto choosenext:endif  
    next 
    bh(currb)(x)=sel
   endif
   if pscreen=2 then
    for z2=1 to 4
     if fm(currf)(z2)=sel and z2<>y2 then x=x-1:goto choosenext:endif
    next
    fm(currf)(y2)=sel
   endif      
   goto choosenext 
  endif 
  if sel=z3 then
   if pscreen=1 then
    for z2=1 to 4: bh(currb)(z2)=0:next
   endif
   if pscreen=2 then
    fm(currf)(y2)=0
   endif  
   return
  endif
 loop
choosenext:
next  
return    

promrules: 
if xrule(1)<1 then xrule(1)=1:endif
if xrule(1)>5 then xrule(1)=5:endif 
for x=2 to 5
 if xrule(x)>3 then xrule(x)=1:endif
next 
for x=6 to 9
 if xrule(x)<1 then xrule(x)=1:endif
 if xrule(x)>5 then xrule(x)=5:endif
next  
for x=0 to 14
 if mrule(x)>3 then mrule(x)=1:endif
next   

gosub clear
printr"*Set Matchtypes for next show*"
printr  
if xrule(1)=1 then printr "   : Use Singles matches only":endif    
if xrule(1)=2 then printr "   : Use mainly Singles matches":endif  
if xrule(1)=3 then printr "   : Use both Single and Team matches":endif
if xrule(1)=4 then printr "   : Use mainly Team matches":endif
if xrule(1)=5 then printr "   : Use Team matches only":endif 
gsiz=1
bl=0:by=2:bt$="<":gosub button 
bl=2:by=2:bt$=">":gosub button  

locate 0,4
printr "   : 4-Man Team matches"
printr "   : 6-Man Team matches"
printr "   : 8-Man Team matches"
printr "   : Handicap Team matches"
for x=2 to 5
 if xrule(x)=1 then bt$="Oft":endif 
 if xrule(x)=2 then bt$="Rar":endif 
 if xrule(x)=3 then bt$="---":endif           
 bl=0:by=x+2:gosub button
next            

locate 0,9
for x=0 to 14 
 printr"   : "+ma$(x)
next
bl=0    
for x=0 to 14       
 if mrule(x)=1 then bt$="Oft":endif
 if mrule(x)=2 then bt$="Rar":endif
 if mrule(x)=3 then bt$="---":endif  
 by=x+9:gosub button 
next     

locate 0,25      
if xrule(6)=1 then printr"   : Only best of 1 Fall":endif
if xrule(6)=2 then printr"   : Usually best of 1 Fall":endif
if xrule(6)=3 then printr"   : Best of either 1 or 3 Falls":endif 
if xrule(6)=4 then printr"   : Usually best of 3 Falls":endif
if xrule(6)=5 then printr"   : Only best of 3 Falls":endif
bl=0:by=25:bt$="<":gosub button 
bl=2:by=25:bt$=">":gosub button  

locate 0,26      
if xrule(7)=1 then printr"   : DQ count always On":endif
if xrule(7)=2 then printr"   : DQ count usually On":endif
if xrule(7)=3 then printr"   : DQ count either On or Off":endif
if xrule(7)=4 then printr"   : DQ count usually Off":endif
if xrule(7)=5 then printr"   : DQ count always Off":endif   
bl=0:by=26:bt$="<":gosub button 
bl=2:by=26:bt$=">":gosub button 

locate 0,27        
if xrule(8)=1 then printr"   : Team Matches always 1st Fall":endif
if xrule(8)=2 then printr"   : Team Matches usually 1st Fall":endif
if xrule(8)=3 then printr"   : Team Matches either 1st Fall or Elim all":endif 
if xrule(8)=4 then printr"   : Team Matches usually Elim all":endif
if xrule(8)=5 then printr"   : Team Matches always Elim all":endif 
bl=0:by=27:bt$="<":gosub button 
bl=2:by=27:bt$=">":gosub button 

locate 0,28 
if xrule(9)=1 then printr"   : Team Matches always Tag":endif   
if xrule(9)=2 then printr"   : Team Matches usually Tag":endif   
if xrule(9)=3 then printr"   : Team Matches either Tag or Tornado":endif 
if xrule(9)=4 then printr"   : Team Matches usually Tornado":endif   
if xrule(9)=5 then printr"   : Team Matches always Tornado":endif 
bl=0:by=28:bt$="<":gosub button 
bl=2:by=28:bt$=">":gosub button    

bt$="Back To Previous Menu":by=34:bl=0:gosub button 
bt$="Save MatchType Settings":by=30:bl=0:gosub button    
bt$="Load MatchType Settings":by=32:bl=0:gosub button

drawtext()
do
gosub mouse       
 if sel>0 and sel<30 then
  if sel=1 then xrule(1)=xrule(1)-1:endif
  if sel=2 then xrule(1)=xrule(1)+1:endif
  if sel>2 and sel<7 then
   xrule(sel-1)=xrule(sel-1)+1
  endif 
  if sel>6 and sel<22 then mrule(sel-7)=mrule(sel-7)+1:endif 
  if sel=22 then xrule(6)=xrule(6)-1:endif
  if sel=23 then xrule(6)=xrule(6)+1:endif  
  if sel=24 then xrule(7)=xrule(7)-1:endif
  if sel=25 then xrule(7)=xrule(7)+1:endif 
  if sel=26 then xrule(8)=xrule(8)-1:endif
  if sel=27 then xrule(8)=xrule(8)+1:endif 
  if sel=28 then xrule(9)=xrule(9)-1:endif
  if sel=29 then xrule(9)=xrule(9)+1:endif 
  goto promrules
 endif
 if sel=30 then return:endif   
 if sel=31 then gosub saverules:goto promrules:endif
 if sel=32 then gosub loadrules:goto promrules:endif
loop 
 
auto:
 if match(currm)(2)=1 then
  if match(currm)(11)=2 then
   '1V1                
   gosub findsingleside
   x=rnd()%100+1
   if x<=table(z)(3) then match(currm)(9)=1 else match(currm)(9)=2:endif
  else
   'BRoyal
   z2=0:y=0
   for x=1 to (match(currm)(11))
    side(x)=wd(entry(currm)(x))(2):side(x)=side(x)+rnd()%100+1
    if side(x)>z2 then z2=side(x):y=x:endif
   next
   match(currm)(9)=y
  endif
 else
 'team         
  gosub findteamside                                
  x=rnd()%100+1
  if x<=table(z)(3) then match(currm)(9)=1 else match(currm)(9)=2:endif
 endif
return    

findsingleside:
x2=wd(entry(currm)(1))(2)
y2=wd(entry(currm)(2))(2)
y=x2-y2    
for z=1 to 21
 if y>=table(z)(1) and y<=table(z)(2) then return:endif
next
return  

findteamside:
z=0
z2=0 
if match(currm)(3)<4 then 
 y=(match(currm)(3)+1)
 x2=y+1
 y2=match(currm)(11)
else
 y=1
 x2=2
 y2=match(currm)(11)
endif
for x=1 to y:z=z+wd(entry(currm)(x))(2):next
for x=x2 to y2:z2=z2+wd(entry(currm)(x))(2):next 

x#=z2  
if match(currm)(3)<4 then x#=x#/(match(currm)(3)+1):endif 
if match(currm)(3)>3 then x#=x#/(match(currm)(3)-2):endif

if match(currm)(3)=4 then x#=x#*3:endif
if match(currm)(3)=5 then x#=x#*6:endif
if match(currm)(3)=6 then x#=x#*10:endif  

gosub fraction
z2=x#     

if match(currm)(3)<4 then x#=z::x#=x#/(match(currm)(3)+1):gosub fraction:z=x#:endif

y=z-z2    
for z=1 to 21
 if y>=table(z)(1) and y<=table(z)(2) then return:endif
next
return

ratingscalc: 
            
if match(currm)(2)=1 then
 if match(currm)(11)=2 then
  '1V1                
  gosub findsingleside       
  if match(currm)(9)=1 then x#=table(z)(4):endif
  if match(currm)(9)=2 then x#=table(z)(5):endif
  if match(currm)(9)=100 then x#=table(z)(6):endif  
  wd(entry(currm)(1))(2)=wd(entry(currm)(1))(2)+x#
  wd(entry(currm)(2))(2)=wd(entry(currm)(2))(2)-x# 
 else
 'BRoyal
  if match(currm)(9)=100 then
   'tie    
   for x=1 to (match(currm)(3))
    x#=0
    for z=1 to (match(currm)(3))
     if x<>z then x#=x#+wd(entry(currm)(z))(2):endif
     next     
     x#=x#/(match(currm)(3)-1):gosub fraction
     z=wd(entry(currm)(x))(2)
     z=z-x# 
     for y=1 to 21
      if z>=table(y)(1) and z<=table(y)(2) then goto brtie:endif
     next        
     brtie:              
     side(x)=wd(entry(currm)(x))(2)+table(y)(6)
    next 
    for x=1 to (match(currm)(3))
     wd(entry(currm)(x))(2)=side(x)
    next
   else
    'BR winner
    x=match(currm)(9):y=entry(currm)(x)    
    x#=1
    for z=1 to (match(currm)(3))
     if entry(currm)(z)<>y then
      side(x#)=entry(currm)(z)
      x#=x#+1
     endif
    next
    x#=0
    for z=1 to (match(currm)(3)-1)
     x#=x#+wd(side(z))(2)
    next
    x#=x#/(match(currm)(3)-1):gosub fraction
    x=wd(y)(2)-x#        
    for z=1 to 21
     if x>=table(z)(1) and x<=table(z)(2) then goto brrat:endif
    next
    brrat:
    x#=table(z)(4)
    if match(currm)(3)=3 then x#=x#*1.33:endif     
    if match(currm)(3)=4 then x#=x#*1.66:endif
    if match(currm)(3)=5 then x#=x#*2:endif
    if match(currm)(3)=6 then x#=x#*2.33:endif  
    if match(currm)(3)=7 then x#=x#*2.66:endif  
    if match(currm)(3)=8 then x#=x#*3:endif      
    gosub fraction
    wd(y)(2)=wd(y)(2)+x#
    x#=x#/(match(currm)(3)-1):gosub fraction
    for z=1 to (match(currm)(3)-1)
     wd(side(z))(2)=wd(side(z))(2)-x#
    next
   endif
  endif
else
  if match(currm)(3)<4 then
   'tag team           
   z=0
   z2=0 
   for x=1 to (match(currm)(3)+1):z=z+wd(entry(currm)(x))(2):next
   for x=(match(currm)(3)+2) to (match(currm)(11)):z2=z2+wd(entry(currm)(x))(2):next  
   x#=z:x#=x#/(match(currm)(3)+1):gosub fraction:z#=x#
   x#=z2:x#=x#/(match(currm)(3)+1):gosub fraction 
   y=z#-x#
   for z=1 to 21
    if y>=table(z)(1) and y<=table(z)(2) then goto tagrats:endif
   next
   tagrats:
   if match(currm)(9)=1 then x#=table(z)(4):endif
   if match(currm)(9)=2 then x#=table(z)(5):endif
   if match(currm)(9)=100 then x#=table(z)(6):endif
   for x=1 to (match(currm)(3)+1)
    wd(entry(currm)(x))(2)=wd(entry(currm)(x))(2)+x#
   next
   for x=(match(currm)(3)+2) to (match(currm)(11))
    wd(entry(currm)(x))(2)=wd(entry(currm)(x))(2)-x#
   next
  else
  'handicap   
   z=wd(entry(currm)(1))(2)
   z2=0
   for x=2 to (match(currm)(11)):z2=z2+wd(entry(currm)(x))(2):next  
   x#=z2:x#=x#/(match(currm)(3)-2):gosub fraction 
   y=z-x#
   for z=1 to 21
    if y>=table(z)(1) and y<=table(z)(2) then goto handirats:endif
   next
   handirats:
   if match(currm)(9)=1 or match(currm)(9)=100 then   
    x#=table(z)(4) 
    if match(currm)(3)=4 then x#=x#*3:endif
    if match(currm)(3)=5 then x#=x#*6:endif
    if match(currm)(3)=6 then x#=x#*10:endif 
    if match(currm)(9)=100 then x#=x#/2:endif
    wd(entry(currm)(1))(2)=wd(entry(currm)(1))(2)+x#
   endif
   if match(currm)(9)=2 then 
    x#=table(z)(5)
    if match(currm)(3)=4 then x#=x#/100:x#=x#*75:endif   
    if match(currm)(3)=5 then x#=x#/100:x#=x#*66.5:endif
    if match(currm)(3)=6 then x#=x#/100:x#=x#*51.25:endif  
    gosub fraction
    wd(entry(currm)(1))(2)=wd(entry(currm)(1))(2)+x#
   endif               
   x#=x#/(match(currm)(3)-2):gosub fraction
   for x=2 to (match(currm)(11))
    wd(entry(currm)(x))(2)=wd(entry(currm)(x))(2)-x#
   next
  endif
endif
return  

vacate:
 for x=1 to 4:bh(sel)(x)=0:next
 return

clear:   
 'clear buttons      
 cls
 bn=0 
 cgrp=1  
 csiz=1
 return    

button:    
 'define clickable stuff
 bn=bn+1  
 bi(bn)(1)=by:bi(bn)(2)=bl:bi(bn)(3)=bl+len(bt$):bi(bn)(4)=cgrp:bi(bn)(5)=csiz   
 bu$(bn)=bt$
 if csiz=gsiz then
  cgrp=cgrp+1:csiz=1
 else
  csiz=csiz+1
 endif        
 color(0,0,128)
 locate bl,by:print bt$    
 color(0,0,0)
 return
 
mouse:      
 highlight=0
 'wait for click
 while mouse_button(mouse_lbutton)
  gosub checkbutt
 wend                     
 while not mouse_button(mouse_lbutton)
  mw=mouse_wheel()  
  if mouse_wheel()<mw then sel=-100:return:endif
  if mouse_wheel()>mw then sel=-200:return:endif
  gosub checkbutt
 wend 
 'find selected
 mx=Mouse_X()*TextCols()
 my=Mouse_Y()*TextRows() 
 sel=0
 for ml=1 to bn
  if my=bi(ml)(1) and mx>=bi(ml)(2) and mx<bi(ml)(3) then sel=bi(ml)(4):sel2=bi(ml)(5):endif
 next
 return  
 
checkbutt:           
 mx=Mouse_X()*TextCols()
 my=Mouse_Y()*TextRows()  
 if highlight=0 then 
  for ml=1 to bn
   if my=bi(ml)(1) and mx>=bi(ml)(2) and mx<bi(ml)(3) then 
    color(255,0,0)
    locate bi(ml)(2),bi(ml)(1):print bu$(ml):drawtext()
    highlight=ml  
    color(0,0,0)
    return
   endif
  next
 else
  if my<>bi(highlight)(1) or mx<bi(highlight)(2) or mx>=bi(highlight)(3) then 
   color(0,0,128)
   locate bi(highlight)(2),bi(highlight)(1):print bu$(highlight):drawtext()
   highlight=0
   color(0,0,0)
   return
  endif
 endif
return  

fraction:        
'rounding fp's
y#=x#
x#=int(x#)
if y#>x# then
 if rnd()%2=0 then x#=x#+1:endif
endif
return  

setuptitlefactions: 
for x=1 to 8           
 for y=1 to 4:fm(16+x)(y)=0:next
 if bd(x)(4)>1 then
  for y=1 to (bd(x)(4))
   fm(16+x)(y)=bh(x)(y)
  next
 endif
next
return

getx3:  
'get 0-3 number, 0 + 3 are rarer
if house=1 then 
 x3=(rnd()%64)
 if x3=63 then x3=3:return:endif
 if x3>0 and x3<63 then x3=rnd()%2+1:return:endif
 return
endif
if house=0 and major=0 then 
 x3=(rnd()%16)
 if x3=15 then x3=3:return:endif
 if x3>0 and x3<15 then x3=rnd()%2+1:return:endif
 return
endif
'major
x3=rnd()%4:return 

redomatch:
for y=1 to match(x)(11)
 if entry(x)(y)>0 then 
  chosen(entry(x)(y))=0
  entry(x)(y)=0
  left=left+1
 endif
next 
star=0 
goto trymatch      

special:        
gosub clear    
sprsettexture(f4)
printr"*Edit Special Roster*"
printr
printr"Wrestler          Use Rat Class Side Sin/TT Prefs"       
gsiz=7
for x=49 to 64
 bt$=wre$(x):by=(x-45):bl=0:gosub button
 if wd(x)(1)=1 then bt$="Yes" else bt$="---":endif
 bl=18:gosub button         
 bt$=wd(x)(2):bl=22:gosub button 
 if wd(x)(3)=1 then bt$="Heavy":endif 
 if wd(x)(3)=2 then bt$="Cruis":endif 
 if wd(x)(3)=3 then bt$="Woman":endif
 bl=26:gosub button     
 if wd(x)(5)=1 then bt$="Face":endif 
 if wd(x)(5)=2 then bt$="Heel":endif 
 if wd(x)(5)=3 then bt$="----":endif
 bl=32:gosub button  
 if wd(x)(4)=1 then bt$="Single":endif
 if wd(x)(4)=2 then bt$="Either":endif    
 if wd(x)(4)=3 then bt$="Tag Tm":endif   
 bl=37:gosub button 
 if wd(x)(6)=1 then bt$="Normal":endif    
 if wd(x)(6)=2 then bt$="H-Core":endif
 if wd(x)(6)=3 then bt$="PureWr":endif
 if wd(x)(6)=4 then bt$="MMArts":endif
 bl=44:gosub button 
next 
gsiz=1
bt$="Back To Previous Menu":by=34:bl=0:gosub button   
bt$="Re-Sort Special Roster":by=32:bl=0:gosub button 

drawtext()    
do
 gosub mouse      
 if sel>0 and sel<17 then   
   sel=sel+48
   if sel2=1 then        
    gosub clear   
    sprsettexture(f2)
    printr "Enter a new name for "+ucase$(wre$(sel)):printr
    printr"(Or enter a blank field to return without change)":printr
    drawtext() 
    color(0,0,128)
    input ">",i$
    color(0,0,0)
    if i$<>"" then wre$(sel)=left$(i$,16):endif
    goto special
   endif    
   if sel2=3 then
    gosub clear   
    sprsettexture(f2)
    printr "Enter a new rating for "+ucase$(wre$(sel)):printr
    printr "(This affects how high up the card this wrestler ":printr "will appear)":printr    
    printr"Guidelines:-":printr    
    printr "Icon: 200":printr 
    printr "Main Eventer: 130-175":printr
    printr "Mid Carder: 75-130":printr
    printr "Under Carder: 25-75":printr 
    printr "Women 0 to 50":printr
    drawtext():color(0,0,128)
    input ">",x
    if x<0 then x=0:endif
    if x>200 then x=200:endif
    wd(sel)(2)=x
    orig(sel)=x
    color(0,0,0):goto special
   endif
   if sel2=2 then 
    wd(sel)(1)=(3-wd(sel)(1)):goto special
   endif 
   if sel2=4 then   
    if wd(sel)(3)=3 then wd(sel)(3)=1:goto special:endif
    wd(sel)(3)=wd(sel)(3)+1:goto special
   endif  
   if sel2=5 then   
    if wd(sel)(5)=3 then wd(sel)(5)=1:goto special:endif
    wd(sel)(5)=wd(sel)(5)+1:goto special
   endif 
   if sel2=6 then 
    if wd(sel)(4)=3 then wd(sel)(4)=1:goto special:endif
    wd(sel)(4)=wd(sel)(4)+1:goto special
   endif 
   if sel2=7 then 
    wd(sel)(6)=wd(sel)(6)+1
    if wd(sel)(6)>4 then wd(sel)(6)=1:endif 
    goto special 
   endif    
 endif     

 if sel=17 then gosub checkspecsort:sprsettexture(f2):goto editmenu:endif   
 if sel=18 then gosub checkspecsort:goto special:endif
loop 

checkspecsort:
for y=49 to 63
 for x=49 to 63
  if wd(x)(1)=2 and wd(x+1)(1)=1 then gosub specresort:endif
 next
next
for y=49 to 63
 for x=49 to 63 
  if wd(x)(2)<wd(x+1)(2) and wd(x)(1)>=wd(x+1)(1) then gosub specresort:endif
 next
next     
return

specresort: 
for x2=1 to 24
 for y2=1 to 4
  if fm(x2)(y2)=x then
   fm(x2)(y2)=x+1     
  else
   if fm(x2)(y2)=x+1 then
    fm(x2)(y2)=x
   endif
  endif
 next
next        
i$=wre$(x)
for z=1 to 6:wd(0)(z)=wd(x)(z):next
wre$(x)=wre$(x+1)
wre$(x+1)=i$       
for z=1 to 6
 wd(x)(z)=wd(x+1)(z)
 wd(x+1)(z)=wd(0)(z)
next    
orig(0)=orig(x)
orig(x)=orig(x+1)
orig(x+1)=orig(0) 
return 

ruleshub:
gosub clear
for x=1 to 8
ruleslot$(x)=findfirstfile("types\*.rsv"+x)  
if ruleslot$(x)="" then 
 ruleslot$(x)="UNUSED":slots(x)=0
else
 ruleslot$(x)=left$(ruleslot$(x),(len(ruleslot$(x))-5))
 ruleslots(x)=1
endif
next
if x2=1 then printr"*Choose Slot to SAVE to*" else printr "*Choose Slot to LOAD from*":endif
for x=1 to 8:printr:printr x+":":next 
gsiz=1:bl=2
for x=1 to 8:by=x*2:bt$=ruleslot$(x):gosub button:next  
bt$="Back to Previous Menu":by=34:bl=0:gosub button                                 
drawtext() 
x3=0
do
 gosub mouse 
 if sel=9 then return:endif 
 if sel>0 and sel<9 then
  if x2=1 then
   
   'save
   gosub clear
   if ruleslots(sel)=1 then 
    z3=sel
    printr "Overwrite File '"+ruleslot$(z3)+"'?"
    gsiz=1
    bt$="Yes":bl=0:by=34:gosub button
    bt$="No":bl=4:by=34:gosub button  
    drawtext()
    do
     gosub mouse  
      if sel=1 then deletefile("types\"+ruleslot$(z3)+".rsv"+z3):sel=z3:goto entermname:endif
      if sel=2 then goto ruleshub:endif
    loop
   endif      
   entermname:
   gosub clear
   printr"Input the name of this matchtypes save:-":printr
   drawtext()   
   color(0,0,128)
   input ">",i$
   color(0,0,0)  
   if i$="" then goto entermname:endif
   i$="types\"+i$+".rsv"+sel
   x3=1:return
  else
   
   'load
   if ruleslots(sel)=1 then
    i$="types\"+ruleslot$(sel)+".rsv"+sel
    x3=1:return
   
   endif 

  endif  
 endif
loop 

saverules:
x2=1:gosub ruleshub  
if x3=0 then return:endif  
f=openfilewrite(i$)
for x2#=1 to 9:writeint(f,xrule(x2#)):next
for x2#=0 to 22:writeint(f,mrule(x2#)):next
closefile(f)  
cls:printr"Matchtypes Data Saved":drawtext():sleep(1000) 
goto saverules

loadrules:
x2=2:gosub ruleshub 
if x3=0 then return:endif 
f=openfileread(i$) 
for x2#=1 to 9:xrule(x2#)=readint(f):next   
for x2#=0 to 22:mrule(x2#)=readint(f):next  
closefile(f)
cls:printr"Matchtypes Data Loaded":drawtext():sleep(1000)
return     

hub:   
gosub clear
for x=1 to 8
slot$(x)=findfirstfile("*.sv"+x)  
if slot$(x)="" then 
 slot$(x)="UNUSED":slots(x)=0
else
 slot$(x)=left$(slot$(x),(len(slot$(x))-4))
 slots(x)=1
endif
next
if x2=1 then printr"*Choose Slot to SAVE to*" else printr "*Choose Slot to LOAD from*":endif
for x=1 to 8:printr:printr x+":":next 
gsiz=1:bl=2
for x=1 to 8:by=x*2:bt$=slot$(x):gosub button:next  
bt$="Back to Previous Menu":by=34:bl=0:gosub button                                 
drawtext() 
x3=0
do
 gosub mouse 
 if sel=9 then return:endif 
 if sel>0 and sel<9 then
  if x2=1 then
   
   'save
   gosub clear
   if slots(sel)=1 then 
    z3=sel
    printr "Overwrite File '"+slot$(z3)+"'?"
    gsiz=1
    bt$="Yes":bl=0:by=34:gosub button
    bt$="No":bl=4:by=34:gosub button  
    drawtext()
    do
     gosub mouse  
      if sel=1 then i$=slot$(z3)+".sv"+z3:x3=1:return:endif
      if sel=2 then goto hub:endif
    loop
   endif 
   gosub clear
   printr"Input the name of this save file:-":printr
   printr"(Or enter a blank field to cancel save)" 
   printr
   drawtext()   
   color(0,0,128)
   input ">",i$
   color(0,0,0)  
   if i$="" then goto hub:endif
   i$=i$+".sv"+sel
   x3=1:return
  else
   
   'load
   if slots(sel)=1 then
    i$=slot$(sel)+".sv"+sel
    x3=1:return
   
   endif 

  endif  
 endif
loop
  
savegame: 
x2=1:gosub hub  
if x3=0 then return:endif    
f=openfilewrite(i$)
writeint(f,house)
writeint(f,major)
writeint(f,mode)
writeint(f,totalm)   
writeint(f,currm)   
writeint(f,tothist)    
writeint(f,realshow)
for x=1 to 24:writeint(f,lines(x)):next
for x=0 to 22:writeint(f,mrule(x)):next 
for x=1 to 11:writeint(f,xrule(x)):next
for x=1 to 12:writeint(f,tried(x)):next
for x=1 to 24:for y=1 to 4:writeint(f,fm(x)(y)):next:next   
for x=1 to 8
 for y=1 to 4:writeint(f,bd(x)(y)):writeint(f,bh(x)(y)):next    
 for y=0 to 22:writeint(f,bmrule(x)(y)):next
next    
for x=1 to 64       
 writeint(f,orig(x))
 for y=1 to 6:writeint(f,wd(x)(y)):next
next   
for x=1 to 12   
 for y=1 to 3:writeint(f,stip(x)(y)):next
 for y=1 to 11:writeint(f,match(x)(y)):next
 for y=1 to 8:writeint(f,entry(x)(y)):next  
next
for x=1 to 8:writeline(f,belt$(x)):next 
for x=1 to 24:writeline(f,fa$(x)):next
for x=1 to 64:writeline(f,wre$(x)):next  
for x=1 to 12:for y=1 to 26:writeline(f,text$(x)(y)):next:next
for x=1 to 12:for y=1 to 8:writeline(f,side$(x)(y)):next:next  
for x=1 to 24:for y=1 to 300:writeline(f,hist$(x)(y)):next:next
writeline(f,prom$)
closefile(f)  
cls:printr"Data Saved":drawtext():sleep(1000)
goto savegame
            
loadgame:   
x2=2:gosub hub 
if x3=0 then return:endif  
f=openfileread(i$) 
house=readint(f)
major=readint(f) 
mode=readint(f)
totalm=readint(f)  
currm=readint(f)  
tothist=readint(f)  
realshow=readint(f)
for x=1 to 24:lines(x)=readint(f):next
for x=0 to 22:mrule(x)=readint(f):next   
for x=1 to 11:xrule(x)=readint(f):next
for x=1 to 12:tried(x)=readint(f):next
for x=1 to 24:for y=1 to 4:fm(x)(y)=readint(f):next:next
for x=1 to 8
 for y=1 to 4:bd(x)(y)=readint(f):bh(x)(y)=readint(f):next
 for y=0 to 22:bmrule(x)(y)=readint(f):next
next   
for x=1 to 64         
 orig(x)=readint(f)
 for y=1 to 6:wd(x)(y)=readint(f):next
next
for x=1 to 12      
 for y=1 to 3:stip(x)(y)=readint(f):next
 for y=1 to 11:match(x)(y)=readint(f):next
 for y=1 to 8:entry(x)(y)=readint(f):next
next
for x=1 to 8:belt$(x)=readline(f):next    
for x=1 to 24:fa$(x)=readline(f):next
for x=1 to 64:wre$(x)=readline(f):next      
for x=1 to 12:for y=1 to 26:text$(x)(y)=readline(f):next:next 
for x=1 to 12:for y=1 to 8:side$(x)(y)=readline(f):next:next      
for x=1 to 24:for y=1 to 300:hist$(x)(y)=readline(f):next:next
prom$=readline(f) 
closefile(f)
cls:printr"Data Loaded":drawtext():sleep(1000)
return    

news:       
currline=0
if xrule(11)=1 then  
news=0

 
 
 
 
'news events 

'example......   

'chance of news
if rnd()%100=0 then     
 'setup news item, always include these lines
 if news=48 then goto sortnews:endif
 news=news+1             
 'headline
 head$(news)="SALES LETDOWN" 
 'main item
 new$(news)="Sales of "+prom$+" merchandise have been down lately, according to financial insiders."     
endif 
'end of example

for x=1 to 48 
 if wd(x)(1)=1 then 
  'individual wrestler news goes here
 
  'example.....  

  'chance of news (lower than for regular news as this is checked for each wrestler on roster)
  if rnd()%1000=0 then  
   'setup news item
   if news=48 then goto sortnews:endif
   news=news+1  
   'headline
   head$(news)=ucase$(wre$(x))+" NEW AUTHOR"
   'main item
   new$(news)=wre$(x)+" has written an autobiography, to be released soon by a major publisher." 
  endif  
  'end of example
  
  if rnd()%1000=0 then 
   'big ratings boost
   if news=48 then goto sortnews:endif
   news=news+1         
   if wd(x)(3)=3 then  
    y=rnd()%3         
    if y=0 then  
     head$(news)=ucase$(wre$(x))+" JOY"  
     new$(news)="It has been annnounced that "+wre$(x)+" is to participate in a photoshoot for Playboy. Fans are happily celebrating this long-awaited news."
    endif  
    if y=1 then  
     head$(news)=ucase$(wre$(x))+" ENGAGED"  
     new$(news)=wre$(x)+" has announced the happy news that she is to be married, to a fellow wrestler. Congratulations "+wre$(x)+"!"
    endif
    if y=2 then  
     head$(news)=ucase$(wre$(x))+" ENHANCEMENT"  
     new$(news)=wre$(x)+" is reported to have had a boob job. Friends say that she is very happy with the results of the surgery."
    endif
   else 
    y=rnd()%2         
    if y=0 then 
     head$(news)=ucase$(wre$(x))+" BREAKTHROUGH"  
     new$(news)=wre$(x)+" has achieved widespread recognition after starring in a new Hollywood blockbuster."
     new$(news)=new$(news)+" Film critics have lined up to praise this new star's screen presence." 
    endif 
    if y=1 then 
     head$(news)=ucase$(wre$(x))+" PASSES TEST"  
     new$(news)=wre$(x)+" has won much kudos after facing down a famous sports star."
     new$(news)=new$(news)+" Fans are praising "+wre$(x)+" for proving himself to be a legitimate tough guy." 
    endif
   endif
   new$(news)=new$(news)+" ("+wre$(x)+" gains +40 Rating pts.)"    
   wd(x)(2)=wd(x)(2)+40
  endif    
  
  if rnd()%1000=0 then 
   'big ratings loss
   if news=48 then goto sortnews:endif
   news=news+1       
   y=rnd()%2
   if y=0 then
    head$(news)=ucase$(wre$(x))+" SHOCK"
    new$(news)=wre$(x)+" has been found to be behind the wheel of a vehicle whilst under the influence of drugs and alcohol."
    new$(news)=new$(news)+" This news will be of great disappointment to the fans."  
   endif
   if y=1 then
    head$(news)=ucase$(wre$(x))+" IS GAME FAN"
    new$(news)=wre$(x)+" has enthusiastically endorsed the latest version of the Smackdown Versus Raw videogame. "
    new$(news)=new$(news)+wre$(x)+" said the game was the finest simulation of wrestling available on the market."
   endif   
   new$(news)=new$(news)+" ("+wre$(x)+" loses -40 Rating pts.)" 
   wd(x)(2)=wd(x)(2)-40
  endif  
  
  if rnd()%150=0 then 
   'ratings boost
   if news=48 then goto sortnews:endif
   news=news+1  
   y=rnd()%3         
   if y=0 then  
    head$(news)=ucase$(wre$(x))+" OVER" 
    new$(news)=wre$(x)+" has cut a fine promo which has boosted popularity with the fans."  
   endif   
   if y=1 then   
    head$(news)=ucase$(wre$(x))+" BOOST" 
    new$(news)=wre$(x)+" has won favor with an influential backstage staff member."  
   endif    
   if y=2 then       
    head$(news)=ucase$(wre$(x))+" EXCELS" 
    new$(news)=wre$(x)+" has showed an impressive state of fitness and application recently."  
   endif  
   new$(news)=new$(news)+" ("+wre$(x)+" gains +5 Rating pts.)"  
   wd(x)(2)=wd(x)(2)+5
  endif 

  if rnd()%150=0 then 
   'ratings loss
   if news=48 then goto sortnews:endif
   news=news+1  
   y=rnd()%3
   if y=0 then     
    head$(news)=ucase$(wre$(x))+" FAILS TO IMPRESS"  
    new$(news)=wre$(x)+" has cut a rambling, confused promo which has left the fans cold." 
   endif
   if y=1 then   
    head$(news)=ucase$(wre$(x))+" BLUNDER"  
    new$(news)=wre$(x)+" has accidentally tumbled out of the ring after a promo, causing much merriment amongst the fans." 
   endif    
   if y=2 then
    head$(news)=ucase$(wre$(x))+" UNIMPRESSIVE"  
    new$(news)=wre$(x)+" has been looking unmotivated and out of shape recently."  
   endif 
   new$(news)=new$(news)+" ("+wre$(x)+" loses -5 Rating pts.)"  
   wd(x)(2)=wd(x)(2)-5
  endif  
  
  if rnd()%150=0 then
   'alignment swing
   if wd(x)(5)=1 then
    'face
    if rnd()%2=0 then
     if news=48 then goto sortnews:endif
     news=news+1  
     head$(news)=ucase$(wre$(x))+" BETRAYAL"
     new$(news)=wre$(x)+" has turned "
     if wd(x)(3)=3 then new$(news)=new$(news)+"her" else new$(news)=new$(news)+"his":endif
     new$(news)=new$(news)+" back on the fans, claiming not to need or want their backing any more."
     new$(news)=new$(news)+" The fans have vowed never to support this individual again."
     new$(news)=new$(news)+" ("+wre$(x)+" shifts from Babyface to Heel.)"
     wd(x)(5)=2
    else
     if news=48 then goto sortnews:endif
     news=news+1  
     head$(news)=ucase$(wre$(x))+" UNCERTAINTY"
     new$(news)=wre$(x)+" has started to behave in a dark and edgy fashion of late."   
     new$(news)=new$(news)+" Fans have been unsure what to make of this new attitude."
     new$(news)=new$(news)+" ("+wre$(x)+" shifts from Babyface to Neutral.)"
     wd(x)(5)=3
    endif 
    goto endshift
   endif
   if wd(x)(5)=2 then
    'heel
    if rnd()%2=0 then
     if news=48 then goto sortnews:endif
     news=news+1  
     head$(news)=ucase$(wre$(x))+" NEW FAN FAVOURITE"
     new$(news)=wre$(x)+" has vowed to win the support of fans by wrestling with fairness and honor in future."   
     new$(news)=new$(news)+" The fans have welcomed this new development."
     new$(news)=new$(news)+" ("+wre$(x)+" shifts from Heel to Babyface.)"
     wd(x)(5)=1
    else
     if news=48 then goto sortnews:endif
     news=news+1  
     head$(news)=ucase$(wre$(x))+" UNCERTAINTY"
     new$(news)=wre$(x)+" has started to behave in a mysterious and enigmatic fashion of late."   
     new$(news)=new$(news)+" Fans have been unsure what to make of this new attitude."
     new$(news)=new$(news)+" ("+wre$(x)+" shifts from Heel to Neutral.)"
     wd(x)(5)=3
    endif
    goto endshift
   endif
   if wd(x)(5)=3 then
    'neutral
    if rnd()%2=0 then
     if news=48 then goto sortnews:endif
     news=news+1  
     head$(news)=ucase$(wre$(x))+" NEW FAN FAVOURITE"
     new$(news)=wre$(x)+" has won favor with the fans by behaving in a decent and honorable manner lately."
     new$(news)=new$(news)+" ("+wre$(x)+" shifts from Neutral to Babyface.)"
     wd(x)(5)=1
    else
     if news=48 then goto sortnews:endif
     news=news+1  
     head$(news)=ucase$(wre$(x))+" ANIMOSITY"
     new$(news)=wre$(x)+" has lost favor with the fans by behaving in a cowardly and treacherous manner lately."
     new$(news)=new$(news)+" ("+wre$(x)+" shifts from Neutral to Heel.)"
     wd(x)(5)=2
    endif
   endif  
  endif
  endshift:
 endif
next

for x=1 to 64   
 
 if wd(x)(1)=1 then 

  if rnd()%50=0 then 
 
  'specific named wrestler news goes here

   if wre$(x)="Sandman" or wre$(x)="The Sandman" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" EMBARASSMENT"
    new$(news)=wre$(x)+" has been humiliated after turning up leglessly drunk to perform at an indy show."
    new$(news)=new$(news)+" To compound his misery the entire episode was filmed and posted on Youtube."
    new$(news)=new$(news)+" ("+wre$(x)+" loses -20 Rating pts.)"  
    wd(x)(2)=wd(x)(2)-20
   endif  
   if wre$(x)="Terry Funk" or wre$(x)="Hulk Hogan" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" RETIREMENT?"
    new$(news)=wre$(x)+" has announced his retirement whilst speaking at a family member's wedding."
    new$(news)=new$(news)+" However, the 'retirement' was greeted with scepticism by experienced wrestling commentators, who do not expect it to last."
   endif  
   if wre$(x)="Chris Jericho" or wre$(x)="Lita" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" LETDOWN"
    new$(news)="Sales of "+wre$(x)+"'s new album have been disappointing, according to industry insiders."  
   endif 
   if wre$(x)="Mick Foley" or wre$(x)="Mankind" or wre$(x)="Cactus Jack" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" SPLASHES OUT"
    new$(news)="Mick Foley has purchased a new shirt, according to reports."
    new$(news)=new$(news)+" ("+wre$(x)+" gains +20 Rating pts.)"  
    wd(x)(2)=wd(x)(2)+20
   endif  
   if wre$(x)="John Cena" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" IN TRAINING"
    new$(news)=wre$(x)+" has been training on the heavy bag recently in an attempt to learn punching skills." 
   endif     
   if wre$(x)="Goldberg" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" SPEAKS OUT"
    new$(news)=wre$(x)+" has complained that his opponents of late have not provided worthy enough opposition for him." 
   endif
   if wre$(x)="Mr Kennedy" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" SPEAKS OUT"
    new$(news)=wre$(x)+" has said on a talk show that there is no longer any drug use within wrestling, to his knowledge." 
    new$(news)=new$(news)+" ("+wre$(x)+" loses -20 Rating pts.)"  
    wd(x)(2)=wd(x)(2)-20
   endif
   if wre$(x)="Big Show" or wre$(x)="The Big Show" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" WEIGHT TROUBLE"
    new$(news)="Fans have remarked on how overweight "+wre$(x)+" is looking lately."
    new$(news)=new$(news)+" It is thought that he could do with slimming down as his matches are being adversely affected."
    new$(news)=new$(news)+" ("+wre$(x)+" loses -20 Rating pts.)"  
    wd(x)(2)=wd(x)(2)-20
   endif  
   if wre$(x)="Batista" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" SHAME"
    new$(news)=wre$(x)+" has been beaten up in a demeaning backstage brawl."
    new$(news)=new$(news)+" It is rumored that he initiated the scuffle himself."
    new$(news)=new$(news)+" ("+wre$(x)+" loses -20 Rating pts.)"  
    wd(x)(2)=wd(x)(2)-20
   endif 
   if wre$(x)="Randy Orton" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" IN TROUBLE"
    new$(news)=wre$(x)+" has been disciplined by his employers after a backstage incident involving a female employee."
    new$(news)=new$(news)+" ("+wre$(x)+" loses -20 Rating pts.)"  
    wd(x)(2)=wd(x)(2)-20
   endif  
   if wre$(x)="Triple H" then
    if news=48 then goto sortnews:endif
    news=news+1  
    head$(news)=ucase$(wre$(x))+" IN FAVOR"
    new$(news)=wre$(x)+"'s wife has suggested it is time he was given another big push."
    new$(news)=new$(news)+" The suggestion has been greeted very positively by top staff within "+prom$+"."
    new$(news)=new$(news)+" ("+wre$(x)+" gains +20 Rating pts.)"  
    wd(x)(2)=wd(x)(2)+20
   endif 

  endif  
 endif
next

if news=0 then goto card:endif

sortnews:     

gosub checksort

for x=1 to news 
 y=1
 z=0
 temp$="" 
 
 findword: 
  if y>len(new$(x)) then goto alldone:endif
  if mid$(new$(x),y,1)=" " then
   y=y+1:goto findword
  endif  
  y2=y+1

 findendword: 
  if y2>len(new$(x)) then goto addword:endif
  if mid$(new$(x),y2,1)<>" " then
   y2=y2+1:goto findendword 
  endif   
  
 addword:
  if z+(y2-y)>49 then 
   for x2=1 to (50-z)
    temp$=temp$+" " 
   next
   z=0
  endif

  temp$=temp$+mid$(new$(x),y,(y2-y))+" "
  z=z+(y2-y)+1:y=y2:goto findword

 alldone: 
 new$(x)=temp$  

next

left=news:x=1     
gosub clear:printr "*NEWS UPDATES*":printr
currline=2  

printnews: 

if left=0 then goto card:endif 

x#=len(new$(x)):x#=x#/50:x#=x#+3:x#=int(x#)
if (currline+x#)>34 then  
 drawtext():gosub mouse
 gosub clear:printr "*NEWS UPDATES*":printr
 currline=2
endif 

currline=currline+x#
printr head$(x):printr new$(x):printr
left=left-1:x=x+1:goto printnews 

endif 
goto card

cardnews:
news2=news:news=0 

'show news goes here

'example.....

'chance of news 
if rnd()%20=0 then 
 'setup news item
 if news=48 then goto sortnews2:endif
 news=news+1  
 'headline
 head$(news)="SHOW TRIUMPH" 
 'main item
 new$(news)="Tonight's show has attracted a sell-out crowd, to the delight of the organisers."
endif 
'end of example 

if house=0 and major=1 then
 if news=48 then goto sortnews2:endif
 news=news+1  
 head$(news)="THE BIG SHOW"
 new$(news)="Fans of "+prom$+" around the world are full of excitement and anticipation as the showpiece event of the year prepares to get underway."
endif

for x=1 to totalm   
 'individual match news goes here

 'stipulations  
 if stip(x)(1)=1 then
  if news=48 then goto sortnews2:endif
  news=news+1  
  head$(news)="MATCH STIPULATION"
  new$(news)="Due to a a special stipulation, the loser in the upcoming match between "+side$(x)(1)+" and "+side$(x)(2)+" will be fired from "+prom$+"!" 
 endif
 if stip(x)(1)=2 then
  if news=48 then goto sortnews2:endif
  news=news+1  
  head$(news)="MATCH STIPULATION"
  new$(news)="Due to a a special stipulation, the losing faction in the upcoming match between "+side$(x)(1)+" and "+side$(x)(2)+" will be permanently broken up!" 
 endif

next 

if news=0 then 
 if news2>0 then drawtext():gosub mouse:endif
 return
endif

sortnews2:     

for x=1 to news 
 y=1
 z=0
 temp$="" 
 
 findword2: 
  if y>len(new$(x)) then goto alldone2:endif
  if mid$(new$(x),y,1)=" " then
   y=y+1:goto findword2
  endif  
  y2=y+1

 findendword2: 
  if y2>len(new$(x)) then goto addword2:endif
  if mid$(new$(x),y2,1)<>" " then
   y2=y2+1:goto findendword2 
  endif   
  
 addword2:
  if z+(y2-y)>49 then 
   for x2=1 to (50-z)
    temp$=temp$+" " 
   next
   z=0
  endif

  temp$=temp$+mid$(new$(x),y,(y2-y))+" "
  z=z+(y2-y)+1:y=y2:goto findword2

 alldone2: 
 new$(x)=temp$  

next

left=news:x=1 

if currline=0 then
 gosub clear:printr "*NEWS UPDATES*":printr
 currline=2
endif 

printnews2: 

if left=0 then 
 drawtext():gosub mouse
 return
endif 

x#=len(new$(x)):x#=x#/50:x#=x#+3:x#=int(x#)
if (currline+x#)>34 then 
 drawtext():gosub mouse
 gosub clear:printr "*NEWS UPDATES*":printr
 currline=2
endif 

currline=currline+x#
printr head$(x):printr new$(x):printr
left=left-1:x=x+1:goto printnews2 
