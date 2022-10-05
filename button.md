 <a href="#projects" class="heading__link">
          <div class="heading-cta"> <!-- Appears as the "View My Work" button -->
            View my work

            <svg
              class="heading__arrow"
              version="1.1"
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
            >
              <title>arrow-right</title>
              <path
                d="M11.293 5.707l5.293 5.293h-11.586c-0.552 0-1 0.448-1 1s0.448 1 1 1h11.586l-5.293 5.293c-0.391 0.391-0.391 1.024 0 1.414s1.024 0.391 1.414 0l7-7c0.092-0.092 0.166-0.202 0.217-0.324 0.101-0.245 0.101-0.521 0-0.766-0.049-0.118-0.121-0.228-0.217-0.324l-7-7c-0.391-0.391-1.024-0.391-1.414 0s-0.391 1.024 0 1.414z"
              ></path>
            </svg> <!-- class="heading_arrow" -->
          </div> <!-- class="heading-cta" -->
        </a> <!-- class="heading__link" -->
      </div> <!-- class="heading" -->
    </div> <!-- class="hero" -->
    


    CSS

    .heading-cta{
    position:relative;
    display:flex;
    align-items:center;
    margin-top:2.4rem;
    padding:0.8rem 3rem;
    width:27.5rem;
    height:4.8rem;
    background-color:rgba(0, 0, 0, 0.6);
    border:1px solid #64ffda;
    border-radius:2px;
    color:#64ffda;
    font-size:2.41rem;
    font-weight:100;
    cursor:pointer;
    animation:moveInBottom 0.7s 1.2s;
    animation-fill-mode:backwards;
    animation-timing-function:cubic-bezier(0.21, 1.11, 0.81, 0.99)
}

@media all and (max-width: 1500px){.heading-cta{width:auto}}
@media all and (max-width: 700px){.heading-cta{margin-top:1.8rem}}
@media all and (max-width: 550px){.heading-cta{padding:0.8rem 2rem}}

.heading-cta:before,.heading-cta:after{
    content:'';
    position:absolute;
    top:-2px;left:-2px;
    width:27.5rem;
    height:4.8rem;
    border-radius:3px;
    border:1px solid #64ffda;
    filter:blur(0);
    transform-origin:50%;
    z-index:-1;
}


@media all and (max-width: 1500px){.heading-cta:before,.heading-cta:after{width:27.8rem}}
@media all and (max-width: 1200px){.heading-cta:before,.heading-cta:after{width:28.5rem;border:2px solid transparent}}

.heading-cta:hover{
    transform:translateY(-2px)}
    
.heading-cta:hover:before,.heading-cta:hover:after{
    border-color:transparent;
    filter:blur(2px);
    transform:scaleX(1.3) scaleY(2.2);
    transition:800ms transform ease, 1900ms blur ease, 700ms border-color ease;
    pointer-events:none
}

.heading-cta:hover:after{transition-delay:150ms}

.heading-cta:active{transform:translateY(-1px)}

.heading__arrow{
    display:inline-block;
    height:24px;
    width:24px;
    margin-left:15px;
    transform:rotate(90deg);
    fill:#64ffda;
    transition:all 0.3s
}

@media all and (max-width: 770px){.heading__arrow{height:20px;width:20px}}
@media all and (max-width: 615px){.heading__arrow{margin-left:10px}}
@media all and (max-width: 550px){.heading__arrow{height:16px;width:16px}}