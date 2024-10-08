<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
    <style>
        html,body{
            padding:0;
            margin:0;
            justify-content: center;
            text-align: center;
            justify-items: center;
        }
        body{
            
            text-align: center;
            height:100%;
            
            justify-content: center;
            justify-items: center;
            padding:100px 150px 200px;
            margin: 80px,300px,600px;
            
            background:linear-gradient(90deg,rgba(104, 35, 35, 0.366),rgba(255, 255, 0, 0.399),rgba(255, 166, 0, 0.357),rgba(0, 128, 0, 0.357));
       cursor: pointer;
  
        }
       #container{
        
       
        padding: 0;
        color: white;
        margin-bottom: 150px;
        padding-bottom: 0;
        z-index: 5;


        }
        #container{  
            background-color: rgba(0, 0, 0, 0.528);
            border-radius:50px;
            border: none;
            }
           #counter button{
                background:linear-gradient(rgb(101, 44, 44),rgba(255, 255, 0, 0.546),rgba(93, 75, 75, 0.579),rgba(164, 124, 124, 0.699),rgb(205, 169, 169),rgb(210, 201, 146),rgb(98, 66, 33));
                border-radius: 50px;
                box-sizing: border-box;
                border-bottom: 50px;
                box-shadow: linear-gradient(rgb(77, 77, 134),rgb(65, 123, 65),rgb(100, 100, 49),rgb(75, 30, 30),rgba(245, 245, 245, 0.767));
           align-items: center;
            }
    </style>
</head>
<body>
    <div id="container">
        <h1 id="main">0</h1>
    
    <div id="counter">
        <button id="increase">increase</button>
        <button id="reset">reset</button>
        <button id="decrease">decrease</button>
    </div> 
</div>
<script>
    let main=document.getElementById("main");
    let increase=document.getElementById("increase");
    let reset=document.getElementById("reset");
    let deccrease=document.getElementById("decrease");
    let cur=0;
    increase.addEventListener("click",()=>{
        cur++;
        main.textContent=cur;
    });
    reset.addEventListener("click",()=>{
        cur=0;
       main.textContent=cur;
    });
    decrease.addEventListener("click",()=>{
        cur--;
        main.textContent=cur;
    });
</script>
</body>
</html>
