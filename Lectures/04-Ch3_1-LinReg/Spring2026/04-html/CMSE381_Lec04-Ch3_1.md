# Test Title Needed
                                                                                   
<div class="slide"> <div class="titlepage"><a 
 id="sl1"></a><p class="links"><a 
href="CMSE381_Lec04-Ch3_12.html#bookmark" target="tex4ht-menu" >toc</a></p>
<img 
src="CMSE381_Lec04-Ch3_10x.png" alt="picture"  />
<img 
src="CMSE381_Lec04-Ch3_12x.png" alt="picture"  /><div class="minipage">                                        <h1 class="title"><span 
class="cmss-12x-x-120">Ch</span>
                                       <span 
class="cmss-12x-x-120">3.1:</span>
                                      <span 
class="cmss-12x-x-120">Linear</span>
                                   <span 
class="cmss-12x-x-120">Regression</span></h1>
                                      Lecture
                                         4
                                         -
                                      CMSE
                                        381                                        </div>
                                         <div class="author"></div>
                                                                                   
                                      <div class="institute"><span 
class="cmss-8">Michigan</span>
                                       <span 
class="cmss-8">State</span>
                                      <span 
class="cmss-8">University</span><br />
                                         <span 
class="cmss-8">::</span><br />
                                        <span 
class="cmss-8">Dept</span>
                                         <span 
class="cmss-8">of</span>
                                    <span 
class="cmss-8">Computational</span>
                                     <span 
class="cmss-8">Mathematics,</span>
                                       <span 
class="cmss-8">Science</span>
                                         <span 
class="cmss-8">&amp;</span>
                                     <span 
class="cmss-8">Engineering</span></div>
                                                                                   
                                       <div class="date" >Wed
                                        Jan
                                        21,
                                       2026</div>
                                                                                   
</div>                                                                                   
                                                                                   
</div>
                                                                                   
                                                                                   
<div class="slide"> <span 
class="colorbox" id="colorbox4"> <span 
class="cmss-12x-x-120">Announcements</span>                                                                           </span>
<h2 class="frametitle"></h2>
<table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g>  <div class="minipage"><!--l. 101--><p class="noindent" >Last time: </p>
      <ul class="itemize1">
      <li class="itemize">
      <!--l. 101--><p class="noindent" >2.2
      Assessing
      Model
      Accuracy</p></li></ul>                                      </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>       <g visibility="hidden">
 </g> <div class="minipage">                                                       </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>
                                                                                   
                                                                                   
</div>
                                                                                   
                                                                                   
<div class="slide"> <span 
class="colorbox" id="colorbox5"> <span 
class="cmss-12x-x-120">Covered</span>
  <span 
class="cmss-12x-x-120">in</span>
  <span 
class="cmss-12x-x-120">this</span>
  <span 
class="cmss-12x-x-120">lecture</span>
                                                                                                 </span>
<h2 class="frametitle"></h2>
<table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g>  <div class="minipage">    <ul class="itemize1">
     <li class="itemize">
     <!--l. 120--><p class="noindent" >Least
      squares
      coefficient
      estimates
      for
      linear
      regression
      </li>
      <li class="itemize">
      <!--l. 120--><p class="noindent" >Residual
      sum
      of
      squares
      (RSS)</p></li></ul>                                     </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>            <g visibility="hidden">
 </g> <div class="minipage">                                                  </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>                                                                                 
                                                                                   
</div>
                                                                                   
                                                                                   
<a 
 id="x1-2r1"></a>
                                                                                   
                                                                                   
<a 
 id="Outline0.1"></a>  <div class="slide">  <!--l. 122--><p class="noindent" ><span 
class="cmss-12x-x-120">Section</span><span 
class="cmss-12x-x-120">&#x00A0;1</span>
<img 
src="CMSE381_Lec04-Ch3_13x.png" alt="picture"  />
<img 
src="CMSE381_Lec04-Ch3_15x.png" alt="picture"  /><div class="minipage">                                                      <a 
href="#Navigation8"><span 
class="cmss-12x-x-120">Simple</span>
                                          <span 
class="cmss-12x-x-120">Linear</span>
                                        <span 
class="cmss-12x-x-120">Regression</span></a>
                                                                                            </div>
                                                                                   
                                                                                   
</div>
                                                                                   
                                                                                   
<div class="slide"> <span 
class="colorbox" id="colorbox6"> <span 
class="cmss-12x-x-120">Setup</span>                                                                                        </span>
<h2 class="frametitle"></h2>
<table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g>  <div class="minipage">    <!--l. 141--><p class="noindent" ><g visibility="hidden">
 </g> Predict \(\beamer@setmathcolor Y\) on a single predictor variable \(\beamer@setmathcolor X\)
      \begin {equation*}  Y \approx \beta _0 + \beta _1 X  \end {equation*}
      <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
      <g visibility="hidden">
 &#8221;\(\beamer@setmathcolor \approx \)&#8221; .... &#8220;is approximately modeled
      as&#8221;</li></ul>
  <object data="CMSE381_Lec04-Ch3_1-20.svg" width="7.87814 " height="7.87814 " type="image/svg+xml"><p>SVG-Viewer needed.</p></object> <object data="CMSE381_Lec04-Ch3_1-21.svg" width="7.87814 " height="7.87814 " type="image/svg+xml"><p>SVG-Viewer needed.</p></object> </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>                                             </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>            <g visibility="hidden">
 </g> <div class="minipage">                                                  </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>                                                                                 
                                                                                   
</div> <div class="slide">
                                                                                   
                                                                                   
<span 
class="colorbox" id="colorbox7"><tspan font-family="cmss" font-size="12">Setup</tspan>                                                                               </span>
<h2 class="frametitle"></h2>
<table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <div class="minipage">    <!--l. 141--><p class="noindent" ><g visibility="hidden">
 </g> Predict \(\beamer@setmathcolor Y\) on a single predictor variable \(\beamer@setmathcolor X\)
    \begin {equation*}  Y \approx \beta _0 + \beta _1 X  \end {equation*}
    <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
    <g visibility="hidden">
 </g> &#8221;\(\beamer@setmathcolor \approx \)&#8221; .... &#8220;is approximately modeled
    as&#8221;</li></ul>
 <object data="CMSE381_Lec04-Ch3_1-22.svg" width="7.87814 " height="7.87814 " type="image/svg+xml"><p>SVG-Viewer needed.</p></object><object data="CMSE381_Lec04-Ch3_1-23.svg" width="7.87814 " height="7.87814 " type="image/svg+xml"><p>SVG-Viewer needed.</p></object> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>                                </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>            <g visibility="hidden">
 </g> <div class="minipage">                                                  </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>                                                                                   
                                                                                   
</div>
                                                                                   
                                                                                   
<div class="slide"> <span 
class="colorbox" id="colorbox8"> <tspan font-family="cmss" font-size="12">Example</tspan>
                                                                                                 </span>
<h2 class="frametitle"></h2>
<table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g>  <div class="minipage"><img 
src="../Figures//AdvertisingDataSet-Screenshot.png" alt="PIC"  
width="130" height="130"  />                                   </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>                <g visibility="hidden">
 </g> <div class="minipage">                                                   </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>
                                                                                   
                                                                                   
</div>
                                                                                   
                                                                                   
<div class="slide"> <span 
class="colorbox" id="colorbox9"> <tspan font-family="cmss" font-size="12">Least</tspan>
  <tspan font-family="cmss" font-size="12">squares</tspan>
  <tspan font-family="cmss" font-size="12">criterion:</tspan>
  <tspan font-family="cmss" font-size="12">Setup</tspan>
  <tspan font-family="cmss" font-size="9">How</tspan>
   <tspan font-family="cmss" font-size="9">do</tspan>
   <tspan font-family="cmss" font-size="9">we</tspan>
   <tspan font-family="cmss" font-size="9">estimate</tspan>
   <tspan font-family="cmss" font-size="9">the</tspan>
   <tspan font-family="cmss" font-size="9">coefficients?</tspan>                                                                                                                                  </span>
<h2 class="frametitle"></h2> <table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g>  <div class="minipage">                                                           </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>              <g visibility="hidden">
 </g> <div class="minipage"><img 
src="../Figures//Fig3-1.png" alt="PIC"  
width="173" height="173"  />                                              </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>
                                                                                   
                                                                                   
</div>
                                                                                   
                                                                                   
<div class="slide"> <span 
class="colorbox" id="colorbox10"> <tspan font-family="cmss" font-size="12">Least</tspan>
  <tspan font-family="cmss" font-size="12">squares</tspan>
  <tspan font-family="cmss" font-size="12">criterion:</tspan>
  <tspan font-family="cmss" font-size="12">RSS</tspan>                                                                                          </span>
<h2 class="frametitle"></h2>
<table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g>  <div class="minipage"><img 
src="../Figures//Fig3-2.png" alt="PIC"  
width="260" height="260"  /> \begin {equation*}  \textrm {sales} \approx \beta _0 + \beta _1 \textrm {TV}  \end {equation*}                                                                   </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>      <g visibility="hidden">
 </g> <div class="minipage">Residual sum of squares RSS is \begin {align*}  RSS &amp;= e_1^2 + \cdots + e_n^2\\ &amp;= \sum _i (y_i - \hat \beta _0 - \hat \beta _1 x_i)^2  \end {align*}
                                          </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>
<table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g>       <div class="minipage"><div class="block"><g visibility="hidden">
 </g> 
<img 
src="CMSE381_Lec04-Ch3_16x.png" alt="picture"  /><div class="minipage"><tspan font-family="cmss" font-size="12">Least</tspan>
<tspan font-family="cmss" font-size="12">squares</tspan>
<tspan font-family="cmss" font-size="12">criterion</tspan>                                             </div>
<img 
src="CMSE381_Lec04-Ch3_17x.png" alt="picture"  />
<img 
src="CMSE381_Lec04-Ch3_19x.png" alt="picture"  /><div class="minipage">Find
\(\beamer@setmathcolor \beta _0\)
and
\(\beamer@setmathcolor \beta _1\)
that
minimize
the
RSS.                                                     </div>
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</div>                                                                                </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>                                                                                 
                                                                                   
</div>
                                                                                   
                                                                                   
<div class="slide"> <span 
class="colorbox" id="colorbox11"> <tspan font-family="cmss" font-size="12">Least</tspan>
  <tspan font-family="cmss" font-size="12">squares</tspan>
  <tspan font-family="cmss" font-size="12">coefficient</tspan>
  <tspan font-family="cmss" font-size="12">estimates</tspan>                                                                                   </span>
<h2 class="frametitle"></h2>
<table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g>  <div class="minipage">
<!--l. 250--><p class="noindent" >\begin {equation*}  \min _{\beta _0,\beta _1} \sum _i (y_i - \hat \beta _0 - \hat \beta _1 x_i)^2  \end {equation*}

</p><!--l. 250--><p class="noindent" >\begin {align*}  \frac {\partial RSS}{\partial \hat \beta _0} &amp; = -2 \sum _i (y_i - \hat {\beta }_0 - \hat {\beta }_1x_i) = 0 \\ \frac {\partial RSS}{\partial \hat \beta _1} &amp; = -2 \sum _i x_i(y_i - \hat \beta _0 - \hat \beta _1x_i) = 0  \end {align*}                                       </p></div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>         <g visibility="hidden">
 </g> <div class="minipage">
<!--l. 250--><p class="noindent" >\begin {align*}  \hat \beta _1 &amp;= \frac {\sum _{i=1}^n(x_i-\overline x) (y_i - \overline y)} {\sum _{i=1}^n (x_i - \overline x)^2}\\ \hat \beta _0 &amp; = \overline y - \hat \beta _1 \overline x  \end {align*}                                       </p></div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>
                                                                                   
                                                                                   
</div>
                                                                                   
                                                                                   
<div class="slide"> <span 
class="colorbox" id="colorbox12"> <tspan font-family="cmss" font-size="12">Coding</tspan>
  <tspan font-family="cmss" font-size="12">group</tspan>
  <tspan font-family="cmss" font-size="12">work</tspan>                                                                                         </span>
<h2 class="frametitle"></h2><table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g>  <div class="minipage">                                          </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>      <g visibility="hidden">
 </g> <div class="minipage">                                           </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>
                                                                                   
                                                                                   
</div>
                                                                                   
                                                                                   
<div class="slide"> <span 
class="colorbox" id="colorbox13"> <tspan font-family="cmss" font-size="12">Next</tspan>
  <tspan font-family="cmss" font-size="12">time</tspan>                                                                                          </span>
<h2 class="frametitle"></h2>
<table class="columns"><tr><g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g>  <div class="minipage">Next time: 
      <ul class="itemize1">
      <li class="itemize">
      <!--l. 342--><p class="noindent" >More
      on
      simple
      linear
      regression!
      </li>
      <li class="itemize">
      <!--l. 342--><p class="noindent" >Evaluation
      of
      model
      etc.</p></li></ul>
<!--l. 342--><p class="noindent" ><img 
src="../Figures//Schedule-S26-Lecs1_to_10.png" alt="PIC"  
width="173" height="173"  />                                              </p></div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g>            <g visibility="hidden">
 </g> <div class="minipage"><tspan font-family="cmssbx" font-size="10">Announcements </tspan>
     <ul class="itemize1">
     <li class="itemize">
     <!--l. 342--><p class="noindent" >Homework 1 </p>
            <ul class="itemize2">
            <li class="itemize">
            <!--l. 342--><p class="noindent" ><tspan font-family="cmss" font-size="10">Due</tspan>
             <tspan font-family="cmss" font-size="10">Sun,</tspan>
             <tspan font-family="cmss" font-size="10">Jan</tspan>
             <tspan font-family="cmss" font-size="10">25</tspan></p></li></ul>
       </li></ul>                                                </div><g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
<g visibility="hidden">
 </g> <g visibility="hidden">
 </g> <g visibility="hidden">
 </g> 
</tr></table>                                                                                 
                                                                                   
</div>
                                                                                   
                                                                                   
                                                                                                                                


