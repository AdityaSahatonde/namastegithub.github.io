showtask();
let input = document.getElementById("input");
let button =document.getElementById("btn")

button.addEventListener("click", function(){
    addtaskinputval = input.value;
    if(addtaskinputval.trim()!=0){
        let webtask = localStorage.getItem("localtask");
        if(webtask == null){
            taskObj = [];
        }
        else{
            taskObj = JSON.parse(webtask);
        }
        taskObj.push(addtaskinputval);
		// console.log(taskObj, 'Ashendra');
        localStorage.setItem("localtask", JSON.stringify(taskObj));
        input.value = '';
    }
    showtask();
   
});
function showtask(){
    let webtask = localStorage.getItem("localtask");
        if(webtask == null){
            taskObj = [];
        }
        else{
            taskObj = JSON.parse(webtask);
        }
    
    let newString ='';
    let table = document.getElementById("table");
           
    taskObj.forEach((itme ,index) => {
       
        newString += ` <tr>
        <th>${index + 1}</th>
        <td>${itme}</td>
        <td alig="center"><button type="button" onclick=edittask(${index})><img src="edit_icon.png" alt="" inc()></button></td>
        
        <td><button type = "button" onclick="deleteitem(${index})"><img src="delete_icon.png" alt=""></button></td>
    </tr>`;
    
        
    });
    
    table.innerHTML = newString;
    

}
function edittask(index){
    let saveindex = document.getElementById("saveindex");
    let button =document.getElementById("btn");
    let savebtn =document.getElementById("savebtn");
    saveindex.value = index;
    let webtask = localStorage.getItem("localtask");
    let  taskObj = JSON.parse(webtask);
    
    input.value = taskObj[index];
   
    button.style.display = "none";
    savebtn.style.display = "inline-block"; 
}
let savebtn =document.getElementById("savebtn");
savebtn.addEventListener("click",function(){
    let webtask = localStorage.getItem("localtask");
    let  taskObj = JSON.parse(webtask);
    let saveindex = document.getElementById("saveindex").value;
    taskObj[saveindex] = input.value;
    button.style.display = "inline-block";
    savebtn.style.display = "none";
    input.value ="";
    localStorage.setItem("localtask", JSON.stringify(taskObj));
    showtask();

});

function deleteitem(index){
    let webtask = localStorage.getItem("localtask");
    let  taskObj = JSON.parse(webtask);
    taskObj.splice(index, 1);
    localStorage.setItem("localtask", JSON.stringify(taskObj));
    button.style.display = "inline-block";
    savebtn.style.display = "none";
    input.value = "";

    showtask();

}
function inc(){
    document.getElementById("section").style.height = "250px";
}
