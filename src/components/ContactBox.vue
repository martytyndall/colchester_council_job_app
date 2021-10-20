<template lang="en">
    <div>
        
        <div class="contactMe-container">
          <div class="inner-container-left">
            <i class="fa fa-arrow-circle-o-right" aria-hidden="true"></i>
          </div>
          
          <div class="inner-container-right">
            <h5>Send me a message using the contact form I created</h5>
            <a href="Contact">Get in touch</a>
          </div>
          
        
  </div>        
    </div>
</template>

<script>
export default {
    name: 'ContactBox'
}
</script>

<style scoped>

.fa{
  background-color: #F2F2F2;
  color: gray;
  font-size: 40px;
  float: right;
}

.contactMe-container{
    background-color: #F2F2F2;
    height: 130px;
}

.inner-container-left{
  float: left;
  width: 60px;
  height: 130px;
  -ms-transform: translateY(30%);
  transform: translateY(30%);
}

.inner-container-right{
  float: right;
  border-left: 5px solid grey;
  height: 70px;
  width: 290px;
  -ms-transform: translateY(40%);
  transform: translateY(40%);
}

.inner-container-right h5 {
  padding-left: 10px;
  padding-bottom: 10px;
}

.inner-container-right a {
  padding-left: 10px;
}
    
</style>
