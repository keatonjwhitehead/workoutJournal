<template>
     <div>
          <form>
               <div id="form-header">
                    <slot name ="form-header"></slot>
               </div>
               <div id="form-fields">
                    <slot name ="form-fields"></slot>
               </div>
               <div id="form-controls">
                    <slot name ="form-controls"></slot>
               </div>
               <div id="useful-links">
                    <ul>
                         <li><a href="#">Link 1 </a></li>
                         <li><a href="#">Link 2 </a></li>
                         <li><a href="#">Link 3 </a></li>
                         <li><a href="#">Link 4 </a></li>
                    </ul>
               </div>
          </form>
     </div>
</template>

<script>
     export default{
          components:{

          },
          data(){
               return{

               }
          },
          methods:{

          }
     }
</script>

<style scoped>
     h1{
          text-align: center;
     }
     form{
     margin: 20px auto;
     max-width: 500px;
     }
     #useful-links ul{
          padding: 0;
     }
     #useful-links li{
          display: inline-block;
          margin-right: 10px;
     }
     form > div{
          padding: 20px;
          background: #eee;
          margin: 20px 0;
     }
     #form-header{
          background: #ddd;
          border: 1px solid #bbb;
     }
     textarea{
          display: block;
          width: 80%;
          padding: 8px;
     }
</style>
