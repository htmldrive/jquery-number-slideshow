jquery-number-slideshow
=======================

Simple and practical numbers image slideshow jQuery plugin

[![Number slideshow - simple and practical numbers image slideshow jQuery plugin](http://www.htmldrive.net/media/2010/9/13/1284364807.png "Number slideshow - simple and practical numbers image slideshow jQuery plugin")](http://www.htmldrive.net/items/demo/570/Number-slideshow-simple-and-practical-numbers-image-slideshow-jQuery-plugin "Number slideshow - simple and practical numbers image slideshow jQuery plugin")

[**Demo**](http://www.htmldrive.net/items/demo/570/Number-slideshow-simple-and-practical-numbers-image-slideshow-jQuery-plugin "Number slideshow - simple and practical numbers image slideshow jQuery plugin")

##Usage
**Include js and css files.**

    <link href="css/number_slideshow.css" rel="stylesheet" type="text/css" />  
    <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.4.0/jquery.min.js"></script 
    <script src="js/number_slideshow.js"></script>
*Tips: image alt attribute treated as title show at top of slideshow window.*
  
**Add html.**

        <div id="number_slideshow" class="number_slideshow">
            <ul>
                <li><a href="#"><img src="images/1.jpg" width="407" height="301" alt="slideshow_large"/></a></li>
                <li><a href="#"><img src="images/2.jpg" width="407" height="301" alt="slideshow_large"/></a></li>
                <li><a href="#"><img src="images/3.jpg" width="407" height="301" alt="slideshow_large"/></a></li>
                <li><a href="#"><img src="images/4.jpg" width="407" height="301" alt="slideshow_large"/></a></li>
            </ul>
            <ul class="number_slideshow_nav">
                <li><a href="#">1</a></li>
                <li><a href="#">2</a></li>
                <li><a href="#">3</a></li>
                <li><a href="#">4</a></li>
            </ul>
            <div style="clear: both"></div>
        </div>
        
**Add startup script.**

        <script language="javascript" type="text/javascript">
            $(function() {
                $("#number_slideshow").number_slideshow({
                    slideshow_autoplay: 'enable',//enable disable
                    slideshow_time_interval: 3000,
                    slideshow_window_background_color: "#fff",
                    slideshow_window_padding: '1',
                    slideshow_window_width: '550',
                    slideshow_window_height: '332',
                    slideshow_border_size: '1',
                    slideshow_transition_speed: 500, //'normal','slow','fast' or numeral
                    slideshow_border_color: 'black',
                    slideshow_show_button: 'enable',//enable disable
                    slideshow_show_title: 'disable',//enable disable
                    slideshow_button_text_color: '#CCC',
                    slideshow_button_current_text_color: '#000',
                    slideshow_button_background_color: '#333',
                    slideshow_button_current_background_color: '#666',
                    slideshow_button_border_color: '#000',
                    slideshow_loading_gif: 'loading.gif',//loading pic, you can replace it.
                    slideshow_button_border_size: '1'
                });
            });
        </script>