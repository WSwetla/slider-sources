# [slider-sources](https://wswetla.github.io/slider-sources/)



let offset = 0;
const destinationSlider = document.querySelector('.destinations-cards');
let width = document.querySelector('.card-big').offsetWidth;

document.querySelector('.vect1').addEventListener('click', function() {
   offset = offset + width;
   if (offset > width) {
      offset = 0;
   }
   destinationSlider.style.left = offset + 'px';
});

document.querySelector('.vect2').addEventListener('click', function() {
   offset = offset - width;
   if (offset <= width) {
      offset = 0;
   }
   destinationSlider.style.left = -offset + 'px';
});

document.querySelector('.vect3').addEventListener('click', function() {
   offset = offset + width;
   if (offset > 1000 ) {
      offset = 0;
   }
   destinationSlider.style.left = -offset + 'px';
});

document.querySelector('.vect4').addEventListener('click', function() {
   offset = offset + width;
   if (offset > width) {
      offset = 0;
   }
   destinationSlider.style.left = offset + 'px';
});

document.querySelector('.vect5').addEventListener('click', function() {
   offset = offset - width;
   if (offset <= width) {
      offset = 0;
   }
   destinationSlider.style.left = -offset + 'px';
});

document.querySelector('.vect6').addEventListener('click', function() {
   offset = offset + width;
   if (offset > width + 1000) {
      offset = 0;
   }
   destinationSlider.style.left = -offset + 'px';
});


let vector = document.querySelectorAll('.vect4 img, vect5, .vect6');

vector.addEventListener('click', ()=> {
   vector.classList.toggle('active');
});

function sliderMenu(){
   document.getElementsByClassName('.vect4').classList.toggle('active');
   // document.getElementById('header-nav').classList.toggle('active');
   // document.getElementById('overlay').classList.toggle('active');
}

const sliderLittle = document.querySelector('.slider');
let widthLittle = document.querySelector('.title-cards').offsetWidth;

document.querySelector('.arrow-l').addEventListener('click', function() {
   offset = offset + width;
   if (offset > width) {
      offset = 0;
   }
   sliderLittle.style.left = offset + 'px';
});
