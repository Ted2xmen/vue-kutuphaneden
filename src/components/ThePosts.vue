<template>
       <div class="col-md-8 order-1">
          <!-- <TheTopRow /> -->
        <h5 class="border border-warning p-2">
          ✨Seçilmiş Blog Yazıları ⭐⭐⭐⭐⭐
        </h5>
        <div class=" ">
          <ul v-for="(post, index) in 7" :key="index" class="list-group list-group-flush" id="blog-post">
            <li class="m-2 p-2">
                <span>
                    <img src="https://pbs.twimg.com/profile_images/1132919325545947136/dZl1s-5u_400x400.png" alt="" style="width: 34px;">
                    <a href="">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed, nisi.</a>
                </span>
             
            </li>
        
          </ul>
        </div>
            
      </div>
</template>