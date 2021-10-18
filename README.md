## Here is what I'm Working On!

Here are some ideas to get you stated:

<style>

:root {
  --offset: 1rem;
}

*, *:before, *:after {
  box-sizing: border-box;
}

@media (min-width: 40em) {
  body {
    display: grid;
    grid-template-columns: 1fr 3fr;
  }
}
img,
a {
  display: block;
  height: 100%;
}

img {
  max-width: 100%;
  width: 100%;
  object-fit: cover;
}

.grid {
  display: grid;
  grid-gap: 0;
  overflow: hidden;
  list-style: none;
  margin: 0;
  padding: 0;
  height: 100vh;
}
.grid li {
  position: relative;
}
.grid li:hover ~ li:last-child:after,
.grid li:last-child:hover:after,
.grid li:hover ~ li:last-child:before,
.grid li:last-child:hover:before {
  opacity: 1;
  transition: 1s ease;
}
.grid li:last-child:after,
.grid li:last-child:before {
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  pointer-events: none;
  clip-path: polygon(var(--offset) var(--offset), var(--offset) calc(100% - var(--offset)), calc(100% - var(--offset)) calc(100% - var(--offset)), calc(100% - var(--offset)) var(--offset));
  -webkit-clip-path: polygon(var(--offset) var(--offset), var(--offset) calc(100% - var(--offset)), calc(100% - var(--offset)) calc(100% - var(--offset)), calc(100% - var(--offset)) var(--offset));
  opacity: 0;
  transition: opacity 1s, transform 1s 1s, background 1s;
}
.grid li:last-child:after {
  mix-blend-mode: multiply;
  background: #aaafc3;
}
.grid li:last-child:before {
  backdrop-filter: grayscale(100%) blur(2px);
  -webkit-backdrop-filter: grayscale(100%) blur(2px);
}
.grid li:nth-child(1):hover ~ li:last-child:after {
  background: #1A237E;
}
.grid li:nth-child(2):hover ~ li:last-child:after {
  background: #b5a1b7;
}
.grid li:nth-child(3):hover ~ li:last-child:after {
  background: #aaafc3;
}
.grid li:nth-child(4):hover ~ li:last-child:after {
  background: #daa384;
}
.grid li:nth-child(5):hover ~ li:last-child:after {
  background: #A5D6A7;
}
.grid li:nth-child(6):hover ~ li:last-child:after {
  background: #6c4331;
}
.grid li:nth-child(7):hover ~ li:last-child:after {
  background: #555;
}
.grid li:last-child:hover:after {
  background: #a88504;
}

.grid {
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(3, 33.3333333333%);
}
.grid li:last-child:after,
.grid li:last-child:before {
  left: 100%;
  transform: translate3d(-100%, -100%, 0);
}
.grid li:nth-child(1):hover ~ li:last-child:after,
.grid li:nth-child(1):hover ~ li:last-child:before {
  transform: translate3d(-200%, -200%, 0);
}
.grid li:nth-child(2):hover ~ li:last-child:after,
.grid li:nth-child(2):hover ~ li:last-child:before {
  transform: translate3d(-100%, -200%, 0);
}
.grid li:nth-child(3):hover ~ li:last-child:after,
.grid li:nth-child(3):hover ~ li:last-child:before {
  transform: translate3d(0%, -200%, 0);
}
.grid li:nth-child(4):hover ~ li:last-child:after,
.grid li:nth-child(4):hover ~ li:last-child:before {
  transform: translate3d(-200%, -100%, 0);
}
.grid li:nth-child(5):hover ~ li:last-child:after,
.grid li:nth-child(5):hover ~ li:last-child:before {
  transform: translate3d(-100%, -100%, 0);
}
.grid li:nth-child(6):hover ~ li:last-child:after,
.grid li:nth-child(6):hover ~ li:last-child:before {
  transform: translate3d(0%, -100%, 0);
}
.grid li:nth-child(7):hover ~ li:last-child:after,
.grid li:nth-child(7):hover ~ li:last-child:before {
  transform: translate3d(-200%, 0%, 0);
}
.grid li:last-child:hover:after,
.grid li:last-child:hover:before {
  transform: translate3d(-100%, 0%, 0);
}

@media (max-width: 60em) {
  .grid {
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(4, 25%);
  }
  .grid li:last-child:after,
.grid li:last-child:before {
    left: 0%;
    transform: translate3d(-50%, -150%, 0);
  }
  .grid li:nth-child(1):hover ~ li:last-child:after,
.grid li:nth-child(1):hover ~ li:last-child:before {
    transform: translate3d(-100%, -300%, 0);
  }
  .grid li:nth-child(2):hover ~ li:last-child:after,
.grid li:nth-child(2):hover ~ li:last-child:before {
    transform: translate3d(0%, -300%, 0);
  }
  .grid li:nth-child(3):hover ~ li:last-child:after,
.grid li:nth-child(3):hover ~ li:last-child:before {
    transform: translate3d(-100%, -200%, 0);
  }
  .grid li:nth-child(4):hover ~ li:last-child:after,
.grid li:nth-child(4):hover ~ li:last-child:before {
    transform: translate3d(0%, -200%, 0);
  }
  .grid li:nth-child(5):hover ~ li:last-child:after,
.grid li:nth-child(5):hover ~ li:last-child:before {
    transform: translate3d(-100%, -100%, 0);
  }
  .grid li:nth-child(6):hover ~ li:last-child:after,
.grid li:nth-child(6):hover ~ li:last-child:before {
    transform: translate3d(0%, -100%, 0);
  }
  .grid li:nth-child(7):hover ~ li:last-child:after,
.grid li:nth-child(7):hover ~ li:last-child:before {
    transform: translate3d(-100%, 0%, 0);
  }
  .grid li:last-child:hover:after,
.grid li:last-child:hover:before {
    transform: translate3d(0%, 0%, 0);
  }

  :root {
    --offset: 0;
  }
}
.description {
  font-family: "Unica One", sans-serif;
  font-size: 1.25rem;
  position: absolute;
  display: block;
  right: 2rem;
  left: 2rem;
  text-align: center;
  top: 50%;
  width: 60px;
  margin: auto;
  color: white;
  z-index: 100;
  opacity: 0;
  transform: translate3d(0, -50%, 0);
  transition: 0.3s 0s;
}

li:hover .description {
  opacity: 1;
  transition: 0.6s 0.3s;
}

header {
  padding: 1rem;
  font-family: "Courier New", monospace, serif;
  font-size: 1em;
}

h1 {
  margin-top: 0;
}

p {
  line-height: 1.4;
}
</style>
<header>
  <h1>WE CREATE THE TREND</h1>
 
</header>
  <ul class="grid">
    <li>
      <a href="#">
        <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/74321/wvfrkayr0mg-christelle-bourgeois-776x1063.jpg" alt="">
        <span class="description">Dearest Diary</span>
      </a>
    </li>
    <li>
      <a href="#">
        <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/74321/fbanijhrol4-annie-spratt-776x951.jpg" alt="">
      </a>
      <span class="description">Window Sill?</span>
    </li>
    <li>
      <a href="#">
        <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/74321/2rm8p0rkxiw-marius-masalar-776x582.jpg" alt="">
        <span class="description">Listen To Me</span>
      </a>      
    </li>
    <li>
     <a href="#">
        <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/74321/71nlan-2ya-andrew-neel-2-776x620.jpg" alt="">
        <span class="description">Travel Often</span>
      </a>
    </li>
    <li>
      <a href="#">
        <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/74321/hdyo6rr3kqk-scott-webb-1172x780.jpg" alt="">
        <span class="description">Another Plant?</span>
      </a>
    </li>
    <li>
      <a href="#">
        <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/74321/fvazbu6zae-andrew-neel-776x517.jpg" alt="">
        <span class="description">On the Wave</span>
      </a>
    </li>
    <li>
      <a href="#">
        <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/74321/typewriter-1-776x968.jpg" alt="">
        <span class="description">Great Gatsby</span>
      </a>
    </li>    
    <li>
      <a href="#">
        <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/74321/xohlruw4k8-christelle-bourgeois-776x758.jpg" alt="">
        <span class="description">In the Sun</span>
      </a>
    </li>
</ul>


:computer: I'm currently working on ... Web Designe & Web Development <br>
:pencil2: I'm currently working on ... Freelancing<br>
:mag_right: I'm looking for help with .... AWS<br>
:arrow_forward: Ask me about ... Anything<br>
:paperclip: How toereach me! ... Gainsboro Infotech (https://gainsboroinfotech.com/)<br>
:busts_in_silhouette: Pronouns .. He/His<br>
:ok: Fun fact .. I am half Finish<br>
