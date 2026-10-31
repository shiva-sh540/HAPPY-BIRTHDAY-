
function celebrate(){

    music.play();

    alert("❤️ Happy Birthday Aarushi Di ❤️\n\nMay your smile shine as brightly as today!");

    for(let i=0;i<200;i++){
        let confetti=document.createElement("div");

        confetti.className="confetti";
        confetti.style.left=Math.random()*100+"vw";
        confetti.style.background=
        `hsl(${Math.random()*360},100%,50%)`;

        confetti.style.animationDuration=
        (2+Math.random()*3)+"s";

        document.body.appendChild(confetti);

        setTimeout(()=>{
            confetti.remove();
        },5000);
    }
}
