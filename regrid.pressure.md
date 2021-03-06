---
layout: default
title:
---

 [ Skip to content. ](/cdat/source/api-reference/regrid.pressure.html) | [ Skip
to navigation ](/cdat/source/api-reference/regrid.pressure.html)

Search Site

[ Advanced Search&#8230; ](/search_form)

#  [ PCMDI Software Portal ](/)

#####  Sections

  * [ Home ](/)

#####  Personal tools

  * [ Log in ](/login_form)

You are here:  [ Home ](/) -> [ CDAT ](/cdat) -> [ Source Code ](/cdat/source)
-> [ API Reference ](/cdat/source/api-reference) -> Python: module
regrid.pressure

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

        * [ Python: module regrid.pressure ](/cdat/source/api-reference/regrid.pressure.html)

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

  * [ ![Send this page to somebody](media/mail_icon.gif) ](/cdat/source/api-reference/regrid.pressure.html/sendto_form)
  * [ ![Print this page](media/print_icon.gif) ](/this.print\(\))

#  Python: module regrid.pressure

  
  
 [ regrid  ](/regrid.html) .pressure 
[ index ](/)  

  
 Modules 

` `

[ MA ](/MA.html)  
[ Numeric ](/Numeric.html)  

[ regrid._regrid ](/regrid._regrid.html)  
[ copy ](/copy.html)  

[ string ](/string.html)  

  
 Classes 

` `

[ PressureRegridder ](/regrid.pressure.html)

  
class  PressureRegridder 

` `

` #---------------------------------------------------------------------------
--------------------  
#  
#&#160;&#160;&#160;&#160;PURPOSE:&#160;To&#160;perform&#160;all&#160;the&#160;tasks&#160;required&#160;to&#160;regrid&#160;the&#160;input&#160;data&#160;into
the&#160;ouput&#160;data&#160;along  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;the&#160;pressure&#160;dimension&#160;only.  
#  
#&#160;&#160;&#160;&#160;PROCEDURE:&#160;Step&#160;One:  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;Make&#160;an&#160;instance&#160;of&#160;class [ PressureRegridder ](/) passing
it&#160;input&#160;and&#160;output&#160;grid&#160;information  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;Step&#160;Two:  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;Pass&#160;the&#160;input&#160;data&#160;with&#160;some&#160;descriptive&#160;parameters&#160;and
get&#160;the&#160;output&#160;data  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;in&#160;return  
#  
#-----------------------------------------------------------------------------
-------------------  
`

Methods defined here:  

 __call__  (self, ar, missing  =None  , order  =None  , method  ='log'  ) 
     ` Call&#160;the&#160;pressure&#160;regridder&#160;function.   
ar&#160;is&#160;the&#160;input&#160;array,&#160;a&#160;variable,&#160;masked&#160;array,&#160;or&#160;Numeric&#160;array.  
missing&#160;is&#160;the&#160;missing&#160;data&#160;value,&#160;if&#160;any.&#160;It&#160;defaults&#160;to&#160;the&#160;missing/fill
value  
defined&#160;for&#160;the&#160;input&#160;array,&#160;if&#160;any.  
order&#160;is&#160;of&#160;the&#160;form&#160;"tzyx",&#160;"tyx",&#160;etc.  
method&#160;is&#160;either&#160;'log'&#160;to&#160;interpolate&#160;in&#160;the&#160;log&#160;of&#160;pressure,&#160;or&#160;'linear'&#160;for
linear&#160;interpolation. `

 __init__  (self, axisIn, axisOut) 
     ` #-----------------------------------------------------------------------------------------------   
#  
#&#160;&#160;&#160;&#160;PURPOSE:&#160;To&#160;make&#160;an&#160;instance&#160;which&#160;entails&#160;setting&#160;up&#160;the&#160;input&#160;and
output&#160;grids  
#  
#&#160;&#160;&#160;&#160;DEFINITION:  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;def [ __init__ ](/) (self,&#160;levIn,&#160;levOut):  
#  
#&#160;&#160;&#160;&#160;PROCEDURE:  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;The&#160;user&#160;must&#160;assemble&#160;two&#160;pieces&#160;of&#160;information:  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;axisIn&#160;-&#160;&#160;the&#160;input&#160;level&#160;axis  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;axisOut&#160;-&#160;&#160;the&#160;output&#160;level&#160;axis  
#  
#&#160;&#160;&#160;&#160;USAGE:  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;To&#160;&#160;make&#160;an&#160;instance&#160;preparing&#160;for&#160;a&#160;regrid&#160;along&#160;the&#160;level
dimension&#160;pnly,&#160;type  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;r&#160;= [ PressureRegridder ](/) (levIn,&#160;levOut)  
#  
#-----------------------------------------------------------------------------
------------------- `

 rgrd  (self, dataIn, missingValueIn, missingMatch, logYes  ='yes'  , positionIn  =None  , missingValueOut  =None  ) 
     ` #---------------------------------------------------------------------------------   
#  
#&#160;&#160;&#160;&#160;PURPOSE:&#160;To&#160;perform&#160;all&#160;the&#160;tasks&#160;required&#160;to&#160;regrid&#160;the&#160;input&#160;data,
dataIn,&#160;into&#160;the&#160;ouput&#160;data,  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;dataout&#160;along&#160;the&#160;level&#160;dimension&#160;only.  
#  
#&#160;&#160;&#160;&#160;DEFINITION:  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;def [ rgrd ](/) (self,&#160;dataIn,&#160;missingValueIn,&#160;missingMatch,
positionIn&#160;=&#160;None,&#160;missingValueOut&#160;=&#160;None):  
#  
#  
#&#160;&#160;&#160;&#160;PASSED&#160;:&#160;&#160;dataIn&#160;\--&#160;data&#160;to&#160;regrid  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;missingValueIn&#160;\--&#160;the&#160;missing&#160;data&#160;value&#160;to&#160;use&#160;in&#160;setting
missing&#160;in&#160;the&#160;mask.&#160;It&#160;is&#160;required  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;and&#160;there&#160;are&#160;two&#160;choices:  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;None&#160;\--&#160;there&#160;is&#160;no&#160;missing&#160;data  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;A&#160;number&#160;\--&#160;the&#160;value&#160;to&#160;use&#160;in&#160;the
search&#160;for&#160;possible&#160;missing&#160;data.  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;The&#160;presence&#160;of&#160;missing&#160;data&#160;at&#160;a&#160;grid&#160;point
leads&#160;to&#160;recording&#160;0.0&#160;in&#160;the&#160;mask.  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;missingMatch&#160;\--&#160;the&#160;comparison&#160;scheme&#160;used&#160;in&#160;searching&#160;for
missing&#160;data&#160;in&#160;dataIn&#160;using&#160;the&#160;value&#160;passed  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;in&#160;as&#160;missingValueIn.&#160;The&#160;choices&#160;are:  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;None&#160;\--&#160;used&#160;if&#160;None&#160;is&#160;the&#160;entry&#160;for
missingValueIn  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;exact&#160;\--&#160;used&#160;if&#160;missingValue&#160;is&#160;the&#160;exact
value&#160;from&#160;the&#160;file  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;greater&#160;\--&#160;the&#160;missing&#160;data&#160;value&#160;is&#160;equal
to&#160;or&#160;greater&#160;than&#160;missingValueIn  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;less&#160;\--&#160;the&#160;missing&#160;data&#160;value&#160;is&#160;equal&#160;to
or&#160;less&#160;than&#160;missingValueIn  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;logYes&#160;\--&#160;choose&#160;the&#160;level&#160;regrid&#160;as&#160;linear&#160;in&#160;log&#160;of&#160;level&#160;or
linear&#160;in&#160;level.&#160;Set&#160;to  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;'yes'&#160;for&#160;log.&#160;Anything&#160;else&#160;is&#160;linear&#160;in&#160;level.  
#  
#  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;positionIn&#160;\--&#160;a&#160;tuple&#160;with&#160;the&#160;numerical&#160;position&#160;of&#160;the
dimensions  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;in&#160;C&#160;or&#160;Python&#160;order&#160;specified&#160;in&#160;the&#160;sequence
longitude,  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;latitude,&#160;level&#160;and&#160;time.&#160;Longitude,&#160;latitude&#160;and
level&#160;are  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;required.&#160;If&#160;time&#160;is&#160;missing&#160;submit&#160;None&#160;in&#160;its
slot&#160;in&#160;the  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;tuple.&#160;Notice&#160;that&#160;the&#160;length&#160;of&#160;the&#160;tuple&#160;is
always&#160;four.  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;Explicitly,&#160;in&#160;terms&#160;of&#160;the&#160;shape&#160;of&#160;dataIn&#160;as
returned&#160;by&#160;Python's&#160;shape&#160;function  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;positionIn[0]&#160;contains&#160;the&#160;position&#160;of
longitude&#160;in&#160;dataIn  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;positionIn[1]&#160;contains&#160;the&#160;position&#160;of
latitude&#160;in&#160;dataIn  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;positionIn[2]&#160;contains&#160;the&#160;position&#160;of&#160;level
in&#160;dataIn&#160;or&#160;None  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;positionIn[3]&#160;contains&#160;the&#160;position&#160;of&#160;time
in&#160;dataIn&#160;or&#160;None  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;As&#160;&#160;examples:  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;If&#160;the&#160;C&#160;order&#160;shape&#160;of&#160;4D&#160;data&#160;is  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;(number&#160;of&#160;longitudes,&#160;number&#160;of&#160;times,
number&#160;of&#160;levels,&#160;number&#160;of&#160;latitudes)  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;submit  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;(0,&#160;3,&#160;2,&#160;1)  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;If&#160;the&#160;C&#160;order&#160;shape&#160;of&#160;3D&#160;data&#160;is  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;(number&#160;of&#160;longitudes,&#160;number&#160;of&#160;times,
number&#160;oflatitudes)  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;submit  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;(0,&#160;2,&#160;1,&#160;None)  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;Send&#160;in&#160;None&#160;if&#160;the&#160;shape&#160;is&#160;a&#160;subset&#160;of&#160;(time,
level,  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;latitude,&#160;longitude)&#160;which&#160;is&#160;evaluated&#160;as
follows:  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;3D&#160;\--&#160;code&#160;assumes&#160;(2,1,0,None)  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;4D&#160;\--&#160;code&#160;assumes&#160;(3,2,1,0)  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;missingValueOut&#160;\--&#160;the&#160;value&#160;for&#160;the&#160;missing&#160;data&#160;used&#160;in
writing&#160;the&#160;output&#160;data.&#160;If&#160;left&#160;at&#160;the  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;default&#160;entry,&#160;None,&#160;the&#160;code&#160;uses
missingValueIn&#160;if&#160;present&#160;or&#160;as&#160;a&#160;last&#160;resort  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;1.0e20  
#  
#  
#&#160;&#160;&#160;&#160;RETURNED&#160;:&#160;dataOut&#160;\--&#160;the&#160;regridded&#160;data  
#  
#  
#&#160;&#160;&#160;&#160;USAGE:  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;Example&#160;1.&#160;&#160;To&#160;regrid&#160;dataIn&#160;into&#160;dataOut&#160;using&#160;all&#160;the&#160;defaults
where&#160;None,&#160;None&#160;signifies&#160;no  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;missing&#160;data.  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;dataOut&#160;=&#160;x. [ rgrd ](/) (dataIn,&#160;None,&#160;None)  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;Example&#160;2.&#160;&#160;To&#160;regrid&#160;dataIn&#160;into&#160;dataOut&#160;using&#160;1.0e20&#160;and&#160;greater
as&#160;the&#160;missing&#160;data  
#  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;dataOut&#160;=&#160;x. [ rgrd ](/) (dataIn,&#160;1.e20,&#160;'greater')  
#  
#-----------------------------------------------------------------------------
---------------------------------------- `

  
 Functions 

` `

 checkorder  (positionIn) 
     ` #-----------------------------------------------------------------------------------------   
#  
#&#160;&#160;&#160;&#160;&#160;purpose:&#160;construct&#160;the&#160;tuples&#160;for&#160;transposing&#160;the&#160;data&#160;to&#160;standard
dimension&#160;order&#160;and&#160;the  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;inverse&#160;for&#160;transposing&#160;it&#160;back&#160;to&#160;the&#160;original&#160;dimension&#160;order  
#  
#&#160;&#160;&#160;&#160;&#160;usage:&#160;&#160;&#160;newOrder,&#160;inverseOrder&#160;= [ checkorder ](/) (positionIn)  
#  
#&#160;&#160;&#160;&#160;&#160;passed:&#160;&#160;positionIn&#160;\--&#160;array&#160;with&#160;location&#160;of&#160;longitude,&#160;latitude.
level&#160;and&#160;time&#160;respectively  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;in&#160;the&#160;sense&#160;of&#160;the&#160;python&#160;shape&#160;of&#160;the&#160;data  
#  
#&#160;&#160;&#160;&#160;&#160;returned:&#160;newOrder&#160;\--&#160;tuple&#160;to&#160;transpose&#160;data&#160;to&#160;the&#160;order&#160;(t,z,y,x)  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;inverseOrder&#160;\--&#160;tuple&#160;to&#160;transpose&#160;data&#160;to&#160;back&#160;to&#160;the
original&#160;order  
#  
#-----------------------------------------------------------------------------
----------------- `

 sendmsg  (msg, value1  =None  , value2  =None  ) 
     ` #---------------------------------------------------------------------------------   
#  
#&#160;&#160;&#160;&#160;purpose:&#160;send&#160;the&#160;same&#160;message&#160;to&#160;the&#160;screen  
#  
#&#160;&#160;&#160;&#160;passed&#160;:&#160;&#160;msg&#160;-&#160;the&#160;string  
#&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;value&#160;-&#160;the&#160;number&#160;associated&#160;with&#160;the&#160;string  
#  
#&#160;&#160;&#160;&#160;returned:&#160;return  
#  
#-----------------------------------------------------------------------------
---- `

* * *

UCRL-WEB-213937 | [ Privacy & Legal Notice ](/disclaimer.html)

[ webmaster@pcmdi.llnl.gov ](/webmaster@pcmdi.llnl.gov)

[ ![Powered by Plone](media/plone_powered.gif) ](/)

