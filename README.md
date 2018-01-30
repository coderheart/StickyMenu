# StickyMenu

/* menu  sticky */
    var header = $('.main_menu');
    var win = $(window);
    
    win.on('scroll', function() {
        var scroll = win.scrollTop();
        if (scroll < 50) {
            header.removeClass("sticky");
        } else {
            header.addClass("sticky");
        }
    });
    
    
    //css here
    .main_menu.sticky {
    background: #fff none repeat scroll 0 0;
    box-shadow: 0 1px 3px rgba(50, 50, 50, 0.4);
    left: 0;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 999999;
    transition: all 1s ease 0s;
  }
