body {
    --megamenu-width: calc(100vw - 6rem);
    --megamenu-transition-time:500ms;
    --animation-delay: 200ms;
    
}

.header {
    transition: background-color 300ms ease;
}

.header.elementor-sticky--effects {
    background-color: #292D34!important;
    box-shadow: 0 0 10px rgba(0,0,0,0.3);
}

/* START MEGAMENU */

.megamenu-open .header.elementor-sticky--effects {
    box-shadow: none;
}

.megamenu-script {
    position: absolute;
}

div#content {
    transition: transform var(--megamenu-transition-time) ease-out;
}


body.megamenu-open div#content {
    position: relative;
    transform: translateX(calc(var(--megamenu-width) * -1 / 2))
}

body.megamenu-open {
    max-height: 100vh;
    overflow: hidden;
    padding-right: 17px;
}

.menu-popup {
    position: fixed;
    top: 0;
    right: 0;
    bottom: 0;
    width: var(--megamenu-width);
    height: 100vh;
    overflow-y: auto;
    padding: 5rem;
    z-index: 20;
    transform: translateX(110%);
    transition: transform var(--megamenu-transition-time) ease-out!important;
    padding: 20% 10% 0;
}

.menu-popup.active {
    transform: translateX(0);
    box-shadow: 0 0 75px 10px #000000;
}


.menu-item,
.nav-toggle {
    cursor: pointer;
}

.nav-trigger {
    margin-left: auto;
    width: auto!important;
}

.menu-popup-content {
    opacity: 0;
    transition: opacity 1000ms ease-in-out 300ms,

}

.menu-popup.active .menu-popup-content {
    opacity: 1;
    transition-delay: 500ms;
}

.main-nav ul:not(.sub-menu) > li.menu-item {
    position: static;
}

.sub-menu{
	float:right;
	font-size: 14px;
}

.sub-menu a {
	font-size: 19px !important; 
}
.elementor-nav-menu--main ul.elementor-nav-menu ul.sub-menu {
	display: none !Important;
}

.elementor-nav-menu--main ul.elementor-nav-menu li.active ul.sub-menu {
	display: block !Important;
}



ul.elementor-nav-menu:not(.sub-menu) > li.menu-item {
    -webkit-transition-property: top;
    -o-transition-property: top;
    transition-property: top;
    -webkit-transition-duration: .45s;
    -o-transition-duration: .45s;
    transition-duration: .45s;
    -webkit-transition-timing-function: ease-in-out;
    -o-transition-timing-function: ease-in-out;
    transition-timing-function: ease-in-out;
}

.menu-popup.active .fade-in-left ul:not(.sub-menu) > li.menu-item  {
    -webkit-animation: FadeInLeft .25s ease-in-out;
    -o-animation: FadeInLeft .25s ease-in-out;
    animation: FadeInLeft .25s ease-in-out;
    -webkit-animation-fill-mode: both;
    -o-animation-fill-mode: both;
    animation-fill-mode: both;

}

.menu-popup.active ul.elementor-nav-menu:not(.sub-menu) > li.menu-item:nth-child(1) {
    animation-delay: calc(var(--animation-delay) * 2);
}
.menu-popup.active ul.elementor-nav-menu:not(.sub-menu) > li.menu-item:nth-child(2) {
    animation-delay: calc(var(--animation-delay) * 3);
}
.menu-popup.active ul.elementor-nav-menu:not(.sub-menu) > li.menu-item:nth-child(3) {
    animation-delay: calc(var(--animation-delay) * 4);
}
.menu-popup.active ul.elementor-nav-menu:not(.sub-menu) > li.menu-item:nth-child(4) {
    animation-delay: calc(var(--animation-delay) * 5);
}
.menu-popup.active ul.elementor-nav-menu:not(.sub-menu) > li.menu-item:nth-child(5) {
    animation-delay: calc(var(--animation-delay) * 6);
}
.menu-popup.active ul.elementor-nav-menu:not(.sub-menu) > li.menu-item:nth-child(6) {
    animation-delay: calc(var(--animation-delay) * 7);
}

.menu-popup.active .fade-in-up ul:not(.sub-menu) > li.menu-item  {
    -webkit-animation: FadeInUp .25s ease-in-out;
    -o-animation: FadeInUp .25s ease-in-out;
    animation: FadeInUp .25s ease-in-out;
    -webkit-animation-fill-mode: both;
    -o-animation-fill-mode: both;
    animation-fill-mode: both;
}

.main-nav ul:not(.sub-menu) > li.active > a,
.main-nav ul:not(.sub-menu) > li:hover > a,
.main-nav ul:not(.sub-menu) > li:hover > a.elementor-item.highlighted{
    color: var(--e-global-color-f41572a)!important;
}

.main-nav ul:not(.sub-menu) > li> a.elementor-item.highlighted {
    color: #D3D4D6!important;
}

.main-nav ul.sub-menu {
    min-width: 500px!important;
    top: 0!important;
    margin-top: 10px!important;
}

.main-nav .sub-menu li {
    --animation-delay: 100ms;
    -webkit-animation: FadeInUp .25s ease-in-out;
    -o-animation: FadeInUp .25s ease-in-out;
    animation: FadeInUp .25s ease-in-out;
    -webkit-animation-fill-mode: both;
    -o-animation-fill-mode: both;
    animation-fill-mode: both;
}

.main-nav .sub-menu li:nth-child(2) {
    animation-delay: calc(var(--animation-delay) * 1);
}
.main-nav .sub-menu li:nth-child(3) {
    animation-delay: calc(var(--animation-delay) * 2);
}
.main-nav .sub-menu li:nth-child(4) {
    animation-delay: calc(var(--animation-delay) * 3);
}
.main-nav .sub-menu li:nth-child(5) {
    animation-delay: calc(var(--animation-delay) * 4);
}
.main-nav .sub-menu li:nth-child(6) {
    animation-delay: calc(var(--animation-delay) * 5);
}
.main-nav .sub-menu li:nth-child(7) {
    animation-delay: calc(var(--animation-delay) * 6);
}
.main-nav .sub-menu li:nth-child(8) {
    animation-delay: calc(var(--animation-delay) * 7);
}
.main-nav .sub-menu li:nth-child(9) {
    animation-delay: calc(var(--animation-delay) * 8);
}
.main-nav .sub-menu li:nth-child(10) {
    animation-delay: calc(var(--animation-delay) * 9);
}
.main-nav .sub-menu li:nth-child(11) {
    animation-delay: calc(var(--animation-delay) * 10);
}
.main-nav .sub-menu li:nth-child(12) {
    animation-delay: calc(var(--animation-delay) * 11);
}
.main-nav .sub-menu li:nth-child(13) {
    animation-delay: calc(var(--animation-delay) * 12);
}
.main-nav .sub-menu li:nth-child(14) {
    animation-delay: calc(var(--animation-delay) * 13);
}
.main-nav .sub-menu li:nth-child(15) {
    animation-delay: calc(var(--animation-delay) * 14);
}
.main-nav .sub-menu li:nth-child(16) {
    animation-delay: calc(var(--animation-delay) * 15);
}
.main-nav .sub-menu li:nth-child(17) {
    animation-delay: calc(var(--animation-delay) * 16);
}

.main-nav ul:not(.sub-menu) > li > a.menu-link {
    white-space: nowrap;
}

button.nav-toggle {
    background-color: transparent;
    border: none;
    padding: 0;
    margin: 0;
    min-height: 1px;
    width: 40px;
    height: 40px;
}

button.nav-toggle:hover {
    background-color: transparent;
}

button.nav-toggle > .hamburger {
    width: 100%;
    height: 2px;
    background-color: white;
    border-radius: 100vw;
    position: relative;
    transform: rotate(0deg);
    transition: transform 500ms ease-in-out;
    transform-origin: center;
    display: block;
}

button.nav-toggle > .hamburger:nth-child(1) {
    top: -10px;
    left: 0;
}

button.nav-toggle > .hamburger:nth-child(2) {

}

button.nav-toggle > .hamburger:nth-child(3) {
    bottom: -10px;
    left: 0;
}


button.nav-toggle.active > .hamburger:nth-child(1) {
    transform: rotate(45deg);
    top: 4px;
}

button.nav-toggle.active > .hamburger:nth-child(2) {
    opacity: 0;
    transition-delay: 200ms;
}

button.nav-toggle.active > .hamburger:nth-child(3) {
    transform: rotate(-45deg);
    top: 0;
}

button.nav-toggle:focus-visible {
    outline: 1px solid var(--e-global-color-primary);
    outline-offset: 5px;
    background-color: transparent;
}

button.nav-toggle:focus {
    background-color: transparent;
}

@media (hover: hover) {
    .main-nav .sub-menu li {
        display: flex;
        align-items: flex-start;
        gap: 0.5rem;
        transition: all 300ms ease-out;
    }
    
    .main-nav .sub-menu li:after {
        content: "";
        background-image: url(/wp-content/uploads/2022/12/right-arrow-32.png);
        width: 25px;
        height: 25px;
        display: block;
        background-repeat: no-repeat;
        background-size: contain;
        opacity: 0;
        transition: all 500ms ease-out;
        margin-top: 10px;
    }
    
    .main-nav .sub-menu li:hover:after {
        opacity: 1;
        transform: translateX(10px);
    }
}

@keyframes FadeInUp {
    0% {
        opacity: 0; 
        top: 20px;
        
    }
    
    100% {
        opacity: 1; 
        top: 0px;
        
    }
}

@keyframes FadeInLeft {
    0% {
        opacity: 0; 
        margin-left: 50px;
        
    }
    
    50% {
        opacity: 0.2;
        
    }

    
    100% {
        opacity: 1; 
        margin-left: 0px;
        
    }
}

@media (max-width: 1024px) {
    .menu-popup.e-con {
        padding: 15rem 4rem;
    }
    
    .main-nav ul:not(.sub-menu) > li.menu-item  {
        transition: opacity 200ms ease;
        position: relative;
    }
    
    
    .main-nav ul:not(.sub-menu) > li.not-active {
        opacity: 0!important;
        position: absolute;
        pointer-events: none;
    }
    
    .main-nav ul.sub-menu {
        min-width: unset!important;
        left: 0px!important;
        top: 0px!important;
        margin-left: 0!important;
        position: relative!important;
        float: unset;

    }
    
    .main-nav ul.sub-menu a.elementor-sub-item.menu-link {
        border: none;
        padding-inline: 0;
    }
}


@media (max-width: 768px) {
    body {
    --megamenu-width: 96vw; 
        
    }
    
    .menu-popup.e-con {
        padding: 150px 2rem;

    }
    
    body.megamenu-open .header {
        padding-right: 1rem;
    }
    
    button.nav-toggle {
        width: 30px;
        height: 30px;
    }
    
    button.nav-toggle > .hamburger:nth-child(1) {
        top: -10px;
    }
    
    button.nav-toggle > .hamburger:nth-child(3) {
        bottom: -10px;
    }
    
    button.nav-toggle.active > .hamburger:nth-child(1) {
        top: 4px;
    }

}

/* END MEGAMENU */
/* PAGE TRANSITIONS */
.elementor-kit-8 e-page-transition {
    background-image: url(/wp-content/uploads/2023/01/cropped-ARMA-GIDEON.png);
    background-repeat: no-repeat;
    background-size: 70px;
    background-position: center;
}

e-preloader[type=spinners] {
	border-width: 3px!important;
}
