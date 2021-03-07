  #H1 First name: 
 Aleksandr  
  Last name:
 Smiian
 
  Contacts for communication: 
  Mail: Smiyanaleksandr@gmail.com
 Telegram: SmiyanAleksandr(+380501802809)
 
  About me:
 I strive to master javascript, because I like how a picture is created in front of my eyes and I understand that I did it, it inspires me.
 At the moment I am working, but every day I set aside time for self-study.
 
  Hard skills:
 Javascript - base
 HTML - sure
 Css/Scss - medium
 Gulp - base
 Bootstrap - base
 
  Code examples:
  $(function(){
/* Fixed Header */
let header = $("#header");
let intro= $("#intro");
let introH;
let scrollPos= $(window).scrollTop();
let nav= $("#nav");
let navToggle =$("#navToggle");

$(window).on("scroll load resize", function() {
    
    introH= intro.innerHeight();
    scrollPos = $(this).scrollTop();
    
    if(scrollPos > introH) {
        header.addClass("fixed");
    }
        else{
            header.removeClass("fixed");
        }
    
    console.log(scrollPos);
});

/*smoth scroll */
$("[data-scroll]").on("click", function(event){
    event.preventDefault();

    let elementID = $(this).data('scroll');
    let elementOffset = $(elementID).offset().top;
    
    nav.removeClass("show");

    $("html, body").animate({
        scrollTop: elementOffset - 60
    }, 700);
});

/* navToggle */

$("#navToggle").on("click", function(event){
    event.preventDefault();

    nav.toggleClass("show")
    

});


/* Reviews https://kenwheeler.github.io/slick/ */
let slider= $("#reviewsSlider");

slider.slick({
    infinite: true,
    slidesToShow: 1,
    slidesToScroll: 1,
    fade: true,
    arrows: false,
    dots: true
  });


});


  Education :
 Self-education,I learn everything myself, practice at https://www.codewars.com/
 
  English:
  A2
 
