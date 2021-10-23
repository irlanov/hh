<!DOCTYPE html>
<html>  
    <head>
        <title>Jupiter</title>
    </head>
    <body>
    
    <form onsubmit="javascript:return false; " id="form">
    
        <input class="text" placeholder="Write...">
            
        <button class="math" onclick="display()">Send</button>
        
        </form>      
        
        <script>
        
        function display() {
            let txt = document.querySelector(".text");
            let show = document.createElement('p')
            show.classList.add('.show')
            let value = txt.value
            if(value != ""){
               show.innerText =value + ' ' + new Date().toLocaleTimeString()
                document.body.append(show)
               form.reset() 
            }
         }  
                                          
        </script>
        
    </body>
</html>
