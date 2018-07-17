# Slick

[Website](http://kenwheeler.github.io/slick/)


slick is a fully responsive slider.

A Demo slick script for a slick slider

``<script>
          jQuery('.yourclass').slick({
      dots: true,
      infinite: false,
      autoplay:true,
      arrows:true,
      speed: 300,
      slidesToShow: 4,
      slidesToScroll: 4,
      infinite: true,
      dots: true,
      responsive: [
          {
          breakpoint: 1025,
          settings: {
              slidesToShow: 4,
              slidesToScroll: 4,
          }
          },
          {
          breakpoint: 830,
          settings: {
              slidesToShow: 1,
              slidesToScroll: 1
          }
          }
          // You can unslick at a given breakpoint now by adding:
          // settings: "unslick"
          // instead of a settings object
      ]
      });
      </script>``