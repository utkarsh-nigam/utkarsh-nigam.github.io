<h1>Typewriter</h1>


<p id="line"></p>
<p id="line2"></p>

<script>
var i = 0;
var txt_1 = 'I am Utkarsh Nigam.'
var txt_2='M.S. Data Science Student at The George Washington University, Washington, D.C.';
var speed = 75;

function typeWriter(txt,p_id) {
    var i = 0;
    function typeWriter1(){
        if (i < txt.length) {
            document.getElementById(p_id).innerHTML += txt.charAt(i);
            i++;
            setTimeout(typeWriter1, speed);}
  }
  typeWriter1()
}


typeWriter(txt_1,"line")
setTimeout(typeWriter, 1800,txt_2,"line2")

</script>
