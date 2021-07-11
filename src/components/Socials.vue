<template>
    <h4>Follow me</h4>   
    <i class="fa fa-facebook" aria-hidden="true"></i>  
    <i class="fa fa-twitter" aria-hidden="true"></i>  
    <i class="fa fa-linkedin" aria-hidden="true"></i>  
    <i class="fa fa-youtube" aria-hidden="true"></i>
    
</template>

<script>

export default{
    name: 'Socials',
}
</script>

<style scoped>
    i {
      font-size: 50px;
      text-decoration: none;
      margin-top: 50px;
      width: 60px;
      height: 60px;
      text-align: center;
    }

    .fa-facebook{
      color: #4360B4;
    }
    
    .fa-twitter{
      color: #41AAF1;
    }
    
    .fa-linkedin{
      color: #0072B1;
    }
    
    .fa-youtube{
      color: #FF0000;
    }

  .fa{
    background-color: white;
  }
</style>