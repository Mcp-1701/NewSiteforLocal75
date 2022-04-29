<section data-bs-version="5.1" class="menu menu1" group="Menu" plugins="DropDown, TouchSwipe" always-top global once="menu" not-draggable position-absolute>
    <mbr-parameters>
        <header>Size</header>
        <input type="checkbox" name="fullWidth" title="Full Width" checked>
        <header>Show/Hide</header>
        <input type="checkbox" title="Logo" name="showLogo" checked>
        <input type="range" title="Logo Size" inline name="logoSize" min="3" max="8" step="0.1" value="8" condition="showLogo">
        <input type="checkbox" title="Brand Name" name="showBrand">
        <input type="checkbox" title="Menu Items" name="showItems" checked>
        <input type="checkbox" title="Button" name="showButton" checked>
        <header>Text</header>
        <input type="color" title="Colored" value="#ffd54d" name="coloredTextColor">
        <header>Styles</header>
        <input type="checkbox" title="Sticky" name="sticky" checked>
        <input type="checkbox" title="Collapsed" name="collapsed">
        <input type="checkbox" title="Transparent" name="transparent" checked>
        <input type="range" title="Opacity" name="bgOpacity" min="0" max="1" step="0.1" value="1" condition="transparent">
        <input type="color" title="Color" name="menuBgColor" value="#161616">
        <input type="color" title="Hamburger" name="hamburgerColor" value="#eeeeee">
    </mbr-parameters>
    <nav class="navbar navbar-dropdown" mbr-class="{'navbar-fixed-top':sticky, 'navbar-expand-lg':!collapsed, 'collapsed':collapsed}">
        <div mbr-class="{'container': !fullWidth, 'container-fluid': fullWidth}">
            <div class="navbar-brand">
                <span mbr-if="showLogo" class="navbar-logo">
                    <a href="index.html">
                        <img src="file:///C:/Users/dc-co/AppData/Local/Mobirise.com/Mobirise/projects/project-2022-04-26_231055/assets/images/logo%20+%20name%20gold%20s-438x217.png" alt="Local 75" mbr-style="{'height': logoSize + 'rem'}">
                    </a>
                </span>
                <span mbr-if="showBrand" mbr-buttons mbr-theme-style="display-5" class="navbar-caption-wrap mbr-text" data-toolbar="-mbrBtnMove,-mbrBtnAdd,-mbrBtnRemove,-iconFont"><a class="navbar-caption text-secondary" data-app-selector=".navbar-caption" href="https://mobiri.se" data-app-placeholder="Type Text">Local 75</a></span>
            </div>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-bs-toggle="collapse" data-target="#navbarSupportedContent" data-bs-target="#navbarSupportedContent" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation" mbr-if="showItems || showButton">
                <div class="hamburger">
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
            </button>
            <div class="collapse navbar-collapse justify-content-end text-center" id="navbarSupportedContent" mbr-if="showItems || showButton">
                <ul mbr-menu class="navbar-nav nav-dropdown" mbr-theme-style="display-7" mbr-if="showItems" mbr-class="{'flex-grow-1 d-flex justify-content-center': showButton && showItems,'navbar-nav-top-padding': isPublish && !showBrand && !showLogo}"><li class="nav-item">
                        <a class="nav-link link text-secondary text-primary" href="index.html#pricing01-l" data-app-selector=".nav-link,.dropdown-item" data-app-placeholder="Type Text" aria-expanded="false">Home</a>
                    </li><li class="nav-item"><a class="nav-link link text-secondary text-primary" href="page3.html" data-app-selector=".nav-link,.dropdown-item" data-app-placeholder="Type Text">Our Menu</a></li><li class="nav-item">
                        <a class="nav-link link text-secondary text-primary" href="page1.html" data-app-selector=".nav-link,.dropdown-item" data-app-placeholder="Type Text">Gallery</a>
                    </li>
                    <li class="nav-item"><a class="nav-link link text-secondary text-primary" href="page2.html" data-app-selector=".nav-link,.dropdown-item" data-app-placeholder="Type Text">Contact us</a></li><li class="nav-item"><a class="nav-link link text-secondary text-primary" href="index.html#pricing01-l" data-app-selector=".nav-link,.dropdown-item" data-app-placeholder="Type Text">Francais</a></li></ul>
                <div mbr-if="showButton" mbr-buttons="true" mbr-theme-style="display-4" data-toolbar="-mbrBtnMove,-mbrBtnRemove,-mbrBtnAdd, -iconFont"><a class="btn rounded-pill shadow-none px-3 btn-primary-outline" data-app-placeholder="Type Text" href="index.html#form01-n">Order Now</a></div>
            </div>
        </div>
    </nav>
</section>
<section data-bs-version="5.1" class="header02" group="Header" mbr-class="{'mbr-fullscreen': fullScreen,
'mbr-parallax-background': bg.parallax}">
    <mbr-parameters>
        <header>Size</header>
        <input type="checkbox" title="Full Screen" name="fullScreen" checked>
        <input type="checkbox" title="Full Width" name="fullWidth" checked>
        <input type="range" inline title="Top" name="paddingTop" min="0" max="10" step="1" value="6" condition="fullScreen == false">
        <input type="range" inline title="Bottom" name="paddingBottom" min="0" max="10" step="1" value="6" condition="fullScreen == false">
        <header>Show/Hide</header>
        <input type="checkbox" title="Title" name="showTitle" checked>
        <input type="checkbox" title="Subtitle" name="showSubitle" checked>
        <input type="checkbox" title="Text" name="showText">
        <header>Text</header>
        <input type="color" title="Colored" value="#ffd54d" name="coloredTextColor">
        <header>Content</header>
        <select title="Align" name="alignText">
            <option value="start">Left</option>
            <option value="center">Center</option>
            <option value="end" selected>Right</option>
        </select>
        <header>Background</header>
        <fieldset type="background" name="bg" parallax>
            <input type="image" title="Image" value="file:///C:/Users/dc-co/AppData/Local/Mobirise.com/Mobirise/projects/project-2022-04-26_231055/assets/images/img1-1.jpg" selected parallax>
            <input type="color" title="Color" value="#414142">
        </fieldset>
        <input type="checkbox" title="Overlay" name="overlay" condition="bg.type !== 'color'" checked>
        <input type="color" title="Overlay Color" name="overlayColor" value="#000000" condition="overlay && bg.type !== 'color'">
        <input type="range" inline title="Opacity" name="overlayOpacity" min="0" max="1" step="0.1" value="0.7" condition="overlay && bg.type !== 'color'">
    </mbr-parameters>

    <div class="mbr-overlay" mbr-if="overlay && bg.type !== 'color'" opacity="{{overlayOpacity}}" bg-color="{{overlayColor}}"></div>

    <div class="px-0 pb-md-3 px-sm-3" mbr-class="{'container': !fullWidth, 'container-fluid': fullWidth}">
        <div class="row mb-5 mx-0 mx-sm-5" mbr-if="showTitle">
            <div class="col-12 px-sm-3">
                <h1 class="mbr-section-title mbr-fonts-style" mbr-theme-style="display-1" data-app-selector=".mbr-section-title" data-app-placeholder="Type Text">
                    Burger</h1>
            </div>
        </div>
        <div class="row justify-content-{{alignText}} mx-0 mx-sm-5">
            <div class="mb-5 mb-md-0 col-12 col-md-6 px-sm-3">
                <h2 class="mbr-section-subtitle mbr-fonts-style mb-4" data-app-selector=".mbr-section-subtitle" mbr-theme-style="display-5" mbr-if="showSubitle" data-app-placeholder="Type Text">
                Enjoy <i class="colored-text">our burgers,</i> made from<br>Grade A Angus beef</h2>
                <p mbr-if="showText" class="mbr-text mbr-fonts-style m-0 pe-2" data-app-selector=".mbr-text" mbr-theme-style="display-7" data-app-placeholder="Type Text">
                    Purus in mollis nunc sed id. Sed arcu non odio euismod
                    lacinia at. Lorem ipsum dolor sit amet consectetur
                    adipisicing elit. Architecto inventore aliquam veritatis.
                </p>
            </div>
        </div>
    </div>
</section>
<section data-bs-version="5.1" class="features01" group="Features" mbr-class="{
    'mbr-fullscreen': fullScreen,
    'mbr-parallax-background': bg.parallax}">
    <mbr-parameters>
        <header>Size</header>
        <input type="checkbox" title="Full Screen" name="fullScreen">
        <input type="checkbox" title="Full Width" name="fullWidth">
        <input type="range" inline title="Top" name="paddingTop" min="0" max="10" step="1" value="6" condition="fullScreen == false">
        <input type="range" inline title="Bottom" name="paddingBottom" min="0" max="10" step="1" value="6" condition="fullScreen == false">
        <header>Row</header>
        <input type="checkbox" title="Title" name="rowTitle" checked>
        <input type="checkbox" title="Text" name="rowText" checked>
        <input type="checkbox" title="Number" name="rowNumber">
        <select title="Amount" name="rowAmount">
            <option value="1">1</option>
            <option value="2" selected>2</option>
            <option value="3">3</option>
        </select>
        <input type="color" title="Line" name="rowLine" value="#EEEEEE">
        <header>Background</header>
        <fieldset type="background" name="bg" parallax>
            <input type="image" title="Image" value="../_images/image6.jpg">
            <input type="color" title="Color" value="#161616" selected>
        </fieldset>
        <input type="checkbox" title="Overlay" name="overlay" condition="bg.type !== 'color'" checked>
        <input type="color" title="Overlay Color" name="overlayColor" value="#414142" condition="overlay && bg.type !== 'color'">
        <input type="range" inline title="Opacity" name="overlayOpacity" min="0" max="1" step="0.1" value="0.7" condition="overlay && bg.type !== 'color'">
    </mbr-parameters>

    <div class="mbr-overlay" mbr-if="overlay && bg.type !== 'color'" opacity="{{overlayOpacity}}" bg-color="{{overlayColor}}"></div>

    <div mbr-class="{'container': !fullWidth, 'container-fluid': fullWidth}" class="px-0 px-sm-3">
        <div class="row justify-content-between mx-0 mx-sm-5 pt-5 mb-2">
            <div class="col-5">
                <h5 mbr-if="rowTitle" class="mbr-section-title mbr-fonts-style pb-4" mbr-theme-style="display-5" data-app-selector=".mbr-section-title" data-app-placeholder="Type Text">a small bistro in the heart of the Monkland Village.</h5>
            </div>
            <div class="col-5 col-lg-3">
                <p mbr-if="rowText" class="mbr-text mbr-fonts-style center-col" mbr-theme-style="display-7" data-app-selector=".mbr-text.center-col" data-app-placeholder="Type Text">
                    We pride ourselves in providing an ever-changing menu selection for our customer’s ever-changing tastes
                </p>
            </div>
            <div class="col-2 ps-0">
                <p mbr-if="rowNumber" class="mbr-text mbr-fonts-style last-col" mbr-theme-style="display-3" data-app-selector=".mbr-text.last-col">
                    <i>01</i>
                </p>
            </div>
            <div class="col-12 pt-1">
                <div class="border-bottom"></div>
            </div>
        </div>
        <div mbr-if="rowAmount > 1" class="row justify-content-between mx-0 mx-sm-5 pt-5 mb-2">
            <div class="col-5">
                <h5 mbr-if="rowTitle" class="mbr-section-title mbr-fonts-style pb-4" mbr-theme-style="display-3" data-app-selector=".mbr-section-title" data-app-placeholder="Type Text">UNIQUE FLAVOURS</h5>
            </div>
            <div class="col-5 col-lg-3">
                <p mbr-if="rowText" class="mbr-text mbr-fonts-style center-col" mbr-theme-style="display-7" data-app-selector=".mbr-text.center-col" data-app-placeholder="Type Text">
                    <br>All food items, from sauces to vinaigrettes, are meticulously prepared in-house from scratch.
                </p>
            </div>
            <div class="col-2 ps-0">
                <p mbr-if="rowNumber" class="mbr-text mbr-fonts-style last-col" mbr-theme-style="display-3" data-app-selector=".mbr-text.last-col">
                    <i>02</i>
                </p>
            </div>
            <div class="col-12 pt-1">
                <div class="border-bottom"></div>
            </div>
        </div>
        <div mbr-if="rowAmount > 2" class="row justify-content-between mx-0 mx-sm-5 pt-5">
            <div class="col-5">
                <h5 mbr-if="rowTitle" class="mbr-section-title mbr-fonts-style pb-4" mbr-theme-style="display-3" data-app-selector=".mbr-section-title" data-app-placeholder="Type Text">100% Organic</h5>
            </div>
            <div class="col-5 col-lg-3">
                <p mbr-if="rowText" class="mbr-text mbr-fonts-style center-col" mbr-theme-style="display-7" data-app-selector=".mbr-text.center-col" data-app-placeholder="Type Text">
                    Lorem ipsum dolor sit amet consectetur.
                </p>
            </div>
            <div class="col-2 ps-0">
                <p mbr-if="rowNumber" class="mbr-text mbr-fonts-style last-col" mbr-theme-style="display-3" data-app-selector=".mbr-text.last-col">
                    <i>03</i>
                </p>
            </div>
            <div class="col-12 pt-1">
                <div class="border-bottom"></div>
            </div>
        </div>
    </div>
</section>
<section data-bs-version="5.1" class="article01" group="Article" mbr-class="{
    'mbr-fullscreen': fullScreen,
    'mbr-parallax-background': bg.parallax}">
    <mbr-parameters>
        <header>Size</header>
        <input type="checkbox" title="Full Screen" name="fullScreen">
        <input type="checkbox" title="Full Width" name="fullWidth">
        <input type="range" inline title="Top" name="paddingTop" min="0" max="10" step="1" value="6" condition="fullScreen == false">
        <input type="range" inline title="Bottom" name="paddingBottom" min="0" max="10" step="1" value="6" condition="fullScreen == false">
        <header>Show/Hide</header>
        <input type="checkbox" title="Title" name="showTitle" checked>
        <input type="checkbox" title="Subtitle" name="showSubtitle" checked>
        <input type="checkbox" title="Text" name="showText" checked>
        <header>Text</header>
        <input type="color" title="Colored" value="#a68462" name="coloredTextColor">
        <header>Background</header>
        <fieldset type="background" name="bg" parallax>
            <input type="image" title="Image" value="file:///C:/Users/dc-co/AppData/Local/Mobirise.com/Mobirise/projects/project-2022-04-26_231055/assets/images/img5-1.jpg" selected parallax>
            <input type="color" title="Color" value="#414142">
        </fieldset>
        <input type="checkbox" title="Overlay" name="overlay" condition="bg.type !== 'color'" checked>
        <input type="color" title="Overlay Color" name="overlayColor" value="#000000" condition="overlay && bg.type !== 'color'">
        <input type="range" inline title="Opacity" name="overlayOpacity" min="0" max="1" step="0.1" value="0.8" condition="overlay && bg.type !== 'color'">
    </mbr-parameters>

    <div class="mbr-overlay" mbr-if="overlay && bg.type !== 'color'" opacity="{{overlayOpacity}}" bg-color="{{overlayColor}}"></div>

    <div class="px-0 px-sm-3" mbr-class="{'container': !fullWidth, 'container-fluid': fullWidth}">
        <div mbr-if="showTitle" class="row mx-0 mx-sm-5 mb-1">
            <div class="col-12 mb-5 px-sm-3">
                <h3 class="mbr-section-title mbr-fonts-style" mbr-theme-style="display-2" data-app-selector=".mbr-section-title" data-app-placeholder="Type Text">
                    <i class="primary-color-text">We offer</i> delicious burgers, steaks, wings</h3>
            </div>
        </div>
        <div class="row mx-0 mx-sm-5">
            <div class="col-12 px-sm-3">
                <h4 mbr-if="showSubtitle" class="mbr-section-subtitle mbr-fonts-style pb-2" mbr-theme-style="display-5" data-app-selector=".mbr-section-subtitle" data-app-placeholder="Type Text">Tasting our food is like heaven in your mouth…</h4>
                <p mbr-if="showText" class="mbr-text mbr-fonts-style" mbr-theme-style="display-7" data-app-selector=".mbr-text" data-app-placeholder="Type Text">
                    Named after aliquam faucibus purus in. Fusce
                    ut placerat orci nulla pellentesque dignissim enim sit amet.
                    Ultricies mi eget mauris pharetra et. Sit amet est placerat
                    in egestas erat imperdiet. Lacinia quis vel eros donec ac
                    odio tempor. Elit sed vulputate mi sit amet. Volutpat diam
                    ut venenatis tellus.&nbsp;<br><br>
                    Mi ipsum faucibus vitae aliquet nec ullamcorper sit.
                    Consequat semper viverra nam libero. Viverra adipiscing at
                    in tellus. Eu feugiat pretium nibh ipsum consequat nisl vel
                    pretium lectus. Facilisi etiam dignissim diam quis enim
                    lobortis. Diam volutpat commodo sed egestas egestas
                    fringilla phasellus.&nbsp;
                </p>
            </div>
        </div>
    </div>
</section>
<section data-bs-version="5.1" class="article01" group="Article" mbr-class="{
    'mbr-fullscreen': fullScreen,
    'mbr-parallax-background': bg.parallax}">
    <mbr-parameters>
        <header>Size</header>
        <input type="checkbox" title="Full Screen" name="fullScreen">
        <input type="checkbox" title="Full Width" name="fullWidth">
        <input type="range" inline title="Top" name="paddingTop" min="0" max="10" step="1" value="6" condition="fullScreen == false">
        <input type="range" inline title="Bottom" name="paddingBottom" min="0" max="10" step="1" value="6" condition="fullScreen == false">
        <header>Show/Hide</header>
        <input type="checkbox" title="Title" name="showTitle" checked>
        <input type="checkbox" title="Subtitle" name="showSubtitle">
        <input type="checkbox" title="Text" name="showText" checked>
        <header>Text</header>
        <input type="color" title="Colored" value="#d3312a" name="coloredTextColor">
        <header>Background</header>
        <fieldset type="background" name="bg" parallax>
            <input type="image" title="Image" value="../_images/image9.jpg">
            <input type="color" title="Color" value="#161616" selected>
        </fieldset>
        <input type="checkbox" title="Overlay" name="overlay" condition="bg.type !== 'color'" checked>
        <input type="color" title="Overlay Color" name="overlayColor" value="#414142" condition="overlay && bg.type !== 'color'">
        <input type="range" inline title="Opacity" name="overlayOpacity" min="0" max="1" step="0.1" value="0.7" condition="overlay && bg.type !== 'color'">
    </mbr-parameters>

    <div class="mbr-overlay" mbr-if="overlay && bg.type !== 'color'" opacity="{{overlayOpacity}}" bg-color="{{overlayColor}}"></div>

    <div class="px-0 px-sm-3" mbr-class="{'container': !fullWidth, 'container-fluid': fullWidth}">
        <div mbr-if="showTitle" class="row mx-0 mx-sm-5 mb-1">
            <div class="col-12 mb-5 px-sm-3">
                <h3 class="mbr-section-title mbr-fonts-style" mbr-theme-style="display-2" data-app-selector=".mbr-section-title" data-app-placeholder="Type Text"><font color="#d3312a"><i>Find your best</i></font>&nbsp;tasted food &amp; drink just in one place</h3>
            </div>
        </div>
        <div class="row mx-0 mx-sm-5">
            <div class="col-12 px-sm-3">
                <h4 mbr-if="showSubtitle" class="mbr-section-subtitle mbr-fonts-style pb-2" mbr-theme-style="display-3" data-app-selector=".mbr-section-subtitle" data-app-placeholder="Type Text">
                    Enjoy our luscious dishes wherever you want
                </h4>
                <p mbr-if="showText" class="mbr-text mbr-fonts-style" mbr-theme-style="display-7" data-app-selector=".mbr-text" data-app-placeholder="Type Text">From casual lunch breaks to after-work cocktails, a spot to grab a beer while watching the game, Local 75 is the perfect gathering spot for any occasion. Drop by and join us anytime.</p>
            </div>
        </div>
    </div>
</section>
<section data-bs-version="5.1" class="image01" group="Image & Video" mbr-class="{'mbr-fullscreen': fullScreen,'mbr-parallax-background': bg.parallax}">
    <mbr-parameters>
        <header>Size</header>
        <input type="checkbox" title="Full Screen" name="fullScreen">
        <input type="range" inline title="Top" name="paddingTop" min="0" max="10" step="1" value="5" condition="fullScreen == false">
        <input type="range" inline title="Bottom" name="paddingBottom" min="0" max="10" step="1" value="5" condition="fullScreen == false">
        <input type="range" inline title="Height" name="imgHeight" min="15" max="30" step="1" value="23" condition="fullScreen == false">
        <header>Background</header>
        <fieldset type="background" name="bg" parallax>
            <input type="image" title="Image" value="../_images/image4.jpg">
            <input type="color" title="Color" value="#161616" selected>
        </fieldset>
        <input type="checkbox" title="Overlay" name="overlay" condition="bg.type !== 'color'" checked>
        <input type="color" title="Overlay Color" name="overlayColor" value="#414142" condition="overlay && bg.type !== 'color'">
        <input type="range" inline title="Opacity" name="overlayOpacity" min="0" max="1" step="0.1" value="0.7" condition="overlay && bg.type !== 'color'">
    </mbr-parameters>

    <div class="mbr-overlay" mbr-if="overlay && bg.type !== 'color'" opacity="{{overlayOpacity}}" bg-color="{{overlayColor}}"></div>

    <div class="container-fluid p-0">
        <div class="row m-0">
            <img class="p-0 image-h" src="file:///C:/Users/dc-co/AppData/Local/Mobirise.com/Mobirise/projects/project-2022-04-26_231055/assets/images/img-5020-2907x1938.jpg" alt>
        </div>
    </div>
</section>
<section data-bs-version="5.1" class="footer1 woodm4_footer1" group="Footers" data-bg-video="{{bg.type == 'video' && bg.value.url}}" mbr-class="{'mbr-parallax-background': bg.parallax}">

    <mbr-parameters>
        <!-- Block parameters controls (Blue "Gear" panel) -->
        <input type="range" inline title="Top" name="paddingTop" min="0" max="9" step="1" value="0">
        <input type="range" inline title="Bottom" name="paddingBottom" min="0" max="20" step="1" value="0">
        <input type="checkbox" title="Show Title" name="showTitle" checked>
        <input type="checkbox" title="Show Text" name="showText" checked>
        <select title="Cards" name="cardsAmount">
            <option value="1">1</option>
            <option value="2">2</option>
            <option value="3" selected>3</option>
        </select>
        <input type="color" title="Icons Color" name="icons" value="#ffffff" selected>
        <fieldset type="background" name="bg" parallax>
            <input type="image" title="Background Image" value="file:///C:/Users/dc-co/AppData/Local/Mobirise.com/Mobirise/karenfigueroagarcia1_0040gmail_002ecom/addons/woodm4/components/_images/bakground5.jpg" parallax>
            <input type="color" title="Background Color" value="#161616" selected>
            <input type="video" title="Background Video" value="https://www.youtube.com/watch?v=36YgDDJ7XSc">
        </fieldset>
        <input type="checkbox" title="Overlay" name="overlay" checked condition="bg.type !== 'color'">
        <input type="color" title="Overlay Color" name="overlayColor" value="#efefef" condition="overlay && bg.type !== 'color'">
        <input type="range" inline title="Opacity" name="overlayOpacity" min="0" max="1" step="0.1" value="0.9" condition="overlay && bg.type !== 'color'">
        <!-- End block parameters -->
    </mbr-parameters>

    <div class="mbr-overlay" mbr-if="overlay && bg.type!== 'color'" mbr-style="{'opacity': overlayOpacity, 'background-color': overlayColor}">
    </div>

    <div class="container">
        <div class="row">
            <div class="col-12 align-center">
                <img src="file:///C:/Users/dc-co/AppData/Local/Mobirise.com/Mobirise/projects/project-2022-04-26_231055/assets/images/logo%20gold-114x191.png" alt="Local 75">
            </div>
            <div class="card p-3 col-12 col-md-6" mbr-class="{'col-lg-3': cardsAmount == '4',
                            'col-lg-4': cardsAmount == '3'}">
                <div class="card-box">
                    <h4 class="card-title mbr-bold mbr-fonts-style" mbr-theme-style="display-5" mbr-if="showTitle" data-app-selector=".card-title, .card-img">
                        Address
                    </h4>
                    <p class="mbr-text mbr-fonts-style" mbr-theme-style="display-7" mbr-if="showText" data-app-selector=".mbr-text"><a href="https://g.page/local75bistro?share" class="text-primary" target="_blank">5601 Monkland Avenue
</a><br><a href="https://g.page/local75bistro?share" class="text-primary" target="_blank">Montréal, QC H4A 1E2</a></p>
                </div>
            </div>

            <div class="card p-3 col-12 col-md-6" mbr-if="cardsAmount > 1" mbr-class="{'col-lg-3': cardsAmount == '4',
                            'col-lg-4': cardsAmount == '3'}">
                <div class="card-box">
                    <h4 class="card-title mbr-bold mbr-fonts-style" mbr-theme-style="display-5" mbr-if="showTitle" data-app-selector=".card-title, .card-img">
                        Hours</h4>
                    <p class="mbr-text mbr-fonts-style" mbr-theme-style="display-7" mbr-if="showText" data-app-selector=".mbr-text">Monday 5–10p.m.<br>Tuesday 5–10 p.m.<br>Wednesday 5–10 p.m.
<br>Thursday 5–11 p.m.<br>Friday 5–11 p.m.
<br>Saturday 5–11 p.m.
<br>Sunday Closed
<br>
<br>	
<br><br></p>
                </div>
            </div>

            <div class="card p-3 col-12 col-md-6" mbr-if="cardsAmount > 2" mbr-class="{'col-lg-3': cardsAmount == '4',
                            'col-lg-4': cardsAmount == '3'}">
                <div class="card-box">
                    <h4 class="card-title mbr-bold mbr-fonts-style" mbr-theme-style="display-5" mbr-if="showTitle" data-app-selector=".card-title, .card-img">
                        Contact</h4>
                    <p class="mbr-text mbr-fonts-style" mbr-theme-style="display-7" mbr-if="showText" data-app-selector=".mbr-text"><a href="tel:+15144847575" class="text-primary">514-484-7575</a></p>
                </div>
            </div>

            <div class="col-lg-12 pt-5 align-center">
                <div class="icon-wrap">
                    <a href="http://facebook.com/local75bistro" target="_blank"><span mbr-icon class="mbr-iconfont socicon-facebook socicon" style="color: rgb(255, 213, 77); fill: rgb(255, 213, 77);"></span></a><br>
                    <span mbr-icon class="mbr-iconfont socicon-instagram socicon"></span>
                </div>
            </div>
        </div>
    </div>
</section>
