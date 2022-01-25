<template>
  <div class="hello">
    <div style="text-align: center; margin: auto; height: 200px; padding: 35px; max-width:300px ">

      <svg id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
           x="0px" y="0px"
           viewBox="0 0 50 50" style="enable-background:new 0 0 50 50;" xml:space="preserve"
           preserveAspectRatio="xMidYMid meet" width="20" height="20">
        <g>
			<circle className="circle" cx="50" cy="49.9999657" r="47.5"/>
          <circle className="circle-dash" cx="50" cy="49.9999657" r="47.5"/>
          <polyline className="check"
                    points="28.6469955,52.0561066 42.2152748,65.6243896 71.3530045,36.4866562 	"/>
          <polyline className="check-dash"
                    points="28.6469955,52.0561066 42.2152748,65.6243896 71.3530045,36.4866562 	"/>
		</g>
		</svg>


    </div>
    <div style="text-align: center; margin: auto; padding: 25px;">

      <a href="#" className="myButton" type=button value="Refresh" onClick="history.go()">Refresh</a>
    </div>

  </div>
</template>

<style>

.circle{fill:none;stroke:#1E4164;stroke-width:3;stroke-linecap:round;stroke-miterlimit:10;}
.circle-dash{fill:none;stroke:#1E4164;stroke-width:3;stroke-linecap:round;stroke-miterlimit:10;}
.check{fill:none;stroke:#1E4164;stroke-width:3;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:10;}
.check-dash{fill:none;stroke:#1E4164;stroke-width:3;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:10;}

.check {
  stroke-dasharray: 60 100;
  animation: check 1.2s cubic-bezier(0.5, 0, 0.6, 1) forwards 0.15s;
  -webkit-animation: check 1.2s cubic-bezier(0.5, 0, 0.6, 1) forwards 0.15s;
  -moz-animation: check 1.2s cubic-bezier(0.5, 0, 0.6, 1) forwards 0.15s;
  -o-animation: check 1.2s cubic-bezier(0.5, 0, 0.6, 1) forwards 0.15s;
  opacity: 0;
}

@-webkit-keyframes check {
  from {stroke-dashoffset: 60;
    opacity: 1;}

  to {stroke-dashoffset: 00;
    opacity: 1;}
}

@-moz-keyframes check {
  from {stroke-dashoffset: 60;
    opacity: 1;}

  to {stroke-dashoffset: 00;
    opacity: 1;}
}

@keyframes check {
  from {stroke-dashoffset: 60;
    opacity: 1;}

  to {stroke-dashoffset: 00;
    opacity: 1;}
}

.check-dash {
  stroke-dasharray: 10 100;
  animation: check-dash 1.2s cubic-bezier(0.5, 0, 0.6, 1) forwards;
  -webkit-animation: check-dash 1.2s cubic-bezier(0.5, 0, 0.6, 1) forwards;
  -moz-animation: check-dash 1.2s cubic-bezier(0.5, 0, 0.6, 1) forwards;
  -o-animation: check-dash 1.2s cubic-bezier(0.5, 0, 0.6, 1) forwards;
}

@-webkit-keyframes check-dash {
  from {stroke-dashoffset: 120;}
  to {stroke-dashoffset: 45;}
}

@-moz-keyframes check-dash {
  from {stroke-dashoffset: 120;}
  to {stroke-dashoffset: 45;}
}

@keyframes check-dash {
  from {stroke-dashoffset: 120;}
  to {stroke-dashoffset: 45;}
}

.circle {
  stroke-dasharray: 300 300;
  animation: circle 1.5s cubic-bezier(0.5, 0, 0.5, 1) forwards 0.15s;
  -webkit-animation: circle 1.5s cubic-bezier(0.5, 0, 0.5, 1) forwards 0.15s;
  -moz-animation: circle 1.5s cubic-bezier(0.5, 0, 0.5, 1) forwards 0.15s;
  -o-animation: circle 1.5s cubic-bezier(0.5, 0, 0.5, 1) forwards 0.15s;
  opacity: 0;
}

@-webkit-keyframes circle {
  from {stroke-dashoffset:300;
    opacity: 1;}
  to {stroke-dashoffset:0;
    opacity: 1;}
}

@-moz-keyframes circle {
  from {stroke-dashoffset:300;
    opacity: 1;}
  to {stroke-dashoffset:0;
    opacity: 1;}
}

@keyframes circle {
  from {stroke-dashoffset:300;
    opacity: 1;}
  to {stroke-dashoffset:0;
    opacity: 1;}
}

.circle-dash {
  stroke-dasharray: 10 300;
  animation: circledash 1.5s cubic-bezier(0.5, 0, 0.5, 1) forwards 0.05s;
  -webkit-animation: circledash 1.5s cubic-bezier(0.5, 0, 0.5, 1) forwards 0.05s;
  -moz-animation: circledash 1.5s cubic-bezier(0.5, 0, 0.5, 1) forwards 0.05s;
  -o-animation: circledash 1.5s cubic-bezier(0.5, 0, 0.5, 1) forwards 0.05s;
  opacity: 0;
}

@-webkit-keyframes circledash {
  from {stroke-dashoffset:320;
    opacity: 1;}
  to {stroke-dashoffset: 20;
    opacity: 1;}
}

@-moz-keyframes circledash {
  from {stroke-dashoffset:320;
    opacity: 1;}
  to {stroke-dashoffset: 20;
    opacity: 1;}
}

@keyframes circledash {
  from {stroke-dashoffset:320;
    opacity: 1;}
  to {stroke-dashoffset: 20;
    opacity: 1;}
}


</style>
