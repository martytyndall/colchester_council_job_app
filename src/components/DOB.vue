<template>
    <div class="contact-input-fields">
        <h5>Date of birth</h5>
        <input type="date" class="" id="date" @blur="validateDOB()" placeholder="eg. 20/01/2000" required>                
    </div>   
</template>

<script>



export default{
    name: 'DOB',

    methods: {
        validateDOB(){
            // create new date object and pass in the value of the DOB element
            var dob = new Date(document.getElementById("date").value);


            // calculate the difference in months from current date in time
            var month_diff = Date.now() - dob.getTime();
            
            // convert the calculated difference in date format
            var age_dt = new Date(month_diff); 
            
            //extract year from date    
            var year = age_dt.getUTCFullYear();
            
            //now calculate the age of the user
            var age = Math.abs(year - 1970);
            
            //display the calculated age
            if(age < 18 ){
                alert("You must be over 18");
            }

            return age;            
        },
    },
}


</script>

<style scoped>
      
    input{
        width: 555px;
        height: 40px;
        padding-left: 10px;
    }
    
</style>