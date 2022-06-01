var form = document.getElementById("formm")

addEventListener('submit',function(r){
    r.preventDefault()

    var search = this.document.getElementById("name").value
    document.getElementById("result").innerHTML=""
    fetch("https://api.github.com/users/"+search)
    .then((result) => result.json())
    .then((data) => {
        this.document.getElementById("result").innerHTML = 
        <a target="_blank" href="https://www.github.com/${Search}">click here</a>
    })
}
)