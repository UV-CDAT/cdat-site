---
layout: default
title:
---

 [ Skip to content. ](/cdat/source/api-reference/vcs.yxvsx.html) | [ Skip to
navigation ](/cdat/source/api-reference/vcs.yxvsx.html)

Search Site

[ Advanced Search&#8230; ](/search_form)

#  [ PCMDI Software Portal ](/)

#####  Sections

  * [ Home ](/)

#####  Personal tools

  * [ Log in ](/login_form)

You are here:  [ Home ](/) -> [ CDAT ](/cdat) -> [ Source Code ](/cdat/source)
-> [ API Reference ](/cdat/source/api-reference) -> Python: module vcs.yxvsx

[ Navigation ](/sitemap)

    

  * [ Home ](/)

  * [ PCMDI Home Page ](/)

  * [ News ](/news)

  * [ CDAT ](/cdat)

    * [ Download and Install ](/cdat/download)

    * [ Screenshots ](/cdat/screenshots)

    * [ Contrib Packages ](/cdat/contrib)

    * [ Getting Started ](/cdat/getting_started)

    * [ Tutorials ](/cdat/tutorials)

    * [ Quick Reference ](/cdat/quick_reference)

    * [ FAQ ](/cdat/FAQ)

    * [ Manuals ](/cdat/manuals)

    * [ Tips and Tricks ](/cdat/tips_and_tricks)

    * [ Source Code ](/cdat/source)

      * [ API Reference ](/cdat/source/api-reference)

        * [ Python: module vcs.yxvsx ](/cdat/source/api-reference/vcs.yxvsx.html)

    * [ Contact Us ](/cdat/contact-us)

    * [ Documents ](/cdat/docs)

    * [ Support ](/cdat/support)

  * [ CMOR ](/cmor)

  * [ IPCC AR4 Model Data Portal ](/esg_data_portal)

  * [ About Us ](/about)

  * [ Newsletter ](/Newsletter)

[ News ](/news)

     [ ![](media/newsitem_icon.gif) CDAT Newsletter, June 2007  2007-06-26  ](/Newsletter/Vol3/index_d.html)
     [ ![](media/newsitem_icon.gif) CDAT 4.1.2 Released  2006-06-07  ](/cdat_4_1_2)
     [ ![](media/newsitem_icon.gif) CDAT 4.0 Released  2005-11-21  ](/cdat_4_0)
     [ ![](media/newsitem_icon.gif) PCMDI Software Portal Released  2005-09-28  ](/software_portal_release)
     [ ![](media/newsitem_icon.gif) CDAT 4.0 Beta Released  2005-09-28  ](/cdat_4_0_beta)
     [ More news&#8230; ](/news)

#####  Document Actions

  * [ ![Send this page to somebody](media/mail_icon.gif) ](/cdat/source/api-reference/vcs.yxvsx.html/sendto_form)
  * [ ![Print this page](media/print_icon.gif) ](/this.print\(\))

#  Python: module vcs.yxvsx

  
  
 [ vcs  ](/vcs.html) .yxvsx 
[ index ](/)  

` #&#160;Yxvsx&#160;( [ GYx ](/) )&#160;module `

  
 Modules 

` `

[ vcs.Canvas ](/vcs.Canvas.html)  
[ Numeric ](/Numeric.html)  

[ vcs.VCS_validation_functions ](/vcs.VCS_validation_functions.html)  
[ vcs._vcs ](/vcs._vcs.html)  

[ cdms ](/cdms.html)  
[ cdtime ](/cdtime.html)  

[ vcs.queries ](/vcs.queries.html)  
[ string ](/string.html)  

  
 Classes 

` `

[ __builtin__.object ](/__builtin__.html)

    

[ GYx ](/vcs.yxvsx.html)

  
class  GYx  ( [ __builtin__.object ](/__builtin__.html) )

` `

` Class: [ GYx ](/) #&#160;Yxvsx  
  
Description&#160;of [ GYx ](/) Class:  
The&#160;Yxvsx&#160;graphics&#160;method&#160;displays&#160;a&#160;line&#160;plot&#160;from&#160;a&#160;1D&#160;data&#160;array&#160;(i.e.&#160;a  
plot&#160;of&#160;Y(x),&#160;where&#160;y&#160;represents&#160;the&#160;1D&#160;coordinate&#160;values).&#160;The&#160;example&#160;below  
shows&#160;how&#160;to&#160;change&#160;line&#160;and&#160;marker&#160;attributes&#160;for&#160;the&#160;Yxvsx&#160;graphics&#160;method.  
  
This&#160;class&#160;is&#160;used&#160;to&#160;define&#160;an&#160;Yxvsx&#160;table&#160;entry&#160;used&#160;in&#160;VCS,&#160;or&#160;it&#160;can&#160;be  
used&#160;to&#160;change&#160;some&#160;or&#160;all&#160;of&#160;the&#160;Yxvsx&#160;attributes&#160;in&#160;an&#160;existing&#160;Yxvsx&#160;table  
entry.  
  
Other&#160;Useful&#160;Functions:  
a=vcs.init()&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Constructor  
a.show('yxvsx')&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Show&#160;predefined&#160;Yxvsx&#160;graphics&#160;methonds  
a.show('line')&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Show&#160;predefined&#160;VCS&#160;line&#160;objects  
a.show('marker')&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Show&#160;predefined&#160;VCS&#160;marker&#160;objects  
a.setcolormap("AMIP")&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Change&#160;the&#160;VCS&#160;color&#160;map  
a.yxvsx(s,&#160;x,&#160;'default')&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Plot&#160;data&#160;'s'&#160;with&#160;Yxvsx&#160;'x'  
and&#160;'default'&#160;template  
a.update()&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Updates&#160;the&#160;VCS&#160;Canvas&#160;at&#160;user's&#160;request  
a.mode=1,&#160;or&#160;0&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;If&#160;1,&#160;then&#160;automatic&#160;update,&#160;else&#160;if  
0,&#160;then&#160;use&#160;update&#160;function&#160;to  
  
Example&#160;of&#160;Use:  
a=vcs.init()  
To&#160;Create&#160;a&#160;new&#160;instance&#160;of&#160;Yxvsx&#160;use:  
yxx=a.createxyvsy('new','quick')&#160;&#160;&#160;&#160;#&#160;Copies&#160;content&#160;of&#160;'quick'&#160;to&#160;'new'  
yxx=a.createxyvsy('new')&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Copies&#160;content&#160;of&#160;'default'&#160;to&#160;'new'  
  
To&#160;Modify&#160;an&#160;existing&#160;Yxvsx&#160;use:  
yxx=a.getxyvsy('AMIP_psl')  
  
yxx. [ list ](/) ()&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Will&#160;list&#160;all&#160;the&#160;Yxvsx
attribute&#160;values  
yxx.projection='linear'&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Can&#160;only&#160;be&#160;'linear'  
lon30={-180:'180W',-150:'150W',0:'Eq'}  
yxx.xticlabels1=lon30  
yxx.xticlabels2=lon30  
yxx. [ xticlabels ](/) (lon30,&#160;lon30)&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Will&#160;set&#160;them&#160;both  
yxx.xmtics1=''  
yxx.xmtics2=''  
yxx. [ xmtics ](/) (lon30,&#160;lon30)&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Will&#160;set&#160;them&#160;both  
yxx.yticlabels1=lat10  
yxx.yticlabels2=lat10  
yxx. [ yticlabels ](/) (lat10,&#160;lat10)&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Will&#160;set&#160;them&#160;both  
yxx.ymtics1=''  
yxx.ymtics2=''  
yxx. [ ymtics ](/) (lat10,&#160;lat10)&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Will&#160;set&#160;them&#160;both  
yxx.datawc_y1=-90.0  
yxx.datawc_y2=90.0  
yxx.datawc_x1=-180.0  
yxx.datawc_x2=180.0  
yxx. [ datawc ](/) (-90,&#160;90,&#160;-180,&#160;180)&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Will&#160;set&#160;them&#160;all  
yxx.xaxisconvert='linear'  
  
Specify&#160;the&#160;Yxvsx&#160;line&#160;type:  
yxx.line=0&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;same&#160;as&#160;yxx.line&#160;=&#160;'solid'  
yxx.line=1&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;same&#160;as&#160;yxx.line&#160;=&#160;'dash'  
yxx.line=2&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;same&#160;as&#160;yxx.line&#160;=&#160;'dot'  
yxx.line=3&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;same&#160;as&#160;yxx.line&#160;=&#160;'dash-dot'  
yxx.line=4&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;same&#160;as&#160;yxx.line&#160;=&#160;'long-dash  
  
Specify&#160;the&#160;Yxvsx&#160;line&#160;color:  
yxx.linecolor=16&#160;&#160;&#160;&#160;#&#160;color&#160;range:&#160;16&#160;to&#160;230,&#160;default&#160;color&#160;is&#160;black  
yxx.linewidth=1&#160;&#160;&#160;&#160;&#160;#&#160;width&#160;range:&#160;1&#160;to&#160;100,&#160;default&#160;color&#160;is&#160;1  
  
Specify&#160;the&#160;Yxvsx&#160;marker&#160;type:  
yxx.marker=1&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='dot'  
yxx.marker=2&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='plus'  
yxx.marker=3&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='star'  
yxx.marker=4&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='circle'  
yxx.marker=5&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='cross'  
yxx.marker=6&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='diamond'  
yxx.marker=7&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='triangle_up'  
yxx.marker=8&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='triangle_down'  
yxx.marker=9&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='triangle_left'  
yxx.marker=10&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='triangle_right'  
yxx.marker=11&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='square'  
yxx.marker=12&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='diamond_fill'  
yxx.marker=13&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='triangle_up_fill'  
yxx.marker=14&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='triangle_down_fill'  
yxx.marker=15&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='triangle_left_fill'  
yxx.marker=16&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='triangle_right_fill'  
yxx.marker=17&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;yxx.marker='square_fill'  
yxx.marker=None&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Draw&#160;no&#160;markers  
  
There&#160;are&#160;four&#160;possibilities&#160;for&#160;setting&#160;the&#160;marker&#160;color&#160;index&#160;(Ex):  
yxx.markercolors=22&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;below  
yxx.markercolors=(22)&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Same&#160;as&#160;below  
yxx.markercolors=([22])&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Will&#160;set&#160;the&#160;markers&#160;to&#160;a&#160;specific  
color&#160;index  
yxx.markercolors=None&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Color&#160;index&#160;defaults&#160;to&#160;Black  
  
To&#160;set&#160;the&#160;Yxvsx&#160;Marker&#160;sizie:  
yxx.markersize=5  
yxx.markersize=55  
yxx.markersize=100  
yxx.markersize=300  
yxx.markersize=None  
`

Methods defined here:  

 __init__  (self, parent, GYx_name  =None  , GYx_name_src  ='default'  , createGYx  =0  ) 

 datawc  (self, dsp1  =1e+20  , dsp2  =1e+20  , dsp3  =1e+20  , dsp4  =1e+20  ) 

 list  (self) 

 rename  = renameGYx(self, old_name, new_name) 
     ` ###############################################################################   
#
#  
#&#160;Function:&#160;&#160;&#160;&#160;&#160;renameGYx
#  
#
#  
#&#160;Description&#160;of&#160;Function:
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;Private&#160;function&#160;that&#160;renames&#160;the&#160;name&#160;of&#160;an&#160;existing&#160;Yxvsx
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;graphics&#160;method.
#  
#
#  
#
#  
#&#160;Example&#160;of&#160;Use:
#  
# [ renameGYx ](/) (old_name,&#160;new_name)
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;where:&#160;old_name&#160;is&#160;the&#160;current&#160;name&#160;of&#160;Yxvsx&#160;graphics&#160;method
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;new_name&#160;is&#160;the&#160;new&#160;name&#160;for&#160;the&#160;Yxvsx&#160;graphics&#160;method
#  
#
#  
##############################################################################
# `

 script  (self, script_filename  =None  , mode  =None  ) 
     ` Function:&#160;&#160;&#160;&#160;&#160;script&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Calls&#160;_vcs.scriptGYx   
  
Description&#160;of&#160;Function:  
Saves&#160;out&#160;a&#160;boxfill&#160;graphics&#160;method&#160;in&#160;Python&#160;or&#160;VCS&#160;script&#160;form&#160;to&#160;a  
designated&#160;file.  
  
Example&#160;of&#160;Use:  
[ script ](/) (scriptfile_name,&#160;mode)  
where:&#160;scriptfile_name&#160;is&#160;the&#160;output&#160;name&#160;of&#160;the&#160;script&#160;file.  
mode&#160;is&#160;either&#160;"w"&#160;for&#160;replace&#160;or&#160;"a"&#160;for&#160;append.  
  
Note:&#160;If&#160;the&#160;the&#160;filename&#160;has&#160;a&#160;".py"&#160;at&#160;the&#160;end,&#160;it&#160;will&#160;produce&#160;a  
Python&#160;script.&#160;If&#160;the&#160;filename&#160;has&#160;a&#160;".scr"&#160;at&#160;the&#160;end,&#160;it&#160;will  
produce&#160;a&#160;VCS&#160;script.&#160;If&#160;neither&#160;extensions&#160;are&#160;give,&#160;then&#160;by  
default&#160;a&#160;Python&#160;script&#160;will&#160;be&#160;produced.  
  
a=vcs.init()  
Yx=a.createboxfill('temp')  
Yx. [ script ](/) ('filename.py')&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Append&#160;to&#160;a&#160;Python&#160;file
"filename.py"  
Yx. [ script ](/) ('filename.scr')&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;#&#160;Append&#160;to&#160;a&#160;VCS&#160;file
"filename.scr"  
Yx. [ script ](/) ('filename','w') `

 xmtics  (self, xmt1  =''  , xmt2  =''  ) 

 xticlabels  (self, xtl1  =''  , xtl2  =''  ) 

 ymtics  (self, ymt1  =''  , ymt2  =''  ) 

 yticlabels  (self, ytl1  =''  , ytl2  =''  ) 

* * *

Properties defined here:  

 datawc_calendar 
    

 _ get _  = _getcalendar(self) 
    

 _ set _  = _setcalendar(self, value) 

 datawc_timeunits 
    

 _ get _  = _gettimeunits(self) 
    

 _ set _  = _settimeunits(self, value) 

 datawc_x1 
    

 _ get _  = _getdatawc_x1(self) 
    

 _ set _  = _setdatawc_x1(self, value) 

 datawc_x2 
    

 _ get _  = _getdatawc_x2(self) 
    

 _ set _  = _setdatawc_x2(self, value) 

 datawc_y1 
    

 _ get _  = _getdatawc_y1(self) 
    

 _ set _  = _setdatawc_y1(self, value) 

 datawc_y2 
    

 _ get _  = _getdatawc_y2(self) 
    

 _ set _  = _setdatawc_y2(self, value) 

 line 
    

 _ get _  = _getline(self) 
    

 _ set _  = _setline(self, value) 

 linecolor 
    

 _ get _  = _getlinecolor(self) 
    

 _ set _  = _setlinecolor(self, value) 

 linewidth 
    

 _ get _  = _getlinewidth(self) 
    

 _ set _  = _setlinewidth(self, value) 

 marker 
    

 _ get _  = _getmarker(self) 
    

 _ set _  = _setmarker(self, value) 

 markercolor 
    

 _ get _  = _getmarkercolor(self) 
    

 _ set _  = _setmarkercolor(self, value) 

 markersize 
    

 _ get _  = _getmarkersize(self) 
    

 _ set _  = _setmarkersize(self, value) 

 name 
    

 _ get _  = _getname(self) 
    

 _ set _  = _setname(self, value) 

 projection 
    

 _ get _  = _getprojection(self) 
    

 _ set _  = _setprojection(self, value) 

 xaxisconvert 
    

 _ get _  = _getxaxisconvert(self) 
    

 _ set _  = _setxaxisconvert(self, value) 

 xmtics1 
    

 _ get _  = _getxmtics1(self) 
    

 _ set _  = _setxmtics1(self, value) 

 xmtics2 
    

 _ get _  = _getxmtics2(self) 
    

 _ set _  = _setxmtics2(self, value) 

 xticlabels1 
    

 _ get _  = _getxticlabels1(self) 
    

 _ set _  = _setxticlabels1(self, value) 

 xticlabels2 
    

 _ get _  = _getxticlabels2(self) 
    

 _ set _  = _setxticlabels2(self, value) 

 ymtics1 
    

 _ get _  = _getymtics1(self) 
    

 _ set _  = _setymtics1(self, value) 

 ymtics2 
    

 _ get _  = _getymtics2(self) 
    

 _ set _  = _setymtics2(self, value) 

 yticlabels1 
    

 _ get _  = _getyticlabels1(self) 
    

 _ set _  = _setyticlabels1(self, value) 

 yticlabels2 
    

 _ get _  = _getyticlabels2(self) 
    

 _ set _  = _setyticlabels2(self, value) 

* * *

Data and other attributes defined here:  

 __slots__  = ['setmember', 'parent', 'name', 'g_name', 'xaxisconvert', 'linecolor', 'line', 'linewidth', 'marker', 'markersize', 'markercolor', 'projection', 'xticlabels1', 'xticlabels2', 'yticlabels1', 'yticlabels2', 'xmtics1', 'xmtics2', 'ymtics1', 'ymtics2', ...] 

 g_name  = <member 'g_name' of 'GYx' objects>

 parent  = <member 'parent' of 'GYx' objects>

 setmember  = <member 'setmember' of 'GYx' objects>

  
 Functions 

` `

 getGYxmember  (self, member) 
     ` ###############################################################################   
#
#  
#&#160;Function:&#160;&#160;&#160;&#160;&#160;getGYxmember
#  
#
#  
#&#160;Description&#160;of&#160;Function:
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;Private&#160;function&#160;that&#160;retrieves&#160;the&#160;Yxvsx&#160;members&#160;from&#160;the&#160;C
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;structure&#160;and&#160;passes&#160;it&#160;back&#160;to&#160;Python.
#  
#
#  
#
#  
#&#160;Example&#160;of&#160;Use:
#  
#&#160;&#160;&#160;&#160;&#160;&#160;return_value&#160;=
#  
# [ getGYxmember ](/) (self,name)
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;where:&#160;self&#160;is&#160;the&#160;class&#160;(e.g., [ GYx ](/) )
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;name&#160;is&#160;the&#160;name&#160;of&#160;the&#160;member&#160;that&#160;is&#160;being&#160;found
#  
#
#  
##############################################################################
# `

 getmember  = getGYxmember(self, member) 
     ` ###############################################################################   
#
#  
#&#160;Function:&#160;&#160;&#160;&#160;&#160;getGYxmember
#  
#
#  
#&#160;Description&#160;of&#160;Function:
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;Private&#160;function&#160;that&#160;retrieves&#160;the&#160;Yxvsx&#160;members&#160;from&#160;the&#160;C
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;structure&#160;and&#160;passes&#160;it&#160;back&#160;to&#160;Python.
#  
#
#  
#
#  
#&#160;Example&#160;of&#160;Use:
#  
#&#160;&#160;&#160;&#160;&#160;&#160;return_value&#160;=
#  
# [ getGYxmember ](/) (self,name)
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;where:&#160;self&#160;is&#160;the&#160;class&#160;(e.g., [ GYx ](/) )
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;name&#160;is&#160;the&#160;name&#160;of&#160;the&#160;member&#160;that&#160;is&#160;being&#160;found
#  
#
#  
##############################################################################
# `

 renameGYx  (self, old_name, new_name) 
     ` ###############################################################################   
#
#  
#&#160;Function:&#160;&#160;&#160;&#160;&#160;renameGYx
#  
#
#  
#&#160;Description&#160;of&#160;Function:
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;Private&#160;function&#160;that&#160;renames&#160;the&#160;name&#160;of&#160;an&#160;existing&#160;Yxvsx
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;graphics&#160;method.
#  
#
#  
#
#  
#&#160;Example&#160;of&#160;Use:
#  
# [ renameGYx ](/) (old_name,&#160;new_name)
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;where:&#160;old_name&#160;is&#160;the&#160;current&#160;name&#160;of&#160;Yxvsx&#160;graphics&#160;method
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;new_name&#160;is&#160;the&#160;new&#160;name&#160;for&#160;the&#160;Yxvsx&#160;graphics&#160;method
#  
#
#  
##############################################################################
# `

 setGYxmember  (self, member, value) 
     ` ###############################################################################   
#
#  
#&#160;Function:&#160;&#160;&#160;&#160;&#160;setGYxmember
#  
#
#  
#&#160;Description&#160;of&#160;Function:
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;Private&#160;function&#160;to&#160;update&#160;the&#160;VCS&#160;canvas&#160;plot.&#160;If&#160;the&#160;canvas&#160;mode&#160;is
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;set&#160;to&#160;0,&#160;then&#160;this&#160;function&#160;does&#160;nothing.
#  
#
#  
#
#  
#&#160;Example&#160;of&#160;Use:
#  
# [ setGYxmember ](/) (self,name,value)
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;where:&#160;self&#160;is&#160;the&#160;class&#160;(e.g., [ GYx ](/) )
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;name&#160;is&#160;the&#160;name&#160;of&#160;the&#160;member&#160;that&#160;is&#160;being&#160;changed
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;value&#160;is&#160;the&#160;new&#160;value&#160;of&#160;the&#160;member&#160;(or&#160;attribute)
#  
#
#  
##############################################################################
# `

 setmember  = setGYxmember(self, member, value) 
     ` ###############################################################################   
#
#  
#&#160;Function:&#160;&#160;&#160;&#160;&#160;setGYxmember
#  
#
#  
#&#160;Description&#160;of&#160;Function:
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;Private&#160;function&#160;to&#160;update&#160;the&#160;VCS&#160;canvas&#160;plot.&#160;If&#160;the&#160;canvas&#160;mode&#160;is
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;set&#160;to&#160;0,&#160;then&#160;this&#160;function&#160;does&#160;nothing.
#  
#
#  
#
#  
#&#160;Example&#160;of&#160;Use:
#  
# [ setGYxmember ](/) (self,name,value)
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;where:&#160;self&#160;is&#160;the&#160;class&#160;(e.g., [ GYx ](/) )
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;name&#160;is&#160;the&#160;name&#160;of&#160;the&#160;member&#160;that&#160;is&#160;being&#160;changed
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;value&#160;is&#160;the&#160;new&#160;value&#160;of&#160;the&#160;member&#160;(or&#160;attribute)
#  
#
#  
##############################################################################
# `

  
 Data 

` `

 StringTypes  = (<type 'str'>, <type 'unicode'>) 

* * *

UCRL-WEB-213937 | [ Privacy & Legal Notice ](/disclaimer.html)

[ webmaster@pcmdi.llnl.gov ](/webmaster@pcmdi.llnl.gov)

[ ![Powered by Plone](media/plone_powered.gif) ](/)

