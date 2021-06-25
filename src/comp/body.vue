<template>
<div id="main1">
    <div id="container">
        <article class="item1"><a href="././img.html" ><img src="img/pic01.jpg" alt="image"></a></article>
        <article class="item2"><a href="././img.html" ><img src="../assets/img/pic06.jpg" alt="image"></a></article>
        <article class="item3"><a href="././img.html" ><img src="../assets/img/pic09.jpg" alt="image"></a></article>
        <article class="item4"><a href="././img.html" ><img src="../assets/img/pic13.jpg" alt="image"></a></article>
        <article class="item5"><a href="././img.html" ><img src="../assets/img/pic02.jpg" alt="photo"></a></article>
        <article class="item6"><a href="././img.html" ><img src="../assets/img/pic12.jpg" alt="photo"></a></article>
        <article class="item7"><a href="././img.html" ><img src="../assets/img/pic05.jpg" alt="photo"></a></article>    
        <article class="item8"><a href="././img.html" ><img src="../assets/img/pic14.jpg" alt="photo"></a></article>  
          
    </div>
    <div id="container">
        <article class="item1"><a href="././img.html" ><img src="../assets/img/pic03.jpg" alt="image"></a></article>
        <article class="item2"><a href="././img.html" ><img src="../assets/img/pic08.jpg" alt="image"></a></article>
        <article class="item3"><a href="././img.html" ><img src="../assets/img/pic11.jpg" alt="image"></a></article>
        <article class="item4"><a href="././img.html" ><img src="../assets/img/pic15.jpg" alt="image"></a></article>
        <article class="item5"><a href="././img.html" ><img src="../assets/img/pic04.jpg" alt="photo"></a></article>
        <article class="item6"><a href="././img.html" ><img src="../assets/img/pic10.jpg" alt="photo"></a></article>
        <article class="item7"><a href="././img.html" ><img src="../assets/img/pic07.jpg" alt="photo"></a></article>    
        <article class="item8"><a href="././img.html" ><img src="../assets/img/pic16.jpg" alt="photo"></a></article>  
          
    </div>
</div>
</template>

<script>
export default {
    data(){
        return{
            name:'hello world'
        }
    }
}
</script>

<style scoped>
#container{
    display:grid;
    margin-bottom:10px;
    grid-template-columns: repeat(4,1fr);
    grid-template-rows: repeat(3,1fr);
    grid-column-gap: 20px;
    grid-row-gap: 20px;
    grid-template-areas:
    "one two three four"
    "five two six four"
    "five seven six eight"
    
}
.item1{grid-area:one}
.item2{grid-area:two}
.item3{grid-area:three}
.item4{grid-area:four}
.item5{grid-area:five}
.item6{grid-area:six}
.item7{grid-area:seven}
.item8{grid-area:eight}
img{
    width:100%;
    height:100%;
    cursor: pointer;
    transition:all 0.3s ease-in-out ;
}
      @media only screen and (max-width:740px){
        #container{
            grid-template-columns: repeat(2,1fr);
            grid-template-areas:
            "five two"
            "five two"
            "one three"
            "six four"
            "six four"
            "seven eight"
        }
      }
       @media only screen and (max-width:476px){
           #container{
               grid-template-columns: 1fr;
           }
       }
article{
    overflow: hidden;
    border-radius:10px;
}
img:hover{
    transform:scale(1.2);
}
</style>
