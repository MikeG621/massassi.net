---
title: Easy Particles
author: Dustino
email: dustino@hyperaction.net
description: >
    How to add particle fields to a level using easy_particle.cog. All the files needed for the tutorial are included in the zip.
date: 2000-07-18
original: original.html
category: jk
---
-----

Author: Dustino

###Before You Get Started:###
Be sure to download the [easy\_particle.zip](easy_particle.zip) file
that contains everything you need.

###Description of Each File in easy\_particle.zip:###
1.  **particle\_tutorial.txt**: This is the file you are reading now.
2.  **easy\_particle.cog**: This COG displays up to ten particle fields
in a level using ghost positions.
3.  **00teleport.mat**: This is the animated MAT that is used in the
particle field used for teleporting and Force Protection.
4.  **sphere.par**: This is the PAR that is used for teleporting and
force protection.

###Other Files Needed:###
> **master.tpl** (for JK Project) -or- **mots.tpl** (for MOTS Project)

- The master.tpl and mots.tpl can be found in the jed/jeddata folder
- Copy the filed needed into your project directory

-----

If you want to make your own PARTICLE FIELD here is what the sphere PAR
used in this tutorial looks like:

```
###############
SECTION: HEADER

PAR 1.0

SIZE .002

MATERIAL 00teleport.mat

LIGHTINGMODE 0


###############
SECTION: GEOMETRYDEF

# Object radius
RADIUS   0.109546

# Insertion offset
INSERT OFFSET   0.000000   0.000000   0.108216

VERTICES 100

# num:     x:         y:         z:         i:
0:  -0.000159  -0.109326  -0.000158   0.000000
1:   0.026518   0.036442   0.099403   0.000000
2:   0.072725   0.036442  -0.073042   0.000000
3:  -0.099720   0.036442  -0.026836   0.000000
4:   0.007469  -0.105279   0.028309   0.000000
5:   0.014532  -0.093437   0.054668   0.000000
6:   0.020507  -0.074677   0.076968   0.000000
7:   0.024952  -0.050388   0.093557   0.000000
8:   0.027538  -0.022368   0.103208   0.000000
9:   0.028073   0.007307   0.105206   0.000000
10:   0.020680  -0.105279  -0.020998   0.000000
11:   0.039976  -0.093437  -0.040294   0.000000
12:   0.056301  -0.074677  -0.056619   0.000000
13:   0.068446  -0.050388  -0.068763   0.000000
14:   0.075511  -0.022368  -0.075828   0.000000
15:   0.076973   0.007307  -0.077291   0.000000
16:  -0.028626  -0.105279  -0.007786   0.000000
17:  -0.054985  -0.093437  -0.014849   0.000000
18:  -0.077285  -0.074677  -0.020824   0.000000
19:  -0.093875  -0.050388  -0.025269   0.000000
20:  -0.103526  -0.022368  -0.027855   0.000000
21:  -0.105524   0.007307  -0.028391   0.000000
22:   0.048912   0.048986   0.084367   0.000000
23:   0.067673   0.057903   0.063073   0.000000
24:   0.081412   0.062532   0.037097   0.000000
25:   0.089111   0.062532   0.008363   0.000000
26:   0.090201   0.057903  -0.021002   0.000000
27:   0.084601   0.048986  -0.048824   0.000000
28:   0.048506   0.048986  -0.084918   0.000000
29:   0.020684   0.057903  -0.090519   0.000000
30:  -0.008681   0.062532  -0.089429   0.000000
31:  -0.037415   0.062532  -0.081730   0.000000
32:  -0.063390   0.057903  -0.067991   0.000000
33:  -0.084684   0.048986  -0.049230   0.000000
34:  -0.097896   0.048986   0.000076   0.000000
35:  -0.088835   0.057903   0.026971   0.000000
36:  -0.073209   0.062532   0.051857   0.000000
37:  -0.052174   0.062532   0.072892   0.000000
38:  -0.027288   0.057903   0.088518   0.000000
39:  -0.000394   0.048986   0.097579   0.000000
40:   0.030531  -0.104607   0.008065   0.000000
41:   0.041934  -0.093912   0.036732   0.000000
42:   0.054740  -0.093912  -0.011060   0.000000
43:   0.054150  -0.071314   0.062428   0.000000
44:   0.073081  -0.078758   0.019466   0.000000
45:   0.078167  -0.071314  -0.027205   0.000000
46:   0.063727  -0.034635   0.081519   0.000000
47:   0.089597  -0.041307   0.046636   0.000000
48:   0.100969  -0.041307   0.004195   0.000000
49:   0.096006  -0.034635  -0.038950   0.000000
50:   0.062060   0.011145   0.089042   0.000000
51:   0.088597   0.013648   0.062198   0.000000
52:   0.104506   0.014518   0.027887   0.000000
53:   0.107884   0.013648  -0.009782   0.000000
54:   0.098324   0.011145  -0.046299   0.000000
55:  -0.008383  -0.104607  -0.030849   0.000000
56:   0.010742  -0.093912  -0.055057   0.000000
57:  -0.037049  -0.093912  -0.042251   0.000000
58:   0.026887  -0.071314  -0.078484   0.000000
59:  -0.019784  -0.078758  -0.073399   0.000000
60:  -0.062745  -0.071314  -0.054467   0.000000
61:   0.038632  -0.034635  -0.096324   0.000000
62:  -0.004512  -0.041307  -0.101287   0.000000
63:  -0.046953  -0.041307  -0.089914   0.000000
64:  -0.081836  -0.034635  -0.064045   0.000000
65:   0.045981   0.011145  -0.098642   0.000000
66:   0.009465   0.013648  -0.108201   0.000000
67:  -0.028204   0.014518  -0.104824   0.000000
68:  -0.062515   0.013648  -0.088914   0.000000
69:  -0.089360   0.011145  -0.062377   0.000000
70:  -0.022626  -0.104607   0.022309   0.000000
71:  -0.053154  -0.093912   0.017850   0.000000
72:  -0.018168  -0.093912   0.052836   0.000000
73:  -0.081515  -0.071314   0.015582   0.000000
74:  -0.053775  -0.078758   0.053457   0.000000
75:  -0.015899  -0.071314   0.081197   0.000000
76:  -0.102837  -0.034635   0.014330   0.000000
77:  -0.085562  -0.041307   0.054176   0.000000
78:  -0.054493  -0.041307   0.085245   0.000000
79:  -0.014648  -0.034635   0.102519   0.000000
80:  -0.108519   0.011145   0.009125   0.000000
81:  -0.098539   0.013648   0.045529   0.000000
82:  -0.076780   0.014518   0.076462   0.000000
83:  -0.045846   0.013648   0.098221   0.000000
84:  -0.009442   0.011145   0.108201   0.000000
85:   0.022626   0.064825   0.084876   0.000000
86:  -0.005470   0.078639   0.075603   0.000000
87:   0.042321   0.078639   0.062797   0.000000
88:  -0.033497   0.088502   0.054689   0.000000
89:   0.012518   0.097740   0.047152   0.000000
90:   0.056136   0.088502   0.030672   0.000000
91:  -0.059089   0.089656   0.020848   0.000000
92:  -0.019825   0.106927   0.011331   0.000000
93:   0.022617   0.106927  -0.000041   0.000000
94:   0.061379   0.089656  -0.011432   0.000000
95:  -0.077726   0.074713  -0.018959   0.000000
96:  -0.048268   0.091495  -0.035744   0.000000
97:  -0.013050   0.097321  -0.048268   0.000000
98:   0.023712   0.091495  -0.055031   0.000000
99:   0.057615   0.074713  -0.055224   0.000000
```
For a description of what each section does in a .PAR checkout the PAR
section at Code Alliance's JK specs:

<http://www.code-alliance.com/~editors/jediknight/docs/jk_specs/jkspecs.htm>

Now you have all of the files in their correct spots in the project
directory and can now begin the addition of particle fields into your
level.

###Steps for Adding Particle Fields:###

1.  Open up JED and start a new JK/MOTS level.

2.  Save the .jed file in your project directory.

3.  Minimize JED and open your project directory.

4.  Open **master.tpl** or **mots.tpl** (depending on which you copied
to the folder).

5.  At the very bottom (always add to the bottom of templates) of the
template add the following lines:  
`# DESC:`  
`# BBOX: 0 0 0 0 0 0`  
`+tut_sphere   none   orient=(0.000000/0.000000/0.000000) type=cog move=physics`  
`timer=60 particle=sphere.par angvel=(60.000000/60.000000/60.000000)`

6.  Remember the number for Timer in the template entry you just added.

7.  Save the template and close it.

8.  Now maximize JED.

9.  Now go to **Commands** and click RELOAD TEMPLATES (always hit reload
templates when you have edited the template manually).

10. Now go to THING and insert a GHOST (Remember the thing \# of this
ghost).

11. Now goto **Tools** and click PLACED COGS.

12. Click ADD COG.

13. In the Resource Picker click cog/

14. Select **easy\_particle.cog**

15. Click OK.

16. Setup the COG
> **Description of each Option:**
>> **PARx** (thing): These are where the thing \# of your ghosts go.
>> Since you only have added 1 ghost so far place its thing \# in the
>> par0 (thing) box.  
>>   
>> **PAR\_LENGTH** (flex): This is where the length of the timer
>> (that I said to remember when you added the particle template
>> entry into the template). This restarts the particle field once it
>> ends.  
>>   
>> **PAR** (template): Here you select the template entry you added
>> earlier, +tut\_sphere.

17. Click REFRESH and then OK.

18. Now Save the .jed, setup the level in the Episode Editor, and save
the .jkl and .gob.

19. Run the level.

20. Enjoy\!
