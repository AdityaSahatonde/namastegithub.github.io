#main{
    position: relative;
    display: flex;
    background-color: #5089C6;
    justify-content: space-around;
    align-items: center;
    width: 100vw;
    height: 100vh;
}
#section{
    
   position: relative;
    border: 1px solid black;
    background-color: white;
    border-radius: 5px;
    padding: 1%;
    width: 50vw;
   
    
}
#h1{
    margin-left: 20vw;
    font-size: 30px;
   align-self: center;
}
#input{
    margin-left: 25px;
    width: 70%;
    height: 30px;
    /* align-self: center;
    justify-content: center; */

}
table{


    border-collapse: collapse;
    border-spacing: 0px;
    width: 87%;
    border: 1px solid #ddd;
     margin-left: 25px;
    /* margin-top: 5px; */
    /* padding: 10px; */
   
  
}
tr:nth-child(even){background-color: #f2f2f2}
td {
    text-align: center;
}
 .button{
    
    width: 15%;
    height: 35px;
    background-color: greenyellow;
    border-radius: 5px;
    color: black;
    font-size: 15px;
    font-weight: bold;
    /* align-self: center;
    align-items: center; */

} 
:hover button{
    cursor: pointer;
}
img{
    width: 20px;
    height: 20px;
}
body{
    margin: none;
    padding: none;
}
p{  
    align-content: center;
    justify-content: center;
 
    text-align: end;
}
/* below media query is for upto 660px screen */
@media only screen and (max-width:660px){
    #h1{
        margin-left: 25vw;
        font-size: 30px;
       align-self: center;
    }
    .button{
        display: inline-block;
        text-align: center;
        width: 28%;
        height: 35px;
        background-color: greenyellow;
        border-radius: 5px;
        color: black;
        font-size: 10px;
        font-weight: medium;
       
        /* align-self: center;
        align-items: center; */
    
    }
    table{
        /* display: flex; */
      
        margin-left: 25px;
        
        width: 85%;
        border: 1px solid #ddd;
    }
    #input{
        display: inline-block;
        border: 1px solid black;
        margin-left: 25px;
        width: 55%;
        height: 30px;
        /* align-self: center;
        justify-content: center; */
    
    }
    #section{
    
    
         
        border: 1px solid black;
        background-color: white;
        border-radius: 5px;
      
        margin-right: 20px;
        margin-bottom: 10px;
        width: 80vw;
       
        
    }
  
    

}
@media only screen and (max-width:280px){
    #h1{
        margin-left: 13vw;
        font-size: 30px;
       align-self: center;
    }
    .button{
        display: inline-block;
        text-align: center;
        width: 35%;
        height: 35px;
        background-color: greenyellow;
        border-radius: 5px;
        color: black;
        font-size: 10px;
        font-weight: medium;
       
           
    }
    table{
           
        margin-left: 25px;
          
        width: 85%;
        border: 1px solid #ddd;
    }
    #input{
        display: inline-block;
        border: 1px solid black;
        margin-left: 25px;
        width: 55%;
        height: 30px;
      
    
    }
    #section{
    
        position: relative;
        scroll-behavior: scroll;
         /* justify-content: center; */
         border: 1px solid black;
         background-color: white;
         border-radius: 5px;
         /* box-shadow: 10px 10px #F2E1C1; */
         margin-right: 20px;
         margin-bottom: 10px;
         width: 80vw;
         /* height: calc(10px + 100px); */
         
     }
  
    

}
/* This media query for up to 320px screen */
@media only screen and (max-width:320px){
   
    .button{
        display: inline-block;
        text-align: center;
        width: 25%;
        height: 35px;
        background-color: greenyellow;
        border-radius: 5px;
        color: black;
        font-size: 10px;
        font-weight: medium;
       
        /* align-self: center;
        align-items: center; */
    
    }
   
    #input{
        display: inline-block;
        margin-left: 25px;
        width: 55%;
        height: 30px;
        border: 1px solid black;
        /* align-self: center;
        justify-content: center; */
    
    }
    #section{
    
    
         
         border: 1px solid black;
         background-color: white;
         border-radius: 5px;
       
         margin-right: 20px;
         margin-bottom: 10px;
         width: 80vw;
        
         
     }
  
    

}
